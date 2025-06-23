# 🌍 Yaro – Prototype Iteratie 1
Yaro is een interactief platform dat reizigers actuele, locatiegebonden meldingen toont via een wereldkaart. Deze eerste iteratie richt zich op het verkennen van de basisfunctionaliteiten en het vormgeven van een eerste visuele ervaring die aansluit bij de behoeften van bewuste reizigers.

## ✨ Features
### 🗺️ Interactieve Kaart
- Klikbare kaart om nieuwe locaties en verhalen te selecteren
### 🔍 Verhalen bekijken
- Lokale verhalen verteld door de lokale bevolking
- Interactieve pins op de kaart met popup details
- De mogelijkheid om als local je eigen verhaal te delen
### 📰 Do's and Dont's
- Een actuele culturele etiquette quiz
- Een overzicht per stad over de culturele normen en waarden
### 📰 Budget and Tips
- Duidelijk overzicht voor tips in het buitenland
- Overzicht over vervoer in het buitenland
- Overzicht over gemiddelde dagelijkse uitgave op basis van lokale prijzen.
### 🎨 Moderne UI/UX
- Responsive design voor desktop en mobiel
- Shadcn/ui componenten voor consistente styling
- Tailwind CSS voor moderne styling
- Smooth animaties en hover effecten
- Intuïtieve interface met duidelijke feedback

## 📚 Lessons Learned
Tijdens deze eerste iteratie leerden we hoe belangrijk het is om vroeg te testen met gebruikers. Onze Thinking Aloud-test bracht snel visuele knelpunten en verwarring rondom navigatie aan het licht. Ook realiseerden we ons dat een goede visualisatie cruciaal is voor vertrouwen en overzicht.
Daarnaast leerden we hoe iteratief werken, zelfs met AI-tools, zorgt voor snelle feedbackloops waarmee we de basis voor onze volgende versies konden leggen.

## 🏗️ Projectstructuur
```bash
world-view-news/
├── public/                         # Statische bestanden zoals afbeeldingen of favicon
├── src/
│   ├── components/                 # Herbruikbare UI-componenten
│   │   ├── Header.tsx             # Zoekbalk, logo, navigatie
│   │   ├── MapComponent.tsx       # Leaflet-kaart met locatie-zoekfunctie
│   │   ├── NewsPanel.tsx          # Nieuwsitems in een lijst of slider
│   │   └── ui/                    # (shadcn/ui) gestylede UI-elementen (zoals buttons, modals)
│   ├── pages/                     # Pagina’s voor routing
│   │   ├── Index.tsx              # Hoofdpagina met kaart en nieuws
│   │   ├── Login.tsx              # Inlogpagina
│   │   └── NotFound.tsx           # 404 fallback pagina
│   ├── services/                  # API-interactie of datavergaring
│   │   ├── LocationService.ts     # Geocoding of Leaflet API helper
│   │   └── NewsService.ts         # Haalt nieuws op of simuleert data
│   ├── hooks/                     # Custom React Hooks
│   │   └── use-toast.ts           # Toasts voor gebruikersfeedback
│   ├── lib/                       # Hulpmethodes en utils
│   │   └── utils.ts               # Helperfuncties voor bv. dataverwerking
│   ├── App.tsx                    # Hoofdcomponent met router
│   ├── App.css                    # Stijlen specifiek voor App component
│   ├── index.css                  # Globale CSS (Tailwind import)
│   ├── main.tsx                   # Entry point (render App.tsx)
│   └── vite-env.d.ts              # Types voor Vite omgevingsvariabelen
├── .gitignore
├── bun.lockb                     # (optioneel) bundler lockfile
├── components.json               # Shadcn component configuratie
├── eslint.config.js              # ESLint instellingen
├── index.html                    # Root HTML-bestand
├── package-lock.json
├── package.json
├── postcss.config.js             # PostCSS + Tailwind config
├── README.md
├── tailwind.config.ts
├── tsconfig.app.json
├── tsconfig.json
├── tsconfig.node.json
└── vite.config.ts                # Vite bundler configuratie
```

## 📌 Andere iteraties:
Volgende iteraties van het project vind je hier:
### Iteratie 2:
- https://github.com/ThomasPrinsen/local-story-explorer
- https://local-story-explorer.vercel.app/verhalen

### Iteratie 3 (Def)
- https://github.com/ThomasPrinsen/world-view-news
- https://world-view-news.vercel.app/
