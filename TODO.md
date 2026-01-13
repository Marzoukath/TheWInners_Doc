# Réduction de la taille de police - Plan d'exécution

## Objectif
Réduire la taille de police des écrits de manière proportionnelle et cohérente

## Étapes à accomplir

### 1. Modifier la configuration de base des polices
- [x] Modifier src/config/theme.json
  - Réduire base : 16px → 14px (-12.5%)
  - Ajuster scale : 1.15 → 1.12

### 2. Ajuster les styles CSS de base
- [x] Modifier src/styles/base.css
  - Réduire taille corps : 20px → 17px (-15%)
  - Ajuster les titres (h1-h6) - réduire les augmentations

### 3. Réduire les tailles des composants
- [x] Modifier src/styles/components.css
  - Section title : 4.8rem → 3.5rem (-27%)
  - Section description : 1.125rem → 1rem
  - Ajuster les media queries

### 4. Tester le résultat
- [x] Vérifier la lisibilité sur différentes tailles d'écran
- [x] S'assurer que la hiérarchie visuelle est maintenue

## Modifications techniques

### Configuration theme.json
```json
{
  "fonts": {
    "font_size": {
      "base": "14",    // était 16
      "scale": "1.12"  // était 1.15
    }
  }
}
```

### Styles de base (base.css)
- Réduction générale de 15% sur les tailles de base
- Aj proportionnelles pour h1-h6

### Composants (components.css)
- Section title : réduction importante pour équilibre
- Section description : normalisation à 1rem

