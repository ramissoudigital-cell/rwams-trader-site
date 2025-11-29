# 📁 Dossier Public - Logos et Images

Ce dossier contient les images statiques de votre site RWAMS Traders.

## 🎨 Comment changer le logo

### Étape 1: Ajoutez votre logo ici
Placez votre fichier logo dans ce dossier :
- `logo.png` - Logo principal (recommandé: 512x512px)
- `logo-white.png` - Version blanche du logo (optionnel)
- `favicon.ico` - Icône de navigateur

### Étape 2: Formats recommandés
- **PNG** avec fond transparent (meilleur pour les logos)
- **SVG** pour une qualité parfaite à toute taille
- **WebP** pour une meilleure compression

### Étape 3: Activez le logo dans le code

#### Dans le Navbar (`components/Navbar.tsx` ligne 34-47):
```tsx
// Commentez l'Option 1 (icône)
{/* Option 1: Icône (actuel) */}
{/* <div className="w-12 h-12 bg-gradient-to-br from-violet-500 to-cyan-500 rounded-xl flex items-center justify-center transform group-hover:scale-110 transition-transform duration-300">
  <TrendingUp className="w-6 h-6 text-white" />
</div> */}

// Décommentez l'Option 2 (image)
<Image
  src="/logo.png"
  alt="RWAMS Traders Logo"
  width={48}
  height={48}
  className="rounded-xl transform group-hover:scale-110 transition-transform duration-300"
/>
```

#### Dans le Footer (`components/Footer.tsx` ligne 18-31):
Faites la même modification.

## 📏 Tailles recommandées

| Usage | Taille | Format |
|-------|--------|--------|
| Logo Navbar | 48x48px | PNG/SVG |
| Logo Footer | 48x48px | PNG/SVG |
| Favicon | 32x32px | ICO/PNG |
| Open Graph | 1200x630px | PNG/JPG |

## 💡 Astuce
Pour un meilleur rendu sur les écrans Retina, utilisez des images 2x plus grandes et laissez Next.js les optimiser automatiquement.
