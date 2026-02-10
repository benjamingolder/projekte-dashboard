# Projekte Dashboard - GitHub Pages

Dieses Repository hostet unser Projekte-Dashboard auf GitHub Pages.

## 🚀 Schnellstart

1. **Repository klonen**:
   ```bash
   git clone https://github.com/benimwinkelried/projekte-dashboard.git
   cd projekte-dashboard
   ```

2. **Lokal ansehen**:
   Einfach `index.html` im Browser öffnen.

3. **Änderungen vornehmen**:
   - `index.html` bearbeiten
   - Änderungen committen und pushen
   - Automatische Aktualisierung auf GitHub Pages

## 📋 Dashboard aktualisieren

### Projekte hinzufügen/ändern
1. `index.html` öffnen
2. Im Bereich `<div class="dashboard">` die Projekt-Cards anpassen
3. Format beibehalten:
   ```html
   <div class="project-card [kategorie]">
       <div class="project-header">
           <div class="project-title">[TITEL]</div>
           <div class="project-status [status]">[STATUS]</div>
       </div>
       <div class="project-description">
           [BESCHREIBUNG]
       </div>
       <div class="project-meta">
           <span class="responsible [anna|beny]">#[VERANTWORTLICHER]</span>
           <span class="due-date">[DATUM]</span>
       </div>
   </div>
   ```

### Kategorien
- `high-priority`: Rote Markierung (dringend)
- `this-week`: Orange Markierung (diese Woche)
- `active`: Blaue Markierung (aktiv)
- `backlog`: Graue Markierung (Backlog)

### Status
- `status-today`: Heute fällig
- `status-active`: In Arbeit
- `status-todo`: Noch zu erledigen

## 🌐 Einbettung in SharePoint

### Als iframe:
```html
<iframe src="https://benimwinkelried.github.io/projekte-dashboard/" 
        width="100%" height="800" frameborder="0"></iframe>
```

### Als Webpart:
1. SharePoint Seite bearbeiten
2. "Einbettung" Webpart hinzufügen
3. URL: `https://benimwinkelried.github.io/projekte-dashboard/`

## 🔄 Automatische Updates

Das Dashboard wird automatisch aktualisiert, wenn:
- Änderungen an `index.html` gepusht werden
- GitHub Pages aktiviert ist

## 📞 Support

Bei Fragen oder Problemen:
- Issue im Repository erstellen
- Oder direkt kontaktieren

---

**Live URL**: https://benimwinkelried.github.io/projekte-dashboard/