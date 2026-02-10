# SharePoint Einbettungsanleitung

## 🎯 Schnellstart

**Dashboard URL**: `https://benjamingolder.github.io/projekte-dashboard/`

## 📋 Einbettung in SharePoint

### Methode 1: iframe (Empfohlen)

1. **SharePoint Seite bearbeiten**
   - Auf die gewünschte Seite gehen
   - "Bearbeiten" anklicken

2. **Code-Snippet Webpart hinzufügen**
   - "+" zum Webpart hinzufügen
   - "Code-Snippet" oder "Einbettung" suchen und auswählen

3. **HTML Code einfügen**:
```html
<div style="width: 100%; height: 800px; border: 1px solid #ddd; border-radius: 8px;">
    <iframe 
        src="https://benjamingolder.github.io/projekte-dashboard/" 
        width="100%" 
        height="100%" 
        frameborder="0" 
        style="border-radius: 8px;">
    </iframe>
</div>
```

### Methode 2: Modernes Webpart

1. **Einbettungs-Webpart verwenden**
   - "Einbettung" Webpart hinzufügen
   - URL eingeben: `https://benjamingolder.github.io/projekte-dashboard/`
   - Höhe: 800px einstellen

### Methode 3: Reaktive Höhe (Advanced)

Für automatische Höhenanpassung:
```html
<script>
window.addEventListener('message', function(e) {
    if (e.origin !== 'https://benjamingolder.github.io') return;
    
    var iframe = document.querySelector('iframe[src*="projekte-dashboard"]');
    if (iframe && e.data.height) {
        iframe.style.height = e.data.height + 'px';
    }
});
</script>
<iframe src="https://benjamingolder.github.io/projekte-dashboard/" 
        width="100%" 
        height="800" 
        frameborder="0">
</iframe>
```

## ⚙️ Anpassungsmöglichkeiten

### Höhe ändern
- Standard: 800px
- Klein: 600px
- Groß: 1000px
- Vollbild: 100vh

### Breite anpassen
- Standard: 100% (füllt verfügbare Breite)
- Fest: 1200px
- Responsive: minmax(300px, 1fr)

### Styling-Optionen
```html
<style>
.dashboard-container {
    border: 2px solid #0078d4;
    border-radius: 10px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    overflow: hidden;
}
</style>
```

## 🔒 Sicherheit & Zuverlässigkeit

### Vorteile von GitHub Pages
- ✅ **Kostenlos** - Keine Hosting-Kosten
- ✅ **SSL verschlüsselt** - Sichere HTTPS-Verbindung
- ✅ **99.9% Uptime** - Zuverlässige Verfügbarkeit
- ✅ **CDN weltweit** - Schnelle Ladezeiten
- ✅ **Automatische Updates** - Bei Code-Änderungen

### SharePoint Vorteile
- ✅ **Integriert** - Direkt in SharePoint Umgebung
- ✅ **Responsive** - Funktioniert auf allen Geräten
- ✅ **Keine zusätzlichen Berechtigungen** - Öffentlich zugänglich

## 🚨 Fehlerbehebung

### Problem: Dashboard wird nicht angezeigt
**Lösung**: 
- URL prüfen: `https://benjamingolder.github.io/projekte-dashboard/`
- Browser Konsole öffnen (F12) für Fehlermeldungen
- SharePoint Berechtigungen prüfen

### Problem: Zu klein/groß
**Lösung**:
- Höhe im iframe Code anpassen
- CSS Media Queries verwenden
- Verschiedene Höhen für Desktop/Mobile

### Problem: Verbindung nicht sicher
**Lösung**:
- Immer HTTPS URL verwenden
- Nie HTTP verwenden
- SSL Zertifikat ist automatisch vorhanden

## 📱 Mobile Optimierung

Das Dashboard ist vollständig responsive und passt sich automatisch an:
- 📱 **Smartphones**: Einspaltiges Layout
- 📋 **Tablets**: Zwei-Spalten Layout  
- 💻 **Desktop**: Mehrspaltiges Layout

## 🔄 Automatische Aktualisierung

- **Live-Uhrzeit**: Aktualisiert jede Sekunde
- **Daten**: Automatisches Reload alle 5 Minuten
- **Manuell**: Browser-Seite neu laden für sofortige Updates

## 📞 Support

Bei Problemen:
1. Repository checken: https://github.com/benjamingolder/projekte-dashboard
2. Issue erstellen im Repository
3. Oder direkt kontaktieren

---

**🔗 Dashboard URL**: https://benjamingolder.github.io/projekte-dashboard/