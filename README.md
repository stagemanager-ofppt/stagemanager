# StageManager

Application web de gestion des stages et des stagiaires.

## 📋 Description

StageManager remplace les fichiers Excel du service des stages 
par une application web unique : centralisation des étudiants, 
entreprises, demandes, stages, conventions et suivis.

**Projet pédagogique** - OFPPT 2026  
**Filière** : Développement Digital - Option Web Full-Stack

## 🛠️ Stack technique

| Couche | Technologie |
|--------|-------------|
| Frontend | React 18 + Vite |
| Routing | React Router 6 |
| HTTP | Axios |
| Graphiques | Recharts |
| Backend | Node.js 20 + Express |
| Base de données | MySQL 8 |
| Auth | JWT + bcrypt + cookie httpOnly |

## 📦 Installation

### Prérequis
- Node.js 20 LTS
- MySQL 8
- Git

### 1. Cloner le repo
\`\`\`bash
git clone https://github.com/stagemanager-ofppt/stagemanager.git
cd stagemanager
\`\`\`

### 2. Base de données
\`\`\`bash
mysql -u root -p < server/database/schema.sql
mysql -u root -p stagemanager < server/database/indexes.sql
mysql -u root -p stagemanager < server/database/seed.sql
\`\`\`

### 3. Serveur (backend)
\`\`\`bash
cd server
cp .env.example .env
npm install
npm run seed
npm run dev
\`\`\`

### 4. Client (frontend)
\`\`\`bash
cd client
npm install
npm run dev
\`\`\`

## 🔑 Comptes de démonstration

| Rôle | Email | Mot de passe |
|------|-------|--------------|
| Admin | admin@stagemanager.ma | Stage2027 |

## 📁 Structure du projet

\`\`\`
stagemanager/
├── client/          # React (frontend)
├── server/          # Node.js + Express (backend)
│   └── src/
│       ├── config/
│       ├── routes/
│       ├── controllers/
│       ├── services/
│       ├── repositories/
│       ├── validators/
│       ├── middlewares/
│       └── utils/
├── docs/            # Documentation
└── README.md
\`\`\`

## 👥 Auteurs

- **Hajar Bahhari** - Développeuse
- **Ihssan Elaidi** - Développeuse



