# StokFlow

Yerel stok, sipariş, PDF fatura/irsaliye ve pazaryeri yapılandırması. FastAPI + React (Vite).

## Özellikler

- **Stok:** Ürün CRUD, kritik eşik
- **Sipariş:** Oluşturma, durum, kalemler, PDF fatura ve irsaliye
- **Pazaryeri:** Trendyol / Hepsiburada / N11 anahtarları (Fernet ile şifreli) ve simülasyon veya canlı HTTP
- **API:** FastAPI `/docs`

## Kurulum

1. Python 3.11+

2. Proje dizinine girin (depo kökünde `Firoşgeh` klasörü).
   ```bash
   cd Firoşgeh
   ```

3. Bağımlılıklar:
   ```bash
   pip install -r requirements.txt
   ```

4. Ortam:
   ```bash
   cp .env.example .env
   ```
   **FERNET_KEY** (pazaryeri kaydı için zorunlu): `openssl rand -base64 32` çıktısını `.env` içine yazın. Anahtar boş bırakılırsa ürün/sipariş/PDF çalışır; pazaryeri oluşturma/güncelleme 503 döner.

5. Sunucu:
   ```bash
   python -m uvicorn app.main:app --reload --host 127.0.0.1 --port 8000
   ```

6. API: http://127.0.0.1:8000/docs

### Frontend

Proxy: `frontend/vite.config.ts` → `/products`, `/orders`, `/marketplaces` → `127.0.0.1:8000`.

```bash
cd frontend
npm install
npm run dev
```

Arayüz: http://127.0.0.1:5173

Production veya `vite preview` için `frontend/.env` ile `VITE_API_URL=http://127.0.0.1:8000`; backend `CORS_ORIGINS` içinde origin olmalı.

**Not:** `GET /` statik `static/index.html` dönebilir; geliştirme arayüzü için Vite portunu kullanın.

## API özeti

- Ürün: `GET/POST /products/`, `GET/PUT/DELETE /products/{id}`
- Sipariş: `GET/POST /orders/`, `GET/PUT/DELETE /orders/{id}` — gövdede isteğe bağlı `items: [{ product_sku, quantity, unit_price }]`
- PDF: `GET /orders/{id}/invoice`, `GET /orders/{id}/receipt`
- Pazaryeri: `GET/POST /marketplaces/` vb. (`.env.example` ve `MARKETPLACE_LIVE_HTTP`)

## Yasal not

PDF çıktıları iç operasyon belgesidir; **resmi e-Fatura / e-İrsaliye (GİB)** kapsamında değildir.

## Test

```bash
pytest tests/
```

## Lisans

Eğitim amaçlı. Coded by **Ebulcode** for **Eşsiz Teknik**.
