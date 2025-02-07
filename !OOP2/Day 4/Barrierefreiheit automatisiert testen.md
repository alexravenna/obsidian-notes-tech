- Anna Maier von codecentric
- Tools
	- finden der langweilen "Bugs"
	- grundlegende Barrierefreiheit
- WCAG criteria
	- nicht alle automatisierbar
- keyboard navigation
	- Tabreihenfolge aufzeigen
	- Playwright page.keyboard
		- assert content of focused element
- Textgröße 
	- nicht dasselbe wie Zoom
	- root DOM `fontSize` setzen
	- Layout testable with Playwright
- Barrierefreiheit braucht Kontext
- manuelles Testen bleibt notwendig

Axe Dashboard 
In Prozess einbauen

Tools
- jest-axe
- @axe-core/playwright
- pa11y for CI
	- dashboard, html, json output
- Accessibility tree in DevTools
- Testing library `findByRole`
- Playwright with `getByRole`
- Accessibility Insights for Web
- overlayfactsheet.com