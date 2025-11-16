# poker-table

Interaktywny stół do pokera online z fikcyjnymi pieniędzmi.

## Technologie
- Frontend: React (TypeScript, Vite)
- Backend: Node.js (Express, Socket.IO)
- Gra: Symulacja Texas Hold'em
- Multiplayer: WebSockets

## Wymagania
- Node.js >= 14
- npm lub yarn

## Instalacja
1. Sklonuj repozytorium: `git clone <url>`
2. Zainstaluj zależności backend: `cd backend && npm install`
3. Zainstaluj zależności frontend: `cd frontend && npm install`

## Uruchomienie
1. Uruchom backend: `cd backend && npm start`
2. Uruchom frontend: `cd frontend && npm run dev`
3. Otwórz przeglądarkę na `http://localhost:5174`

## Jak grać
- Dołącz do gry wpisując nick i klikając "Dołącz do gry".
- Rozpocznij grę gdy jest co najmniej 2 graczy.
- W fazie pre-flop: każdy gracz ma 2 karty (widoczne tylko dla niego).
- Bet, Raise, Call, Fold lub All In.
- Użyj "Następna faza" aby przejść do Flop, Turn, River.
- Po River: zwycięzca zostaje wybrany na podstawie najlepszej ręki pokerowej, a pot zostaje rozdany.

## Funkcje
- Stół pokerowy z kartami i żetonami
- Zarządzanie wirtualną walutą (każdy gracz zaczyna z 1000 żetonów)
- Multiplayer (do 10 graczy)
- Animacje i efekty wizualne
- Timer dla decyzji (30 sekund)
- Automatyczna ocena rąk pokerowych

## API
Backend używa Socket.IO dla komunikacji w czasie rzeczywistym.
Zdarzenia: joinGame, bet, raise, call, fold, allIn, startGame, nextPhase, resetGame.

## Licencja
MIT
