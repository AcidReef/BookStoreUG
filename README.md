# Book Store
> „Pokój bez książek jest jak ciało bez duszy.” ~ Cyceron

## Spis Treści
- [Wprowadzenie](#wprowadzenie)
- [Funkcjonalności](#funkcjonalności)
- [Technologie](#technologie)
- [Uruchomienie projektu](#uruchomienie-projektu)
- [API](#api)

---

## Wprowadzenie
Book Store to projekt zbudowany przy użyciu stacku MERN (MongoDB, Express, React, Node.js).
Projekt biblioteki cyfrowej umożliwiający tworzenie cyfrowego zbioru swoich książek. Projekt umożlwia edycję i usuwanie pozycji już istniejących.

## Funkcjonalności
- [ ] Rejestracja użytkowników.
- [ ] Logowanie z uwierzytelnieniem JWT.
- [x] CRUD książek.
- [x] Interfejs użytkownika z React.
- [x] Możliwość edycji zbiorów.

## Technologie
- **Frontend**: React, Tailwind CSS
- **Backend**: Node.js, Express
- **Baza danych**: MongoDB
- **Inne**: Axios, JWT, Mongoose

## Uruchomienie projektu
1. Zainstaluj zależności:
   ```bash
   npm install

2. Skonfiguruj plik .env
   ```env
   MONGO_URI=mongodb://localhost:27017/mern_project
   JWT_SECRET=your_secret_key

3. Uruchom aplikację
   ```bash
   npm run dev

## API
Testy przeprowadzono w środowisku Postman.
Endpointy użytkownika:
-	POST /api/users/register - rejestracja nowego użytkownika
-	POST /api/users/login - logowanie użytkownika
-	GET /api/users/me - pobieranie danych zalogowanego użytkownika

Endpointy książek:
- GET /api/books - pobieranie listy książek
- POST /api/books - dodanie nowej książki
- PUT /api/books/:id - edycja książki
- DELETE /api/books/:id - usunięcie książki
