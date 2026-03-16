<div align="center">

# 📈 CoinWtch

**Compare Bitcoin prices across multiple exchanges in real-time**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Axios](https://img.shields.io/badge/Axios-5A29E4?style=flat-square&logo=axios&logoColor=white)

</div>

---

## 📖 About

CoinWtch is a cryptocurrency price comparison tool that fetches live Bitcoin exchange rates from multiple providers and displays them side-by-side. Enter a USD amount and instantly see how much BTC you'd get from each exchange, helping you find the best rate.

## ✨ Features

- **Multi-provider comparison** — fetches rates from multiple crypto exchanges simultaneously
- **Live price updates** — real-time BTC/USD rates with debounced API calls
- **Custom amount input** — enter any USD amount to compare conversions
- **Sorted results** — providers ranked by best exchange rate
- **Loading skeletons** — smooth UX with skeleton placeholders during data fetch
- **Backend caching** — AirCode serverless backend caches rates to reduce API calls
- **Responsive design** — Tailwind CSS for mobile-first layout

## 🏗️ Architecture

```
CoinWtch/
├── src/
│   ├── App.tsx              # Main app — state management, API calls
│   ├── AmountInput.tsx      # USD amount input with debounce
│   ├── ResultRow.tsx        # Individual provider result display
│   ├── LoadingSkeleton.tsx  # Skeleton loading placeholders
│   └── main.tsx             # React entry point
├── backend/
│   ├── providers.ts         # Exchange API integrations
│   └── cache.ts             # Rate caching logic
├── tailwind.config.js
└── vite.config.ts
```

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React 18, TypeScript, Tailwind CSS |
| Build | Vite |
| HTTP | Axios with debounced requests |
| Backend | AirCode serverless functions |
| Utilities | Lodash (sortBy), use-debounced-effect |

## 🚀 Getting Started

```bash
git clone https://github.com/Emrebym/CoinWtch.git
cd CoinWtch
npm install
npm run dev
```

The app will be available at `http://localhost:5173`

## 📝 License

MIT
