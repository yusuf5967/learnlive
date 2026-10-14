# Learn&Live

Erasmus / yüksek lisans öğrencileri için dil hazırlık programının sohbet + aday toplama sistemi.

## Kurulum
```
python -m venv venv
venv\Scripts\activate          # Mac/Linux: source venv/bin/activate
pip install -r gereksinimler.txt
```
`.env` dosyasına `GROQ_API_KEY=gsk_...` ekleyin (anahtar yoksa sistem demo modunda çalışır).

## Çalıştırma
`python baslat.py` → http://localhost:5000  |  /panel  |  /saglik-durumu

## Render
Build: `pip install -r gereksinimler.txt` · Start: `gunicorn baslat:uygulama`
Ortam değişkenleri: FLASK_ORTAMI=uretim, GROQ_API_KEY, CORS_ALLOWED_ORIGINS=<site adresiniz>
