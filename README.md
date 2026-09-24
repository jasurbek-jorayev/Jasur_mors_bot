# Mors Bot

Mors (meva ichimligi) sotuvchisi uchun **kunlik savdo hisobi** Telegram boti. Real kichik biznes ehtiyoji uchun yozilgan.

## Imkoniyatlar

- Mahsulot turini tanlash: katta stakan, kichik stakan, 1 L, 1.5 L, 5 L
- Sotilgan miqdorni kiritish
- Kunni yakunlash: kunlik jami savdo
- Hisobot: sotuvlar tarixi

## Texnologiyalar

- **Python 3**, **aiogram 3**
- **SQLite** + **aiosqlite** (jadvallar: `sales`, `user_settings`)
- **aiohttp** - ichki veb-server va self-ping (bepul hostingda bot uxlab qolmasligi uchun)
- **Docker**

## Ishga tushirish

~~~bash
pip install -r requirements.txt
cp .env.example .env
python bot.py
~~~

Docker orqali:

~~~bash
docker build -t mors-bot .
docker run -e BOT_TOKEN=... mors-bot
~~~