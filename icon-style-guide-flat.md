# Stream Deck Icon Style Guide

## Allgemeine Spezifikationen
- **Format**: SVG
- **Größe**: 72x72px (ViewBox: 0 0 72 72)
- **Stil**: Modern Flat Design
- **Hintergrund**: Transparent (für schwarzen Stream Deck Hintergrund optimiert)

## Farbpalette

### Hauptfarben (helle Elemente)
- **Primärweiß**: `#ffffff` - Für wichtige Hauptelemente
- **Sekundärweiß**: `#ecf0f1` - Für Text und Details

### Akzentfarben
- **Blau**: `#3498db` - Für interaktive Elemente, Links, Code-Syntax
- **Grün**: `#2ecc71` - Für positive Aktionen, Terminal-Prompt, Erfolg
- **Orange**: `#f39c12` - Für Warnungen, Hervorhebungen, Buttons

### Dunkle Elemente (nur für Kontrast)
- **Dunkelblau**: `#2c3e50` - Für Hintergründe von Fenstern/Containern
- **Dunkelgrau**: `#34495e` - Für sekundäre Hintergründe

## Design-Prinzipien

### Formen
- **Flache Formen**: Keine Schatten oder 3D-Effekte
- **Gerundete Ecken**: rx="2" bis rx="3" für weiche Kanten
- **Klare Geometrie**: Einfache, erkennbare Grundformen

### Linien und Striche
- **Stroke-Width**: 2-3px für gute Sichtbarkeit bei 72px
- **Minimale Details**: Nur wesentliche Elemente darstellen
- **Hoher Kontrast**: Helle Elemente auf transparentem Hintergrund

### Typografie
- **Font-Family**: `monospace` für Code-Elemente
- **Font-Size**: 8-12px je nach Kontext
- **Farbe**: Entsprechend der Akzentfarben

## Icon-Kategorien

### Anwendungen
- **Fenster**: Rahmen in `#ecf0f1`, Titelleiste in `#34495e`
- **Inhalte**: Farbige Akzente je nach Funktion
- **Beispiel**: IDE mit `#3498db` für Code-Syntax

#### Workspace Icons (Spezialfall)
- **Standardisierte Struktur**: Einheitliche Rahmen und Titelleisten für alle workspace-bezogenen Icons
- **Template verfügbar**: Siehe `workspace-icon-guide.md` für detaillierte Anleitung
- **Erkennungsmerkmale**: Fensterbuttons (Orange/Grün/Blau), einheitlicher 56x44px Rahmen
- **Beispiele**: `workspace_terminal.svg`, `workspace_ide.svg`, `workspace_browser.svg`

### Navigation
- **Pfeile**: Einfache Polygone in `#ecf0f1`
- **Buttons**: Gerundete Rechtecke, klare Formen
- **Beispiel**: Previous/Next Pfeile

### Medien-Kontrollen
- **Symbole**: Standard-Icons (Play, Pause, etc.)
- **Farbe**: Hauptsächlich `#ecf0f1`
- **Größe**: Gut sichtbar bei 72px

### System/Übersicht
- **Grids**: Gleichmäßige Abstände, gerundete Ecken
- **Highlight**: Ein Element in Akzentfarbe hervorheben
- **Beispiel**: Overview-Grid mit einem blauen Quadrat

## Beispiel-Template

```svg
<svg viewBox="0 0 72 72" xmlns="http://www.w3.org/2000/svg">
  <!-- Haupt-Container -->
  <rect x="8" y="8" width="56" height="56" rx="3" fill="#2c3e50" stroke="#ecf0f1" stroke-width="2"/>
  
  <!-- Inhalt/Details -->
  <rect x="12" y="12" width="48" height="8" fill="#34495e"/>
  
  <!-- Akzent-Elemente -->
  <rect x="16" y="20" width="20" height="3" fill="#3498db"/>
  <rect x="16" y="26" width="16" height="3" fill="#2ecc71"/>
  <rect x="16" y="32" width="24" height="3" fill="#f39c12"/>
</svg>
```

## Qualitätskriterien
- ✅ Bei 72px gut erkennbar
- ✅ Hoher Kontrast zu schwarzem Hintergrund
- ✅ Minimale, klare Formen
- ✅ Konsistente Farbverwendung
- ✅ Responsive Design (funktioniert auch bei kleineren Größen)