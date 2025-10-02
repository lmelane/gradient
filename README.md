# Gradient Animation

Deux versions de gradient animé WebGL disponibles :

## 📦 Fichiers

### 1. `gradient.js` - Version Dark Theme
Gradient avec fond sombre et animation complexe.

**Couleurs :**
- Bleu marine sombre (#1A1A2E)
- Bleu-gris (#2D3E50)
- Bleu moyen (#3A5F7D)
- Vert/turquoise (#7DD9A8)
- Vert lime (#5BC98D)
- Turquoise clair (#4ECDC4)

**Caractéristiques :**
- Animation rapide et complexe (30 fps)
- 6 couleurs pour plus de richesse
- Mouvements dynamiques et fluides
- Amplitude élevée (320)

### 2. `gradient-light.js` - Version Light Theme
Gradient clair correspondant exactement à l'image de référence.

**Couleurs :**
- Blanc/gris clair (#F0F5F4)
- Vert menthe pâle (#D5EDE5)
- Vert/turquoise (#7DD9A8)
- Vert lime (#5BC98D)

**Caractéristiques :**
- Animation douce et lente (8 fps)
- 4 couleurs pour un rendu épuré
- Formes ultra-larges et fluides
- Amplitude modérée (150)

## 🚀 Utilisation via CDN

### Version Dark (animation complexe)
```html
<canvas id="gradient-canvas"></canvas>
<script src="https://cdn.jsdelivr.net/gh/lmelane/gradient@main/gradient.js"></script>
<script>
  const gradient = new Gradient();
  gradient.initGradient('#gradient-canvas');
</script>
```

### Version Light (image de référence)
```html
<canvas id="gradient-canvas"></canvas>
<script src="https://cdn.jsdelivr.net/gh/lmelane/gradient@main/gradient-light.js"></script>
<script>
  const gradient = new Gradient();
  gradient.initGradient('#gradient-canvas');
</script>
```

## 🎨 Exemple complet

```html
<!DOCTYPE html>
<html>
<head>
    <title>Gradient Animation</title>
    <style>
        body { 
            margin: 0; 
            padding: 0; 
            overflow: hidden;
        }
        #gradient-canvas { 
            width: 100vw; 
            height: 100vh;
            display: block;
        }
    </style>
</head>
<body>
    <canvas id="gradient-canvas"></canvas>
    
    <!-- Choisissez une version : -->
    
    <!-- Version Dark -->
    <!-- <script src="https://cdn.jsdelivr.net/gh/lmelane/gradient@main/gradient.js"></script> -->
    
    <!-- Version Light -->
    <script src="https://cdn.jsdelivr.net/gh/lmelane/gradient@main/gradient-light.js"></script>
    
    <script>
        const gradient = new Gradient();
        gradient.initGradient('#gradient-canvas');
    </script>
</body>
</html>
```

## 📝 Notes

- Les deux versions utilisent WebGL pour des performances optimales
- L'animation est fluide et responsive
- Compatible avec tous les navigateurs modernes
- Aucune dépendance externe requise
