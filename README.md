# FlyRadar
FlyRadar
import os
import requests

token = os.environ["TELEGRAM_BOT_TOKEN"]
chat_id = os.environ["TELEGRAM_CHAT_ID"]

url = f"https://api.telegram.org/bot{token}/sendMessage"

data = {
    "chat_id": chat_id,
    "text": "🎉 測試成功！\n\n你的機票雷達已經可以發送 Telegram 通知了 ✈️"
}

response = requests.post(url, json=data)

print(response.status_

print(response.text)