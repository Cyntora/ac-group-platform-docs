# AC Group Platform — Internt strategidokument

Ett internt strategidokument för Angry Creative Group om varför vi
bör bygga en gemensam AI-plattform för digital marknadsföring och
webbutveckling.

## Innehåll

Webbplatsen består av fem delar:

1. **Översikt** (`index.html`) — sammanfattning och varför nu
2. **Koncernen** (`koncernen.html`) — hur Cyntora, Angry Creative, Bishop och Synotio drar nytta
3. **Användning** (`anvandning.html`) — konkreta scenarier per yrkesroll
4. **Affärsvärde** (`affarsvarde.html`) — investering, ROI, intäktsmöjligheter
5. **Teknik** (`teknik.html`) — arkitektur, integrationer, säkerhet
6. **Roadmap** (`roadmap.html`) — faser, beslutspunkter, nästa steg

## Designsystem

Webbplatsen följer Cyntoras designsystem:

- **Färger:** Charcoal (#272723), Warm Taupe (#5A4D41), Warm Off-White (#F8F6EC)
- **Typografi:** Poppins (display), Montserrat (brödtext)
- **Layout:** 1440px max-width, generöst whitespace, skarpa kanter
- **Filosofi:** Scandinavian minimalism, sofistikerad återhållsamhet

## Publicera på GitHub Pages

### Steg 1: Skapa ett GitHub-repo

```bash
cd /sökväg/till/cyntora-platform-site
git init
git add .
git commit -m "Initial commit: AC Group Platform strategy site"
```

Skapa ett nytt repo på GitHub (privat eller publikt) — t.ex. `ac-group-platform-docs`.

```bash
git remote add origin https://github.com/[ditt-username]/ac-group-platform-docs.git
git branch -M main
git push -u origin main
```

### Steg 2: Aktivera GitHub Pages

1. Gå till repots **Settings** på GitHub
2. Klicka på **Pages** i vänstermenyn
3. Under **Source**, välj **Deploy from a branch**
4. Välj branch **main** och folder **/ (root)**
5. Klicka **Save**

Efter 1–2 minuter är sidan tillgänglig på:

```
https://[ditt-username].github.io/ac-group-platform-docs/
```

### Steg 3: (Valfritt) Egen domän

Om du vill använda en egen domän som t.ex. `platform.cyntora.se`:

1. Skapa en fil `CNAME` i repots root med innehåll: `platform.cyntora.se`
2. Hos domän-leverantören, lägg till en CNAME-record som pekar mot `[ditt-username].github.io`
3. Vänta på att DNS sprids (kan ta upp till 24 timmar)
4. Aktivera HTTPS i GitHub Pages-inställningarna när domänen verifieras

## Lokal förhandsgranskning

Filerna är ren HTML/CSS utan byggsteg. För att förhandsgranska lokalt:

```bash
# Med Python (vanligt installerat)
cd cyntora-platform-site
python3 -m http.server 8000

# Eller med Node.js
npx http-server -p 8000
```

Öppna sedan `http://localhost:8000` i webbläsaren.

## Justeringar

Vill du justera innehåll eller design? Allt är ren HTML/CSS — öppna
respektive `.html`-fil i en editor och redigera direkt. CSS finns i
`styles.css` och bygger på CSS-variabler för enkel temat-anpassning.

För större ändringar i designsystemet — se `DESIGN_CYNTORA.md` för
fullständig specifikation av färger, typografi, komponenter och
layoutprinciper.

## Frågor?

Detta är ett internt dokument från Cyntora AB. Frågor om innehållet
besvaras enklast genom Cyntoras kontaktyta i Angry Creative Group.

---

Maj 2026
