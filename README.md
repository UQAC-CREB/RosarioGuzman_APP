# Sélection de sites forestiers — PIG & EPN

Application web interactive de visualisation et de filtrage de sites d'échantillonnage forestier au Québec.

🔗 **[Accéder à l'application](https://uqac-creb.github.io/RosarioGuzman_APP/)**

---

## Description

L'application affiche 275 points d'inventaire répartis en deux groupes d'espèces :
- **PIG** — Pin gris (*Pinus banksiana*)
- **EPN** — Épinette noire (*Picea mariana*)

Les données de sol proviennent de la couche 0–5 cm et incluent sept variables explicatives : azote total (N), argile (Clay), fractions grossières (CoarseF), pH eau (PHw), sable (Sand), carbone organique (SOC) et limon (Silt).

## Fonctionnalités

**Filtres**
- Sélection par espèce (PIG, EPN ou les deux)
- Sélection d'une variable explicative avec gradient de couleur vert → jaune → rouge sur la carte
- Slider double curseur pour filtrer les points selon une plage de valeurs

**Carte**
- Fond cartographique light gray (CARTO)
- Info-bulle au survol : identifiant du point, espèce, et valeur de la variable si sélectionnée
- Légende dynamique (espèces ou gradient selon le mode actif)

**Export**
- Export CSV de la sélection active avec nom de fichier généré automatiquement (`Espèce_Variable_min_max.csv`)

## Structure

```
web/
└── index.html    # Application auto-contenue (données intégrées, aucune dépendance externe)
```

## Technologies

[Leaflet.js](https://leafletjs.com/) · [noUiSlider](https://refreshless.com/nouislider/) · CARTO Basemaps
