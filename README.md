# API Laravel Event Management

Projekt **API Laravel Event Management** to aplikacja webowa zbudowana w frameworku Laravel, która służy do zarządzania wydarzeniami. Udostępnia RESTful API pozwalające na tworzenie, edytowanie, przeglądanie oraz usuwanie wydarzeń, a także zarządzanie uczestnikami i kategoriami wydarzeń.

## Opis

System pozwala na:
- Dodawanie nowych wydarzeń (eventów)
- Edycję oraz usuwanie istniejących wydarzeń
- Przeglądanie listy wydarzeń i szczegółów
- Zarządzanie kategoriami wydarzeń
- Zarządzanie uczestnikami wydarzeń

Projekt wykorzystuje Laravel jako backend oraz bazę danych MySQL do przechowywania danych.

## Wymagania

- PHP >= 8.1
- Composer
- MySQL/MariaDB
- Laravel >= 10

## Instalacja

1. Sklonuj repozytorium:
    ```bash
    git clone https://github.com/MaciejGuszczak/api_laravel_event_managment.git
    cd api_laravel_event_managment
    ```

2. Zainstaluj zależności:
    ```bash
    composer install
    ```

## Konfiguracja

1. Skopiuj plik `.env.example` do `.env`:
    ```bash
    cp .env.example .env
    ```

2. Ustaw dane dostępowe do bazy danych w pliku `.env`.

3. Wygeneruj klucz aplikacji:
    ```bash
    php artisan key:generate
    ```

4. Wykonaj migracje:
    ```bash
    php artisan migrate
    ```

## Uruchomienie

Uruchom lokalny serwer deweloperski:
```bash
php artisan serve
```
Domyślnie API będzie dostępne pod adresem `http://localhost:8000`.

## Endpointy API

Przykładowe endpointy:
- `GET /api/events` - lista wydarzeń
- `POST /api/events` - dodanie wydarzenia
- `GET /api/events/{id}` - szczegóły wydarzenia
- `PUT /api/events/{id}` - edycja wydarzenia
- `DELETE /api/events/{id}` - usunięcie wydarzenia
- `GET /api/categories` - lista kategorii
- `POST /api/participants` - dodanie uczestnika

Dokładny opis endpointów znajduje się w dokumentacji API (np. plik `/docs` lub komentarze w kontrolerach).

## Testowanie

Aby uruchomić testy:
```bash
php artisan test
```

## Autor

Projekt stworzony przez [Maciej Guszczak](https://github.com/MaciejGuszczak).

---

Jeśli masz pytania lub sugestie, napisz issue lub skontaktuj się przez GitHub.
