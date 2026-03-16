# UTB Learn — Documentation

Documentation technique et fonctionnelle de la plateforme e-learning interne de l'**Union Togolaise de Banque (UTB)**.

Construite avec [Mintlify](https://mintlify.com).

---

## Structure

```
docs/
├── intro/          → Présentation, stack, architecture, installation
├── mobile/         → Application Android (React Native / Expo)
│   ├── modules/
│   ├── formations/
│   ├── quiz/
│   ├── offline/
│   ├── profil/
│   └── build/
├── admin/          → Dashboard administration (Nuxt 4)
│   ├── dashboard/
│   ├── agents/
│   ├── modules/
│   ├── quiz/
│   ├── categories/
│   ├── directions/
│   ├── departements/
│   └── logs/
├── infra/          → Supabase, Storage, Edge Functions, Vercel
└── guides/         → Guides opérationnels
```

---

## Lancer en local

```bash
npm install -g mintlify
mintlify dev
```

Ouvre [http://localhost:3000](http://localhost:3000).

---

## Déploiement

La documentation est déployée automatiquement via **Mintlify Cloud** à chaque push sur `main`.

---

## Stack documentée

| Interface | Technologies |
|-----------|-------------|
| Application mobile | React Native, Expo SDK 54, Expo Router, Supabase JS |
| Dashboard admin | Nuxt 4, Nuxt UI v3, TipTap 3, Supabase JS |
| Backend & BDD | Supabase (PostgreSQL, Storage, Auth, Edge Functions) |
| Hosting | Vercel (dashboard), EAS Build (APK Android) |

---

## Contenu

- **61 pages** couvrant l'intégralité du projet
- Schémas d'architecture et de BDD
- Guides opérationnels (déploiement, upload vidéo, APK, logs)
- Documentation des endpoints API et Edge Functions
- Variables d'environnement dev et production