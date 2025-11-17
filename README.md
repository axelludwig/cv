# JSON Resume – Mini Projet

Ce projet utilise le format **JSON Resume** pour générer un CV moderne et entièrement personnalisable.  
Le thème utilisé est **elegant**, un thème populaire et esthétique compatible avec l’écosystème JSON Resume.

---

## 📦 Installation

1. Assure-toi d’avoir **Node.js** installé.
2. Installe l’outil CLI officiel de JSON Resume :

```bash
npm install -g resume-cli
```

3. Installe le thème **jsonresume-theme-elegant** :

```bash
npm install -g jsonresume-theme-elegant
```

---

## 📝 Éditer le CV

Le fichier principal du projet est :

```
resume.json
```

C’est ici que tu définis ton parcours, tes expériences, tes compétences, tes projets, etc.

La structure suit le schéma officiel :  
https://jsonresume.org/schema/

---

## 🧪 Prévisualiser le CV

Pour vérifier l’apparence avant export :

```bash
resume serve --theme elegant
```

Cela ouvre un serveur local et génère ton CV en temps réel.

---

## 🛠 Compiler / Exporter le CV

### ➤ Export HTML

```bash
resume export cv.html --theme elegant
```

### ➤ Export PDF

Selon ta config, l’export PDF natif peut être capricieux.  
Si ça bloque, exporte en HTML puis imprime en PDF depuis ton navigateur :

```bash
resume export cv.html --theme elegant
```

Ensuite ouvre `cv.html` → Imprimer → Enregistrer en PDF.

---

## 🗂 Arborescence recommandée

```
.
├── resume.json
├── README.md
└── dist/
    ├── cv.html
    └── cv.pdf
```

---

## ❗ Astuce importante (sinon erreur fréquente)

Si tu obtiens :

```
theme path jsonresume-theme-elegant could not be resolved
```

Cela signifie que le thème n’est pas installé **globalement**.  
Réinstalle-le avec :

```bash
npm install -g jsonresume-theme-elegant
```

---

## 🚀 Infos utiles

• Documentation officielle JSON Resume : https://jsonresume.org/  
• Liste des thèmes : https://jsonresume.org/themes/  
• Thème Elegant sur npm : https://www.npmjs.com/package/jsonresume-theme-elegant

---

Tu peux enrichir ce README en ajoutant tes propres scripts npm ou une section CI/CD si tu veux automatiser l’export du CV.  
Le format JSON te permet même de générer plusieurs versions spécialisées en quelques lignes 🎨
