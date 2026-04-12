<p align="center">
  <img src="docs/images/generateur-devis-fr-light.png" alt="Interface du générateur de devis — Palks Studio" width="1200">
</p>

> 🇫🇷 Français | [🇬🇧 English](./README.md)

![License](https://img.shields.io/badge/License-LICENSE.md-lightgreen.svg)
![PDF](https://img.shields.io/badge/Output-PDF-0095b1?style=flat)
![No Dependencies](https://img.shields.io/badge/Dependencies-0-27ae60?style=flat)
![Bilingual](https://img.shields.io/badge/Lang-FR%20%2F%20EN-8e44ad?style=flat)
[![Quote Generator](https://img.shields.io/badge/Quote%20Generator-0095b1?style=flat)](https://palks-studio.com/fr/generateur-devis)

<p align="center">
  <a href="https://palks-studio.com">
    <img src="https://img.shields.io/badge/Palks%20Studio-Website-0095b1?style=for-the-badge" />
  </a>
</p>

# Générateur de devis gratuit — Palks Studio

> Ce dépôt constitue une présentation technique et une documentation du projet.  
> Il ne contient pas de code source téléchargeable ni de fichiers de production.

Un outil web 100% client-side pour générer des devis professionnels en PDF, sans compte, sans serveur, sans données transmises.

**[→ Accéder à l'outil](https://palks-studio.com/fr/generateur-devis)**

---

## Cas d’usage

Exemples d’utilisation :  

- freelances générant rapidement un devis  
- consultants envoyant une proposition simple  
- petites structures préparant un devis client  
- démonstration pédagogique de génération de PDF côté navigateur

---

## Fonctionnalités

- Génération de devis PDF directement dans le navigateur  
- Bilingual **FR / EN** — interface et PDF  
- Logo personnalisé (PNG, JPEG, SVG, WebP)  
- Informations émetteur complètes : SIRET, SIREN, TVA intracommunautaire  
- Lignes de prestations dynamiques avec calcul automatique HT / TVA / TTC  
- Multi-devises : EUR, USD, GBP, CHF, CAD  
- Bloc **Bon pour accord** avec date et signature  
- Design print-friendly — fond blanc, encre minimale  
- Reset automatique du formulaire après téléchargement  
- Aucune donnée conservée, aucun cookie, aucun tracking

---

## Stack

| Technologie                                     | Usage                      |
|-------------------------------------------------|----------------------------|
| HTML / CSS / JS vanilla                         | Interface                  |
| [jsPDF](https://github.com/parallax/jsPDF)      | Génération PDF côté client |
| [DM Sans + DM Mono](https://fonts.google.com/)  | Typographie                |

Aucun framework, aucune dépendance NPM, aucun build step.

---

## Fonctionnement

Le générateur fonctionne entièrement dans le navigateur.

Flux de fonctionnement :  

1. l’utilisateur remplit le formulaire de devis  
2. les données sont traitées en JavaScript  
3. le PDF est généré avec **jsPDF**  
4. le fichier est téléchargé localement

Aucune requête n’est envoyée à un serveur et aucune donnée n’est stockée.

---

## Structure

```
index.html       # Tout-en-un : formulaire + styles + logique + génération PDF
```


---

## Limitations

Cet outil est conçu pour la génération simple de devis.

Il ne comprend pas :  

- de stockage côté serveur  
- de système de numérotation comptable  
- d’intégration avec un logiciel de facturation  
- de système de paiement

Pour des usages plus avancés, un moteur de facturation dédié est nécessaire.

---

## Confidentialité

Le PDF est généré **entièrement dans le navigateur**. Aucune donnée n'est envoyée à un serveur. Aucun stockage local (`localStorage` désactivé). Le formulaire est réinitialisé après chaque téléchargement.

---

© Palks Studio — voir LICENSE.md  
- https://palks-studio.com
