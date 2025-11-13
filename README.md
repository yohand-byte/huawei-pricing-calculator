# Huawei Pricing Calculator

Application web monopage permettant de calculer rapidement les prix Huawei avec répartition transport/marge.

## Accès en ligne (GitHub Pages)
- URL : https://yohand-byte.github.io/huawei-pricing-calculator/
- Mot de passe (par défaut) : `Huawei@2025`
- Le mot de passe est stocké sous forme de hash SHA-256 dans `index.html`. Pour le modifier, remplace la constante `PASSWORD_HASH` et mets à jour la valeur via :

```bash
python3 - <<'PY'
import hashlib
print(hashlib.sha256('NOUVEAU_MOT_DE_PASSE'.encode()).hexdigest())
PY
```

## Mise à jour du tableau
1. Mets à jour `index.html` (la logique du calculateur est contenue dans ce fichier).
2. Commit & push sur `main` : GitHub Pages republie automatiquement la dernière version.

## Utilisation hors-ligne
Tu peux toujours ouvrir `index.html` localement. Pour enlever la protection, supprime le bloc `auth-overlay` + le script associé en haut du fichier.
