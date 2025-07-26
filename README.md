# black-market-app

React Native + Expo app for tracking discounts in supermarkets.
![Login Screen](./ansicht/1.png)

# Black Market Anwendung

Installations- und Startanleitung

## Voraussetzungen

- Node.js 16+ (für Frontend)
- Java 17+ (für Backend)
- Docker (optional für PostgreSQL)
- PostgreSQL 15+

## Backend (Spring Boot)

### Ersteinrichtung

1. **Datenbank einrichten**:

   ```bash
   docker run --name postgres_container -e POSTGRES_USER=django_user -e POSTGRES_PASSWORD=password -e POSTGRES_DB=black_market_db -p 5432:5432 -d postgres:15
   ```

2. **Abhängigkeiten installieren**:
   `cd backend`
   `mvn clean install`

### Anwendung starten

`mvn spring-boot:run`

## Frontend

`cd blackMarket`
`npx expo start --clear`
