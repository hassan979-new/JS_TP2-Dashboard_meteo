# JavaScript – Dashboard Météo avec WebSocket

## 📖 Description
Ce projet illustre une application **JavaScript** qui consomme des données météorologiques en temps réel via un **serveur WebSocket**.  
Les données issues d’un fichier CSV sont transmises au client, affichées dans un tableau HTML et représentées graphiquement avec **Chart.js**.

---

## 📂 Structure du projet
```
ProjetMeteo/
├── server.js
├── temp.csv         
└── index.html       
```


---

## ⚙️ Fonctionnalités

### 🌐 Serveur WebSocket (Node.js)
- Utilise le module `ws` pour créer un serveur WebSocket sur le port **5002**.  
- Convertit le fichier `temp.csv` en JSON avec `csvtojson`.  
- Envoie les données ligne par ligne au client toutes les **3 secondes**.  
- Gère la déconnexion du client et arrête l’envoi des données.  

### 🖥️ Interface Client (HTML/JS)
- **Tableau dynamique** affichant les données météo : mois, températures max/min et jours de pluie.  
- **Graphiques interactifs** avec Chart.js :  
  - Courbes des températures max/min.  
  - Histogramme du nombre de jours de pluie.  
- Connexion WebSocket avec gestion des événements (`onopen`, `onmessage`, `onerror`, `onclose`).  
- Mise à jour en temps réel du tableau et des graphiques.  

---

## 🖥️ Exemple d’exécution

https://github.com/user-attachments/assets/b41264b4-e1f8-4719-b0a0-ca67377e5bb1

---

## 💡 Concepts pratiqués
- Communication temps réel avec **WebSocket**.  
- Conversion de données CSV en JSON côté serveur.  
- Manipulation du DOM pour mise à jour dynamique du tableau.  
- Visualisation de données avec **Chart.js** (courbes et histogrammes).  
- Gestion des événements réseau et erreurs côté client.  

---

## 🧑‍💻 Auteur
👤 **Agouram Hassan**  
🌐 Développement JavaScript
🎓 Instructor : **Mr. LACHGAR**  
📅 16 Avril 2026

