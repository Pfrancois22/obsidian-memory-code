

recherche pour savoir si une photo est truqué

Dans **Photoshop 20.0.0 (version CC 2019)**, la fonction **"Détecter les manipulations"** (_"Content-Aware Fill" avancé ou outils forensiques_) n'existait pas encore sous forme automatisée. Adobe a introduit des améliorations dans les versions ultérieures (notamment avec l'IA **"Adobe Sensei"**).

### **Comment vérifier les retouches manuellement dans Photoshop 20.0.0 ?**

Même sans outil dédié, tu peux utiliser ces techniques :

#### **1. Utilise l’outil "Désaturation" (Ctrl+Shift+U) + Niveaux (Ctrl+L)**

- Passe l’image en noir et blanc, puis joue sur les niveaux pour faire ressortir les zones suspectes (retouches créent souvent des différences de luminosité).
    

#### **2. Zoom haute résolution (300%+) sur les zones critiques**

- **Peau** : Cherche des textures trop lisses ou répétitives (signe de _clone stamp_ ou _patch tool_).
    
- **Contours** : Les bords trop nets (comme un collage) ou des flous incohérents.
    

#### **3. Calques de réglage "Courbes" (Ctrl+M)**

- Augmente le contraste pour voir les transitions suspectes entre les zones modifiées et non modifiées.
    

#### **4. Filtre "Passe-haut"**

- Duplique le calque → **Filtre > Autres > Passe-haut** (rayon 3-5 px).
    
- Changez le mode de fusion en **"Lumière tamisée"** pour voir les distortions.
    

#### **5. Vérifiez les métadonnées**

- **Fichier > Informations > Métadonnées** : Si l’image a été sauvegardée plusieurs fois dans Photoshop, c’est un indice.