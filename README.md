# Minified Dosyalar Hakkında

Bu klasörde, erişilebilirlik ve sesli komut desteği sağlayan voice-access projesinin minify (küçültülmüş) JavaScript ve CSS dosyaları bulunmaktadır.

## Dosyalar
- `voice-access.min.js`: Sesli komut ve erişilebilirlik özelliklerini sağlayan minify edilmiş JavaScript dosyası.
- `voice-access.min.css`: Mikrofon butonu ve animasyonları için minify edilmiş CSS dosyası.

## Kullanım
Bu dosyaları CDN üzerinden doğrudan projenize ekleyebilirsiniz:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/ercanvas/voice-access-turkish@main/voice-access.min.css" />
<script src="https://cdn.jsdelivr.net/gh/ercanvas/voice-access-turkish@main/voice-access.min.js"></script>
```

Buton eklemek için:
```html
<button id="micBtn" aria-label="Mikrofon tuşu">
  <i class="bi bi-mic-fill"></i>
  <span class="pulse"></span>
</button>
```

Komutları özelleştirmek için, script'ten önce şunu ekleyebilirsiniz:
```html
<script>
window.voiceCommands = {
  "profil": "/profil",
  "hakkımda": "/hakkimda",
  "anasayfa": "/"
};
</script>
```

Daha fazla bilgi için ana README dosyasına bakınız.
