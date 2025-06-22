---
title: Vérifier si une photo est truquée (Photoshop)
tags: [image, retouche, vérification, photo, manipulation]
created: 2025-06-09
---  

# Vérifier si une photo est truquée (Photoshop)  

## 🧠 Résumé rapide  

> Cette fiche regroupe plusieurs techniques manuelles pour détecter d’éventuelles retouches ou falsifications sur une photo, notamment via Photoshop CC 2019 ou équivalent.  

---  

## 📌 Techniques manuelles dans Photoshop CC 2019 (v20.0.0)  

### 🖤 1. Désaturation + Niveaux  

- `Ctrl + Shift + U` pour désaturer (passer en noir et blanc).

- `Ctrl + L` pour ouvrir les **Niveaux** et augmenter les contrastes.

- 📍 Objectif : faire ressortir les zones de texture anormales ou les différences de luminosité dues aux retouches. 

---  

### 🔍 2. Zoom haute résolution (>300%) sur zones critiques  

- Inspecte les **textures de peau** trop lisses ou floues.

- Regarde les **bords** trop nets (effet collage) ou les zones floues incohérentes.

- Cherche des **zones clonées ou répétées**.  

---  

### 🎚️ 3. Calques de réglage "Courbes"  

- `Ctrl + M` pour ouvrir les **Courbes**.

- Accentue le contraste pour mettre en évidence les transitions douteuses.

- Permet de repérer les modifications locales dans la lumière.  

---

### 🔎 4. Filtre "Passe-haut"  

- Duplique le calque.

- Va dans `Filtre > Autres > Passe-haut` (rayon : 3–5 px).

- Change le **mode de fusion** du calque en **Lumière tamisée**.

- 🔍 Objectif : voir les détails et distorsions invisibles à l'œil nu.

---  

### 🗂️ 5. Vérification des métadonnées  

- Menu `Fichier > Informations > Métadonnées`.

- Vérifie s’il y a des traces de sauvegardes successives dans Photoshop.

- Présence de **logiciels d’édition** mentionnés = alerte potentielle.

---

## 🧠 Autres outils gratuits en ligne

- [FotoForensics](https://fotoforensics.com/) — Analyse d’erreur de niveau (ELA).

- [Image Edited?](https://imageedited.com/) — Vérifie les métadonnées et détecte les traces de retouche.

- [Forensically](https://29a.ch/photo-forensics/) — Suite complète d’outils (copie, niveaux, analyse ELA, bruit, etc).

---

## 🔗 Liens connexes

- [[image]]

- [[vérification visuelle]]

---

## 🧭 Navigation / Contexte

📂 Dossier : `03 - Références générales/Images`  

🔍 Vue locale : `Analyse d’images truquées`

---

## 🗒️ Notes personnelles

- Ces méthodes ne garantissent pas la preuve absolue mais aident à lever le doute.

- L’usage combiné de plusieurs techniques augmente la fiabilité de l’analyse.