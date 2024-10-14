# 🤖 CrowBot - Un Bot Discord pour Render

Bienvenue dans le dépôt de **CrowBot**, un bot Discord simple conçu pour être hébergé sur [Render](https://render.com/) et maintenir sa connexion active grâce à [UptimeRobot](https://uptimerobot.com/).

## 🚀 Fonctionnalités

- ✨ **Hébergement facile** sur Render
- 🔄 **Keep-alive automatique** avec un script `keepalive.js`
- 🛠️ Nécessite seulement une configuration minimale

## ⚙️ Prérequis

Avant de démarrer, assure-toi d'avoir :

- Un compte [Render](https://render.com/) pour héberger ton bot
- Un compte [UptimeRobot](https://uptimerobot.com/) pour maintenir le bot en ligne
- Le **token** de ton bot Discord

## 📦 Installation

### 1. Cloner ce dépôt

```bash
git clone https://github.com/xDatabaseDev/Crowbot
cd ton-repo
```

### 2. Configuration de Render

1. Crée un nouveau service sur [Render](https://dashboard.render.com/).
2. Sélectionne **Web Service** et choisis ton dépôt GitHub.
3. Dans la section **Environment Variables**, ajoute la variable suivante :

   - `DISCORD_TOKEN` : Le token de ton bot Discord.

4. Règle le **Start Command** sur `node index.js` (ou ton fichier principal).



### 3. UptimeRobot

1. Crée un compte gratuit sur [UptimeRobot](https://uptimerobot.com/).
2. Ajoute une nouvelle **HTTP Monitor** avec l'URL de ton service Render (par exemple, `https://ton-service.onrender.com/`).
3. UptimeRobot vérifiera régulièrement cette URL pour maintenir ton bot en ligne.

## 🚀 Lancement du Bot

Si tout est correctement configuré, Render va démarrer ton bot automatiquement. Sinon, tu peux manuellement lancer le bot avec :

```bash
node index.js
```

## 🛠️ Technologies Utilisées

- [Discord.js](https://discord.js.org/) - Framework pour les bots Discord
- [Node.js](https://nodejs.org/) - Runtime JavaScript
- [Express](https://expressjs.com/) - Serveur minimaliste pour le keep-alive

## 🎯 Contribuer

Les contributions sont les bienvenues ! Ouvre une pull request ou signale un problème.

## 📝 Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE](./LICENSE) pour plus d'informations.

---

### 🤖 Garde ton bot en ligne et amuse-toi bien !

---

Avec ce README, les utilisateurs pourront facilement suivre les étapes pour configurer et héberger le bot sur Render et utiliser UptimeRobot pour maintenir le bot actif. 😊
