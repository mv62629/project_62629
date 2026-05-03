# ZADANIE 8 - Backend

Projekt spelnia wymagania zadania:

1. Wysylka danych formularza metoda POST
2. Zapis danych poza przegladarka (plik serwera `data/submissions.json`)
3. Potwierdzenie poprawnego wyslania danych na froncie
4. Mozliwosc pokazania w wideo, gdzie dane trafiaja

## Jak uruchomic

1. Otworz terminal w folderze projektu.
2. Uruchom:

```bash
npm start
```

3. Otworz w przegladarce:

```text
http://localhost:3000
```

## Co zostalo dodane

- Backend: `server.js`
- Endpointy API:
  - `POST /api/submissions` - zapisuje dane formularza
  - `GET /api/submissions` - zwraca ostatnio zapisane wpisy
- Trwale przechowywanie danych: `data/submissions.json`
- Frontend (w `script.js`):
  - formularz "Zadanie 8 - backend (POST + zapis na serwerze)"
  - wysylka `fetch(..., { method: 'POST' })`
  - komunikat o sukcesie / bledzie
  - lista ostatnich wpisow odczytana z backendu

## Jak pokazac to na wideo

1. Uruchom serwer (`npm start`).
2. Otworz strone pod `http://localhost:3000`.
3. Wypelnij formularz "Zadanie 8 - backend" i kliknij wysylke.
4. Pokaz komunikat sukcesu na stronie.
5. Otworz plik `data/submissions.json` i pokaz, ze wpis zostal dopisany.
