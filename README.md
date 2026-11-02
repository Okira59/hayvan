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
python fiyat.py
```

> Not: Çıktı `../docs/hayvan/data/fiyat.json` dosyasına yazılır (eski depo düzeni: panel `Okira59/Pyhton/docs/hayvan/`).
