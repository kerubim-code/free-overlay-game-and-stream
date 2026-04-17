# 🖼 OverlayApp

**OverlayApp** est un outil Windows léger développé en **C++ / Qt6** permettant de superposer des images et des GIFs animés par-dessus n'importe quelle application — jeux, streams, présentations — avec un contrôle total sur la position, la taille et l'opacité de chaque élément.

---
# how to use 
## 1) extract the zip w 7zip
## 2) start the .exe 
## 3) enjoy
## discord for any help : ke8u
## or
## https://discord.gg/kBbzb6QYPp


# ✨ Fonctionnalités

- 🖼 **Import d'images** — PNG, JPG, BMP, WEBP, affichées à leur taille originale
- 🎞 **Import de GIFs animés** — lecture en boucle en temps réel
- 🖱 **Déplacement & redimensionnement** — glisser-déposer et poignées de coins directement sur l'overlay
- 🔒 **Mode Lock** — bloque tous les éléments pour éviter les déplacements accidentels en pleine partie
- 👁 **Afficher / Masquer** — raccourci clavier configurable (F1 à F4)
- 🖥 **Click-Through** — l'overlay devient totalement transparent aux clics souris
- 🎯 **Positionnement rapide** — plein écran, centrer, coins haut-gauche / haut-droite / bas-gauche / bas-droite
- 💾 **Configurations nommées** — sauvegarde et charge plusieurs configs JSON dans le dossier Documents
- 🗂 **Icône dans le tray** — l'app tourne en arrière-plan, accessible depuis la barre des tâches
- 📐 **Résolutions multiples** — 1280×720, 1440×1080, 1920×1080, 2560×1440

---

## 🛠 Stack technique

| | |
|---|---|
| Langage | C++17 |
| Framework | Qt 6 (Widgets) |
| Build | CMake 3.16+ |
| Compilateur | MinGW 64-bit |
| OS cible | Windows 10/11 |

---

## 🚀 Compilation

### Prérequis
- [Qt 6.11+](https://www.qt.io/download) avec le module **Widgets** et **MinGW 64-bit**
- CMake 3.16+

### Build
```bash
git clone https://github.com/TON_USER/OverlayApp.git
cd OverlayApp
cmake -B build -S .
cmake --build build
```

### Déploiement (DLL)
Depuis le terminal Qt MinGW :
```bash
windeployqt OverlayApp.exe
```

Ou utilise [Enigma Virtual Box](https://enigmaprotector.com/en/aboutvb.html) pour packager en un seul `.exe` portable.

---

## 📁 Structure du projet

```
OverlayApp/
├── main.cpp
├── mainwindow.cpp / .h      # Panneau de contrôle principal
├── overlaywindow.cpp / .h   # Fenêtre overlay transparente
├── overlaymanager.cpp / .h  # Gestion des items + save/load JSON
├── overlayitem.h            # Structure d'un élément (image ou GIF)
├── canvas.cpp / .h          # Widget canvas
├── app.qrc                  # Ressources (icônes)
└── CMakeLists.txt
```

---

## 📋 Utilisation

1. Lance `OverlayApp.exe`
2. Clique **🖼 Image** ou **🎞 GIF** pour ajouter un élément
3. Positionne et redimensionne directement sur l'écran
4. Utilise les boutons de **positionnement rapide** pour centrer ou mettre en coin
5. Active le **mode Lock** avant de jouer pour figer tous les éléments
6. **💾 Sauvegarder** pour enregistrer ta configuration sous un nom personnalisé
7. **📂 Charger** pour rappeler une configuration sauvegardée

---

## 📄 Licence

MIT — libre d'utilisation, modification et distribution.
