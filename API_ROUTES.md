1. Base URL

Все JSON-файлы находятся по базовому адресу:

https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/

2. Endpoints (полный список)
Districts
https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/districts.json

Government
https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/gov.json

Medical
Аптеки
https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/med_pharmacies.json

Клиники
https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/med_clinics.json

Стоматологи
https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/med_dentists.json

Beauty (Салоны красоты)
https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/beauty.json

Translator (Переводчик)
https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/translator.json

Sport
https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/sport.json

Transfer
https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/transfer.json

Products (AliMind Products)
https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/products.json

Misc (Разное)
https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/misc.json

3. Формат API

Все эндпоинты возвращают массив объектов JSON:

[
  {
    ...object fields...
  }
]

4. Использование в Telegram-боте

Пример загрузки данных:

import requests

URL = "https://raw.githubusercontent.com/olesiaHairstylist/alimind-directory/main/data/gov.json"

data = requests.get(URL).json()
