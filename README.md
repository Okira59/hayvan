# Hayvan — Edirne Ticaret Borsası canlı hayvan fiyatları

`Okira59/Pyhton` deposundaki `hayvan/` klasöründen (commit geçmişiyle birlikte) taşındı.

`fiyat.py`, Edirne Ticaret Borsası'nın açık API'sinden (canlı hayvan salonu) son işlem fiyatlarını çeker
(Kuzu, Süt Kuzusu, Koyun, Toklu … — en az / en çok / ortalama TL/kg ve satılan baş sayısı) ve
fiyat geçmişine ekler. Bu veriyi "Sürü Takip" paneli (Borsa / Yem Maliyeti sekmeleri) kullanır.

## Kurulum
```bash
pip install -r requirements.txt
```

## Çalıştırma
```bash
python fiyat.py      # -> docs/data/fiyat.json
```

## Otomatik çalışma ve panel
- `.github/workflows/hayvan.yml` her 30 dakikada tetiklenir, 2 saatte bir gerçekten çalışır (elle: Actions → "Hayvan Borsa Fiyatlari" → Run workflow).
- "Sürü Takip" paneli (GitHub Pages, `main` dalı `/docs`): https://okira59.github.io/hayvan/ — sürü kayıtları tarayıcıda (localStorage) tutulur.
- Android uygulaması: `docs/SuruTakip.apk`.
