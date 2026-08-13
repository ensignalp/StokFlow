# StokFlow

Yerel stok, sipariş, PDF fatura/irsaliye ve pazaryeri yapılandırması. FastAPI + React (Vite).

<p align="center">
  <img src="docs/screenshots/001%20-%20Panel.png" alt="StokFlow Panel" width="100%">
</p>

## Özellikler

- **Stok:** Ürün CRUD, kritik eşik
- **Sipariş:** Oluşturma, durum, kalemler, PDF fatura ve irsaliye
- **Pazaryeri:** Trendyol / Hepsiburada / N11 anahtarları (Fernet ile şifreli) ve simülasyon veya canlı HTTP
- **API:** FastAPI `/docs`

## Ekran Görüntüleri

- [Panel](#panel)
- [Finans ve Analiz](#finans-ve-analiz)
- [Ürünler](#ürünler)
- [Siparişler](#siparişler)
- [Entegrasyon](#entegrasyon)
- [Kampanyalar](#kampanyalar)
- [Yorumlar](#yorumlar)
- [Paketler](#paketler)
- [Profil](#profil)

### Panel

Satış performansı, kanal dağılımı, akıllı stok tahmini, en çok satanlar ve canlı sipariş akışı.

<img src="docs/screenshots/001%20-%20Panel.png" alt="Panel" width="100%">

### Finans ve Analiz

Portföy, kasa, kâr/zarar, risk, hak ediş ve pazaryeri metrikleri.

#### Portföy ve Nakit Kasa

<img src="docs/screenshots/002%20-%20Finans%20ve%20Analiz%20-%20Portfoy%20ve%20Nakit%20Kasa.png" alt="Portföy ve Nakit Kasa" width="100%">

#### Kâr / Zarar ve Ciro

<img src="docs/screenshots/003%20-%20Finans%20ve%20Analiz%20-%20Kar%20Zarar%20ve%20Ciro.png" alt="Kâr Zarar ve Ciro" width="100%">

#### Risk ve İade Analizi

<img src="docs/screenshots/004%20-%20Finans%20ve%20Analiz%20-%20Risk%20ve%20Iade%20Analizi.png" alt="Risk ve İade Analizi" width="100%">

#### Hak Ediş ve Transferler

<img src="docs/screenshots/005%20-%20Finans%20ve%20Analiz%20-%20Hak%20Edis%20ve%20Transferler.png" alt="Hak Ediş ve Transferler" width="100%">

#### Pazaryeri Metrikleri

<img src="docs/screenshots/006%20-%20Finans%20ve%20Analiz%20-%20Pazaryeri%20Metrikleri.png" alt="Pazaryeri Metrikleri" width="100%">

#### Mağaza Vadeleri

<img src="docs/screenshots/007%20-%20Finans%20ve%20Analiz%20-%20Magaza%20Vadeleri.png" alt="Mağaza Vadeleri" width="100%">

#### Finansal Raporlar

<img src="docs/screenshots/008%20-%20Finans%20ve%20Analiz%20-%20Finansal%20Raporlar.png" alt="Finansal Raporlar" width="100%">

### Ürünler

Liste ve kart görünümü, XML katalog aktarımı ve yeni ürün sihirbazı.

#### Liste Görünümü

<img src="docs/screenshots/009%20-%20Urunler%20-%20Liste%20Gorunumu.png" alt="Ürünler — Liste Görünümü" width="100%">

#### Kart Görünümü

<img src="docs/screenshots/010%20-%20Urunler%20-%20Kart%20Gorunumu.png" alt="Ürünler — Kart Görünümü" width="100%">

#### XML Katalog — Dosya Yükle

<img src="docs/screenshots/013%20-%20Urunler%20-%20XML%20Katalog%20Dosya%20Yukle.png" alt="XML Katalog — Dosya Yükle" width="100%">

#### XML Katalog — URL ile Aktar

<img src="docs/screenshots/014%20-%20Urunler%20-%20XML%20Katalog%20URL%20ile%20Aktar.png" alt="XML Katalog — URL ile Aktar" width="100%">

#### XML Katalog — Canlı Çıktı

<img src="docs/screenshots/017%20-%20Urunler%20-%20XML%20Katalog%20Canli%20Cikti.png" alt="XML Katalog — Canlı Çıktı" width="100%">

#### Yeni Ürün — Genel ve Medya

<img src="docs/screenshots/018%20-%20Urunler%20-%20Yeni%20Urun%20Genel%20ve%20Medya.png" alt="Yeni Ürün — Genel ve Medya" width="100%">

#### Yeni Ürün — Fiyat ve Stok

<img src="docs/screenshots/019%20-%20Urunler%20-%20Yeni%20Urun%20Fiyat%20ve%20Stok.png" alt="Yeni Ürün — Fiyat ve Stok" width="100%">

#### Yeni Ürün — Varyantlar

<img src="docs/screenshots/020%20-%20Urunler%20-%20Yeni%20Urun%20Varyantlar.png" alt="Yeni Ürün — Varyantlar" width="100%">

#### Yeni Ürün — SEO ve Pazaryeri

<img src="docs/screenshots/021%20-%20Urunler%20-%20Yeni%20Urun%20SEO%20ve%20Pazaryeri.png" alt="Yeni Ürün — SEO ve Pazaryeri" width="100%">

### Siparişler

Sipariş KPI’ları, durum filtresi ve sipariş yönetimi.
ensignalp/StokFlow
<img src="docs/screenshots/022%20-%20Siparisler.png" alt="Siparişler" width="100%">

### Entegrasyon

Pazaryeri bağlantıları, ping matrisi, XML içe/dışa aktarma.

<img src="docs/screenshots/023%20-%20Entegrasyon.png" alt="Entegrasyon" width="100%">

#### Trendyol Bağlantısı

<img src="docs/screenshots/024%20-%20Entegrasyon%20-%20Trendyol%20Baglantisi.png" alt="Entegrasyon — Trendyol Bağlantısı" width="100%">

### Kampanyalar

İndirim kuponu oluşturma ve tanımlı kupon listesi.

<img src="docs/screenshots/025%20-%20Kampanyalar.png" alt="Kampanyalar" width="100%">

### Yorumlar

Pazaryeri yorumları, AI yanıtı ve manuel yanıt.

<img src="docs/screenshots/026%20-%20Yorumlar.png" alt="Yorumlar" width="100%">

#### Manuel Yanıt

<img src="docs/screenshots/027%20-%20Yorumlar%20-%20Manuel%20Yanit.png" alt="Yorumlar — Manuel Yanıt" width="100%">

### Paketler

Aylık ve yıllık ödeme planları.

#### Aylık Ödeme

<img src="docs/screenshots/029%20-%20Paketler%20-%20Aylik%20Odeme.png" alt="Paketler — Aylık Ödeme" width="100%">

#### Yıllık Ödeme

<img src="docs/screenshots/030%20-%20Paketler%20-%20Yillik%20Odeme.png" alt="Paketler — Yıllık Ödeme" width="100%">

### Profil

Mağaza hesabı ve profil ayarları.

<img src="docs/screenshots/033%20-%20Profil%20-%20Magaza%20Hesabi.png" alt="Profil — Mağaza Hesabı" width="100%">

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

Eğitim amaçlı. Coded by **Ensignalp**
