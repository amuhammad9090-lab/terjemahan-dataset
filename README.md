# Terjemahan Dataset - Kemenag

Dataset terjemahan Al-Qur'an Bahasa Indonesia dari Kementerian Agama RI.

## Format
```json
{
  "1": {
    "1": "Dengan nama Allah Yang Maha Pengasih lagi Maha Penyayang.",
    "2": "Segala puji bagi Allah, Tuhan semesta alam",
    ...
  },
  ...
}
```

## Usage
```python
import json
import requests

url = "https://raw.githubusercontent.com/amuhammad9090-lab/terjemahan-dataset/main/terjemahan_kemenag.json"
response = requests.get(url)
terjemahan = response.json()

# Get specific ayat
print(terjemahan["1"]["1"])  # Al-Fatihah ayat 1
```

## Stats

- **Total Surah:** 114
- **Total Ayat:** 6,236
- **Format:** JSON
- **Encoding:** UTF-8
