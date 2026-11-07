# Site-139 SCP RP — Launcher © Clem'Studio

## 1. API (sur ton VPS / PC serveur) — Node 18+
cd server && npm install
JWT_SECRET="un-long-secret" node index.js     (port 3000)
Devenir owner (après avoir créé ton compte) :
sqlite3 data.db "update users set rank='owner' where username='TonPseudo';"

## 2. Launcher -> .exe (sur ton PC Windows) — Node 18+
1. Édite launcher/config.json : mets l'URL de ton API.
2. Mets ton logo : launcher/logo.png (https://postimg.cc/7Cxs8T5R -> télécharge l'image) et pour l'icône de l'.exe, launcher/build/icon.ico
3. cd launcher && npm install && npm run build
4. Ton installeur : launcher/dist/Site-139 SCP RP Setup 1.0.0.exe

## 3. Premier réglage (menu ADMIN, compte owner)
- IP du serveur, URL de l'installeur Forge 1.20.1 (.jar), mods (nom, URL .jar, nom de fichier).

## Sans rien installer : compiler avec GitHub
1. Crée un dépôt GitHub (privé) et envoie-y tout le contenu de ce dossier (y compris .github).
2. Onglet "Actions" -> "Build Launcher EXE" -> attends ~3 min.
3. Clique sur le run terminé -> télécharge "Site-139-Launcher-EXE" -> ton .exe est dedans.
