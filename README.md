# Minden ami Szeged – MVP

## 🎯 Projekt célja
A **Minden ami Szeged** egy közösségi városi alkalmazás, amely független a globális közösségi médiától, és a szegedieknek kínál egy **helyi, interaktív platformot**.  
Az alkalmazás célja: hírek, közösségi posztok, események, kuponok és hibabejelentések egyetlen appban.

---

## ⚙️ Technológiai stack
- **Mobil alkalmazás:** Flutter (Android + iOS)
- **Backend API:** Laravel (PHP 8.x) vagy Node.js (Express)
- **Adatbázis:** PostgreSQL / MySQL
- **Autentikáció:** JWT token
- **Push értesítések:** Firebase Cloud Messaging
- **Térkép integráció:** Google Maps API

---

## 📂 Projekt struktúra
```plaintext
minden-ami-szeged/
│
├── backend/                  # REST API és adatbázis logika
│   ├── src/
│   │   ├── controllers/       # CRUD vezérlők (users, posts, coupons)
│   │   ├── models/            # DB modellek
│   │   ├── routes/            # API végpontok
│   │   └── services/          # kupon logika, értesítések
│   ├── tests/                 # unit/integration tesztek
│   └── .env.example           # környezeti változók
│
├── mobile-app/               # Flutter kliens
│   ├── lib/
│   │   ├── screens/           # képernyők (Feed, Groups, Coupons, Map)
│   │   ├── widgets/           # UI komponensek
│   │   ├── services/          # API hívások
│   │   └── providers/         # state management (Provider/Bloc)
│   └── pubspec.yaml           # Flutter csomagok
│
├── docs/                     # Dokumentáció
│   ├── database-schema.sql    # DB séma
│   ├── api-spec.yaml          # OpenAPI/Swagger specifikáció
│   └── roadmap.md             # Fejlesztési ütemterv
│
└── README.md                 # Projekt leírása
