# Billed App - Fullstack

Application complète de gestion de notes de frais

## 📋 Description

Application SaaS permettant aux employés de soumettre des notes de frais et aux administrateurs RH de les valider.

Ce repository contient l'application complète (frontend + backend) pour une vue d'ensemble du projet.

## 🚀 Structure du projet
```
Billed-App-Fullstack/
├── Billed-app-FR-Front/    # Application frontend (HTML, CSS, JavaScript)
└── Billed-app-FR-Back/     # API backend (Node.js, Express, SQLite)
```

#### Page de connexion
![Login](screenshots/login-page.png)


## 🎯 Travail réalisé

### Bugs corrigés
- **Bug #1** : Tri antichronologique des dates dans Bills.js
- **Bug #2** : Login administrateur (sélecteurs data-testid incorrects)
- **Bug #3** : Validation des formats de fichiers (jpg, jpeg, png uniquement)
- **Bug #4** : Ouverture simultanée de plusieurs listes dans le Dashboard
- **Bonus** : Correction de bugs querySelector avec backticks (Bills.js et NewBill.js)

### Tests ajoutés
- **Tests unitaires NewBill.js** : 5 tests (validation extensions + handleSubmit)
- **Tests d'intégration GET Bills.js** : 3 tests (succès, erreur 404, erreur 500)
- **Tests d'intégration POST NewBill.js** : 3 tests (upload fichier avec gestion erreurs)
- **Couverture globale** : 89.76% (objectif : 80% ✅)
- **Total** : 57 tests qui passent

## 📸 Résultats des tests

#### Tests Jest - 57 tests passent avec succès
![Tests Jest](screenshots/rapport-tests-jest.png)

#### Couverture globale - 89.76%
![Couverture globale](screenshots/rapport-couverture-global.png)



## 🛠️ Installation et lancement

### Prérequis
- Node.js v16 ou v18
- npm

### 1. Cloner le projet
```bash
git clone https://github.com/MTDev2024/Billed-App-Fullstack.git
cd Billed-App-Fullstack
```

### 2. Lancer le backend
```bash
cd Billed-app-FR-Back
npm install
npm run run:dev
```

Le serveur backend démarre sur **http://localhost:5678**

### 3. Lancer le frontend (dans un nouveau terminal)
```bash
cd Billed-app-FR-Front
npm install
npm install -g live-server
live-server
```

L'application frontend s'ouvre sur **http://127.0.0.1:8080/**

## 🧪 Tests

### Lancer tous les tests
```bash
cd Billed-app-FR-Front
npm run test
```

### Voir le rapport de couverture
```bash
npm run test
# Puis ouvrir : http://127.0.0.1:8080/coverage/lcov-report/
```

## 👤 Comptes de test

**Administrateur RH :**
- Email : `admin@test.tld`
- Password : `admin`

**Employé :**
- Email : `employee@test.tld`
- Password : `employee`

## 📚 Technologies utilisées

**Frontend :**
- HTML5, CSS3, JavaScript (ES6+)
- Jest, Testing Library
- Live-server

**Backend :**
- Node.js, Express
- SQLite
- JWT (authentification)

**Outils :**
- Chrome DevTools (debugging)
- ESLint, Prettier
- Git, GitHub

## 🔗 Repository avec historique détaillé

Pour voir l'historique complet des commits (corrections de bugs, ajout progressif des tests) :

👉 **[Billed-App - Frontend avec historique complet](https://github.com/MTDev2024/Billed-App)**

## 📝 Note

Projet réalisé dans le cadre de la formation Développeur d'application React. 