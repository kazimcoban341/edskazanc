# EDS Kazanç Dashboard

Tek dosyalık statik dashboard. Netlify üzerinde yayınlamak için build komutu gerekmez.

## Netlify Ayarları

- Build command: boş bırakın
- Publish directory: `.`
- Ana dosya: `index.html`

## Yerelde çalıştırma

```powershell
python -m http.server 8000 --bind 127.0.0.1
```

Ardından `http://127.0.0.1:8000` adresini açın.

## Veri güncelleme

Aylık veriler `index.html` içindeki `rawData` tablosunda (sekmeyle ayrılmış) tutulur. Yeni ay için tabloya bir satır ekleyin; KPI kartları, grafikler ve dışa aktarımlar bu tablodan üretilir. Panoda ve pano özetinde görünen "Son güncelleme" tarihi için aynı dosyadaki `DATA_UPDATED` sabitini de güncelleyin.
