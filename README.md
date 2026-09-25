# Soulmate persongalleri

Lokalt kioskgalleri med slumpad personordning, varierade placeringar, mjuk bildöppning och zoom. API-data hämtas vid start och varannan timme.

## Starta

1. Kopiera `config.example.js` till `config.local.js`.
2. Fyll i API-nyckeln i den lokala konfigurationen. Ingen office-parameter behövs.
3. Öppna `index.html` i webbläsaren och använd helskärm.

`config.local.js` är undantagen från Git. API:et behöver tillåta CORS från den lokala sidan. Repositoryt innehåller inga personuppgifter. Vid start utan API visas ett felmeddelande; om en uppdatering misslyckas fortsätter galleriet med den senast inlästa listan. Lokal reservdata kan anges som `fallbackPeople` i `config.local.js`.

JSON-format: `employees` med `name`, `office`, `profileImageBase64` och `texts` (objekt med `label` och `value`).
