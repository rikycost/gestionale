GESTIONALE ONLINE + MOBILE

File principale: app.py

Cosa è stato cambiato:
- UI responsive per telefono e tablet
- menu mobile a scomparsa
- tabelle trasformate in schede su schermi piccoli
- agenda leggibile da telefono
- configurazione database pronta per PostgreSQL online tramite DATABASE_URL
- SQLite resta come fallback per uso locale
- predisposizione PWA: puoi aggiungerlo alla schermata Home del telefono

Per avvio locale:
1. pip install -r requirements.txt
2. python app.py
3. apri http://localhost:5000

Credenziali iniziali:
username: admin
password: admin123

Per Render:
- carica questi file in una repository GitHub
- crea un nuovo Web Service collegato alla repository
- aggiungi PostgreSQL gratuito oppure usa render.yaml come Blueprint
- Render imposterà DATABASE_URL e SECRET_KEY
- comando start: gunicorn app:app

Nota importante:
Il database è online con PostgreSQL, ma i file caricati nella cartella uploads possono non essere permanenti su hosting gratuiti senza disco persistente. Per allegati e foto professionali conviene poi collegare uno storage esterno o un disco persistente.
