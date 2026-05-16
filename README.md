# LAB 11 — GPS & Google Maps 🗺️

> Programmation Mobile Android — Java  
> ENSA · ma.ensa.localisation

---

## 🎬 Démo vidéo

<!-- Ajoute le lien de ta vidéo ici -->
▶️ [Voir la démonstration](https://youtu.be/vyw5hEDopj4?si=46GceqChVt4_FWfr)

---

## 📋 Description

Application Android qui affiche une carte Google Maps et suit la position GPS de l'utilisateur en temps réel.

---

## ✅ Fonctionnalités

- Affichage d'une carte Google Maps interactive
- Demande de permission de localisation au runtime
- Suivi de la position en temps réel (NETWORK_PROVIDER)
- Marker unique qui se déplace avec l'utilisateur
- Zoom automatique sur la position (niveau 15)
- Dialog d'alerte si le GPS est désactivé

---

## 🛠️ Technologies

- Java · Android SDK
- Google Maps SDK for Android
- LocationManager / LocationListener
- Runtime Permissions (Android 6+)

---

## ⚙️ Installation

1. Clone le projet :
```bash
git clone https://github.com/TON_USERNAME/TON_REPO.git
```

2. Génère ta propre clé API sur [Google Cloud Console](https://console.cloud.google.com) en activant **Maps SDK for Android**

3. Dans `res/values/google_maps_api.xml`, remplace :
```xml
<string name="google_maps_key" translatable="false">YOUR_API_KEY_HERE</string>
```
par ta clé API.

4. Lance l'application sur un émulateur ou appareil réel.

---

## 📁 Structure du projet

```
app/
├── manifests/
│   └── AndroidManifest.xml        # Permissions + clé API
├── java/ma.ensa.localisation/
│   └── MainActivity.java          # Logique principale
└── res/
    ├── layout/activity_main.xml   # Fragment carte
    └── values/google_maps_api.xml # Clé API (non pushée)
```

---

## 👩‍💻 Auteur

FATIMAEZZAHRA ENNASSIRI · ENSA
