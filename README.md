# 🌍 Country API - SlrmyApi

**Country API** ini membolehkan anda mendapatkan maklumat negara berdasarkan kod negara ISO 3166-1 alpha-2.
## 📌 Endpoint
https://slrmyshop.us/country.php?code={ISO_CODE}
## Parameter
| Parameter | Wajib? | Jenis  | Keterangan |
|-----------|--------|--------|------------|
| `code`    | ✅     | string | Kod negara (2 huruf, huruf besar) |

---

## 📥 Cara Integrasi

```javascript
1️⃣ Gunakan Fetch API (JavaScript)

const countryCode = "MY"; // Contoh kod negara Malaysia

fetch(`https://slrmyshop.us/country.php?code=${countryCode}`)
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => console.error("Error:", error));

---
```php
2️⃣ Gunakan cURL (PHP)

$code = "MY"; // Contoh kod negara Malaysia
$url = "https://slrmyshop.us/country.php?code=" . $code;

$ch = curl_init();
curl_setopt($ch, CURLOPT_URL, $url);
curl_setopt($ch, CURLOPT_RETURNTRANSFER, true);
$response = curl_exec($ch);
curl_close($ch);

$data = json_decode($response, true);
print_r($data);
---
3️⃣ Gunakan Axios (Node.js)

const axios = require("axios");

const countryCode = "MY"; // Contoh kod negara Malaysia
axios.get(`https://slrmyshop.us/country.php?code=${countryCode}`)
    .then(response => console.log(response.data))
    .catch(error => console.error("Error:", error));
---

📌 Contoh Output JSON
# Jika kod negara betul (MY untuk Malaysia) :
{
  "name": "Malaysia",
  "emoji": "🇲🇾",
  "phoneCode": "+60",
  "devInfo": {
    "GitHub": "https://github.com/slrmyshop",
    "NPM": "@slrmybot/countryapi",
    "WhatsApp": "+601136871190",
    "Instagram": "@slrmyshopofficial"
  }
}

# Jika kod negara tidak sah (XX) :
{
  "name": "Tidak Diketahui",
  "emoji": "❓",
  "phoneCode": "N/A",
  "devInfo": {
    "GitHub": "https://github.com/slrmyshop",
    "NPM": "@slrmybot/countryapi",
    "WhatsApp": "+601136871190",
    "Instagram": "@slrmyshopofficial"
  }
}


# Jika tiada kod diberikan :
{
  "error": "Sila masukkan kod negara.",
  "devInfo": {
    "GitHub": "https://github.com/slrmyshop",
    "NPM": "@slrmybot/countryapi",
    "WhatsApp": "+601136871190",
    "Instagram": "@slrmyshopofficial"
  }
}


---

👨‍💻 Developer Info

<p align="center">
  <a href="https://github.com/slrmyshop">
    <img src="https://img.shields.io/badge/GitHub-000000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="https://www.npmjs.com/package/@slrmybot/countryapi">
    <img src="https://img.shields.io/badge/NPM-CB3837?style=for-the-badge&logo=npm&logoColor=white" alt="NPM">
  </a>
  <a href="https://wa.me/601136871190">
    <img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>
  <a href="https://instagram.com/slrmyshopofficial">
    <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram">
  </a>


💡 Jangan lupa untuk ⭐ repo ini jika anda suka!
