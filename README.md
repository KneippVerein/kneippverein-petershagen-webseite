Kneipp-Verein Petershagen – Website
Ganzheitliche Vereins-Website basierend auf der Lehre Sebastian Kneipps. Fokus: klare Informationen, Kurs- und Programmübersicht, attraktive Präsentation der 5 Säulen (Wasser, Bewegung, Ernährung, Heilpflanzen, Balance), gute Lesbarkeit und einfache Pflege.



Inhalt

Überblick
Features
Tech-Stack
Projektstruktur
Loslegen (lokal)
WordPress-Theme nutzen
Deployment
Inhalte pflegen
Qualität und Barrierefreiheit
Lizenz
Mitwirken
Kontakt
Überblick

Ziel: Eine freundliche, barrierearme Website für Mitglieder, Interessierte und Kursleitungen.
Schwerpunkte:
Startseite mit Hero, 5-Säulen-Teaser, Call-to-Actions
Kurse/Angebote, Team/Dozenten, Vereinsinfos
Leicht verständliche Artikel zu Kneipp-Themen (Wasser etc.)
Pflegefreundlich: Inhalte können als Markdown/Seiten gepflegt werden; optional WordPress-Theme inklusive.
Features

Moderne Oberfläche mit hoher Lesbarkeit (Tailwind, shadcn UI)
Seiten für die 5 Säulen (Wasser, Bewegung, Ernährung, Heilpflanzen, Balance)
Kurs-/Angebotsseiten, Team/Dozenten, Kontakt/Beitritt
Responsiv und performant (React 18, Page-Transitions)
Optionales WordPress-Theme (fertig paketiert)
Tech-Stack

Frontend: React 18, TypeScript, Tailwind CSS, shadcn UI, lucide-react
Routing: react-router
Build: esbuild
Optional: WordPress-Theme (PHP, theme.json, Templates/Blocks)
Projektstruktur

src/ … React-App (Seiten, Komponenten, Konfiguration)
public/ … Manifest/Assets
wordpress/kneipp-petershagen … eigenständiges WordPress-Theme
.github/workflows … CI/Release-Workflows (optional)
package.json … Scripts (dev/build)
Loslegen (lokal) Voraussetzungen

Node.js 20+ (empfohlen)
Installation und Entwicklung

npm install
npm run dev
startet den Entwicklungsbuild (esbuild)
npm run build
Produktionsbuild erstellen
Hinweis: React-Router (HashRouter) ist bereits konfiguriert. Tailwind & shadcn UI sind vorbereitet.

WordPress-Theme nutzen (optional)

Ordner: wordpress/kneipp-petershagen
ZIP erstellen:
In WordPress/Backend: Design > Themes > Theme hochladen > kneipp-petershagen.zip
Seiten/Templates:
Startseite, Kurse/Angebote, Lösungen (5 Säulen), Über uns, Veranstaltungen, Kontakt
Säulen-Taxonomie: wasser, bewegung, ernaehrung, heilpflanzen, lebensordnung
Deployment

GitHub Pages (für die React-App):
Optional Workflow einrichten, der den Build nach gh-pages deployt
Externes Hosting:
React: beliebige statische Hoster (z. B. Netlify/Vercel)
WordPress-Theme: klassisches WP-Hosting (PHP/MySQL)
CI:
Wenn .github/workflows vorhanden, Actions aktivieren und Statuschecks für main setzen
Inhalte pflegen

Texte/Artikel liegen als React-Seiten/Komponenten (src/pages/…) vor
Bilder: Nutzen lizenzfreie Quellen oder Vereinsmaterial (Achtung: Rechte klären)
Tipp: Einheitliche Bildsprache – naturnah, freundlich, authentisch
Qualität und Barrierefreiheit

Lesbarkeit: klare Kontraste, skalierbare Schrift, semantische HTML-Struktur
Fokuszustände sichtbar, ARIA-Labels wo sinnvoll
Performance: schlanke Assets, Lazy Loading, wenige Blocker
Design-Hinweis: Bei shadcn UI Buttons mit variant="outline" immer className="bg-transparent" ergänzen
Lizenz Dieses Projekt steht unter der GNU General Public License v3.0 or later (GPL-3.0-or-later). Siehe LICENSE.

Mitwirken

Issues/Feature-Wünsche willkommen
PRs bitte in separaten Branches, CI-Grundregeln beachten
Code-Stil: TypeScript, funktionale Komponenten, kleine, wiederverwendbare Units
Kontakt

Website: https://www.kneippverein-petershagen.de/
E-Mail: info@kneippverein-petershagen.de
Adresse: Kneipp-Zentrum Petershagen, Nachtigallenstr. 9, 32469 Petershagen
