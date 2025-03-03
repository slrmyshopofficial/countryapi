# 🌍 Country API - SlrmyApi

**Country API** membolehkan anda mendapatkan maklumat negara berdasarkan kod negara ISO 3166-1 alpha-2 secara langsung dari API.

# 📦 Pemasangan
```javascript
npm install @slrmyapi/countryapi
```
# 📥 Cara Penggunaan
```javascript
const getCountryInfo = require("@slrmyapi/countryapi");

getCountryInfo("MY").then(console.log);
// Output: { name: 'Malaysia', emoji: '🇲🇾', phoneCode: '+60' }

getCountryInfo("XX").then(console.log);
// Output: { error: 'Gagal mendapatkan data dari API.' }
```
# 📌 Negara Yang Disokong

API ini mengambil data secara langsung dari : SlrmyApi

# 👨‍💻 Developer Info

<p align="left">
  <a href="https://github.com/slrmyshopofficial">
    <img src="https://img.shields.io/badge/GitHub-000000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="https://www.npmjs.com/package/@slrmyapi/countryapi">
    <img src="https://img.shields.io/badge/NPM-CB3837?style=for-the-badge&logo=npm&logoColor=white" alt="NPM">
  </a>
  <a href="https://wa.me/601136871190">
    <img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>
  <a href="https://instagram.com/slrmyshopofficial">
    <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram">
  </a>
</p>
