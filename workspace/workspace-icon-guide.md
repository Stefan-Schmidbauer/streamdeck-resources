# Workspace Icon Erstellungsanleitung

Diese Anleitung zeigt, wie neue workspace icons im standardisierten Stil erstellt werden.

## Standard Template

Jedes workspace icon folgt dieser einheitlichen Struktur:

```svg
<svg viewBox="0 0 72 72" xmlns="http://www.w3.org/2000/svg">
  <!-- Titelleiste (dunkelgrau) -->
  <rect x="8" y="6" width="56" height="8" rx="3" fill="#34495e"/>
  <rect x="8" y="12" width="56" height="2" fill="#34495e"/>
  
  <!-- Fensterbuttons (standard Farben, links positioniert) -->
  <circle cx="14" cy="10" r="1.5" fill="#f39c12"/>
  <circle cx="18" cy="10" r="1.5" fill="#2ecc71"/>
  <circle cx="22" cy="10" r="1.5" fill="#3498db"/>
  
  <!-- HIER: Anwendungs-spezifischer Inhalt -->
  <!-- [Platz für individuelle Elemente des workspace] -->
  
  <!-- Äußerer Rahmen (IMMER als letztes Element!) -->
  <rect x="8" y="6" width="56" height="44" rx="3" fill="none" stroke="#ecf0f1" stroke-width="2"/>
</svg>
```

## Standardisierte Spezifikationen

### Rahmen & Layout
- **ViewBox**: `0 0 72 72`
- **Äußerer Rahmen**: Position `x="8" y="6"`, Größe `56x44px`
- **Titelleiste**: Höhe 8px + 2px Separator
- **Inhaltbereich**: `y="16"` bis `y="48"` (32px Höhe verfügbar)

### Farben (aus style guide)
- **Rahmen**: `stroke="#ecf0f1" stroke-width="2"`
- **Titelleiste**: `fill="#34495e"`
- **Fensterbuttons**: Orange `#f39c12`, Grün `#2ecc71`, Blau `#3498db`
- **Inhalte**: Nutze Farbpalette aus `icon-style-guide.md`

### Fensterbuttons
- **Position**: `cx="14,18,22" cy="10" r="1.5"`
- **Reihenfolge**: Orange, Grün, Blau (von links nach rechts)

## Schritt-für-Schritt Anleitung

### 1. Template kopieren
Beginne mit dem Standard-Template oben.

### 2. Anwendungs-spezifischen Inhalt hinzufügen
Zwischen den Fensterbuttons und dem äußeren Rahmen:

**Beispiele für verschiedene Workspace-Typen:**

#### Terminal/Konsole
```svg
<text x="14" y="32" fill="#2ecc71" font-family="monospace" font-size="12" font-weight="bold">$</text>
<rect x="22" y="26" width="18" height="2" fill="#ecf0f1"/>
<rect x="42" y="26" width="2" height="2" fill="#ffffff"/>
```

#### Code Editor/IDE
```svg
<text x="36" y="36" fill="#3498db" font-family="monospace" font-size="16" font-weight="bold" text-anchor="middle">&lt;/&gt;</text>
<rect x="14" y="42" width="16" height="2" fill="#ecf0f1"/>
<rect x="18" y="46" width="12" height="2" fill="#2ecc71"/>
```

#### Browser
```svg
<rect x="28" y="14" width="32" height="4" rx="1" fill="#ecf0f1"/>
<circle cx="36" cy="36" r="10" fill="none" stroke="#3498db" stroke-width="2"/>
<line x1="36" y1="26" x2="36" y2="46" stroke="#3498db" stroke-width="1.5"/>
```

#### Präsentation
```svg
<rect x="14" y="26" width="44" height="26" rx="2" fill="#ecf0f1"/>
<rect x="16" y="28" width="40" height="22" fill="#2c3e50"/>
<circle cx="44" cy="38" r="6" fill="#f39c12"/>
<rect x="34" y="52" width="4" height="2" fill="#ecf0f1"/>
```

### 3. Design-Prinzipien befolgen

#### Proportionen
- Nutze verfügbaren Platz effizient (16px bis 48px in y-Achse)
- Halte symmetrische Abstände ein
- Verwende gerundete Ecken (`rx="1"` bis `rx="3"`)

#### Farben strategisch einsetzen
- **Hauptelemente**: `#ecf0f1` (helles Grau)
- **Akzente**: `#3498db` (Blau), `#2ecc71` (Grün), `#f39c12` (Orange)
- **Container**: `#2c3e50` (dunkel), `#34495e` (mittel)

#### Erkennbare Symbole
- Verwende charakteristische Elemente der Anwendung
- Halte Details minimal aber aussagekräftig
- Teste Lesbarkeit bei 72px Größe

### 4. Wichtige Reihenfolge beachten
**CRITICAL**: Der äußere Rahmen muss IMMER das letzte Element sein:
```svg
<rect x="8" y="6" width="56" height="44" rx="3" fill="none" stroke="#ecf0f1" stroke-width="2"/>
```

### 5. Datei speichern
- **Dateiname**: `workspace_[anwendung].svg`
- **Erst speichern als**: `workspace_[anwendung].svg.deleteme`
- **Dann umbenennen zu**: `workspace_[anwendung].svg`

## Beispiele für weitere Workspace-Typen

### Database Tool
```svg
<!-- Cylinder für Database -->
<ellipse cx="36" cy="28" rx="12" ry="4" fill="#3498db"/>
<rect x="24" y="28" width="24" height="16" fill="#3498db"/>
<ellipse cx="36" cy="44" rx="12" ry="4" fill="#2ecc71"/>
```

### Email Client
```svg
<!-- Envelope -->
<rect x="18" y="30" width="36" height="24" rx="2" fill="#ecf0f1"/>
<path d="M18 32 L36 42 L54 32" stroke="#3498db" stroke-width="2" fill="none"/>
```

### Chat/Messaging
```svg
<!-- Speech bubble -->
<rect x="16" y="26" width="32" height="20" rx="4" fill="#2ecc71"/>
<path d="M20 46 L16 50 L24 46" fill="#2ecc71"/>
<rect x="20" y="32" width="20" height="2" fill="#ffffff"/>
```

### Design Tool
```svg
<!-- Artboard with shapes -->
<rect x="16" y="26" width="40" height="24" rx="2" fill="#ecf0f1"/>
<circle cx="28" cy="36" r="4" fill="#3498db"/>
<rect x="36" y="32" width="8" height="8" fill="#f39c12"/>
```

## Qualitätsprüfung

Vor dem Finalisieren prüfen:
- ✅ Rahmen ist letztes Element in SVG
- ✅ Farben entsprechen style guide
- ✅ ViewBox ist 72x72px
- ✅ Proportionen sind ausgewogen
- ✅ Icon ist bei 72px gut erkennbar
- ✅ Dateiname folgt Konvention: `workspace_[name].svg`