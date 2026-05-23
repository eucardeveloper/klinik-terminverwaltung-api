# Klinik Terminverwaltung API

Eine REST API zur Verwaltung von Klinikterminen, entwickelt mit Spring Boot 3.5 und PostgreSQL.

## Technologien

- Java 21
- Spring Boot 3.5
- Spring Data JPA
- PostgreSQL
- Swagger / OpenAPI
- Maven

## Funktionen

- Termin erstellen
- Alle Termine abrufen
- Termin nach ID abrufen
- Termin aktualisieren
- Termin löschen
- Validierung der Eingabedaten
- Globale Fehlerbehandlung

## Installation

1. Repository klonen:
git clone https://github.com/eucardeveloper/klinik-terminverwaltung-api.git
2. Konfigurationsdatei erstellen: `src/main/resources/application.properties`

3. Folgende Einstellungen eintragen:

   spring.datasource.url=jdbc:postgresql://localhost:5432/klinik_terminverwaltung

   spring.datasource.username=postgres

   spring.datasource.password=DEIN_PASSWORT

   spring.jpa.hibernate.ddl-auto=update

   spring.jpa.show-sql=true

4. Anwendung starten:
   mvn spring-boot:run

## API Dokumentation

Nach dem Start erreichbar unter: `http://localhost:8080/swagger-ui/index.html`

## API Endpunkte

| Method | Endpoint | Beschreibung |
|--------|----------|--------------|
| GET | /api/termine | Alle Termine abrufen |
| GET | /api/termine/{id} | Termin nach ID abrufen |
| POST | /api/termine | Neuen Termin erstellen |
| PUT | /api/termine/{id} | Termin aktualisieren |
| DELETE | /api/termine/{id} | Termin löschen |