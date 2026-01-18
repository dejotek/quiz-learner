# Platforma Quizowa – Frontend (React + TS) + Backend (NestJS)
 
## Informacje ogólne
 
Projekt składa się z dwóch części.
 
Frontend: aplikacja webowa typu SPA (React + TypeScript) do przeglądania i rozwiązywania quizów.
Backend: API w NestJS udostępniające dane o quizach, pytaniach i wynikach oraz przygotowujące system pod logowanie, rankingi i statystyki.
 
Platforma pozwala użytkownikom wybierać quizy, odpowiadać na pytania (jednokrotny lub wielokrotny wybór), mierzyć czas rozwiązywania i otrzymywać wynik końcowy.
 
---

## Wymagania funkcjonalne
 
Frontend
 
* Przeglądanie listy dostępnych quizów
* Uruchomienie wybranego quizu
* Wyświetlanie pytań i odpowiedzi
* Obsługa odpowiedzi jednokrotnego i wielokrotnego wyboru
* Zliczanie punktów na podstawie poprawnych odpowiedzi
* Pomiar czasu trwania quizu
* Ekran podsumowania z wynikiem
* Nawigacja pomiędzy widokami aplikacji
 
Backend (NestJS API)
 
* Endpoint listy quizów
* Endpoint szczegółów quizu (pytania + odpowiedzi)
* Walidacja i zapis wyników quizu
* Udostępnienie historii wyników (opcjonalnie)
* Namespace i wersjonowanie endpointów (np. /api/v1)
 
---
 
## Wymagania niefunkcjonalne
 
### Technologiczne
 
Frontend
 
* React (SPA)
* TypeScript – pełne typowanie danych
* Struktura feature-based
* Rozdzielenie UI, logiki i komunikacji z API
 
Backend
 
* NestJS (Node.js)
* TypeScript
* DTO + walidacja danych (class-validator / class-transformer)
* Warstwy: controller → service → repository
* Możliwość pracy w trybie mock/in-memory lub z bazą danych
 
### Wydajnościowe
 
Frontend
 
* Szybkie przełączanie pytań bez przeładowania strony
* Ograniczanie niepotrzebnych renderów
* Gotowość pod lazy loading widoków
 
Backend
 
* Stabilne czasy odpowiedzi API
* Gotowość pod paginację w listach
* CORS + podstawowe zabezpieczenia (opcjonalnie: helmet, rate limit)
 
---

## Funkcjonalności / moduły systemu
 
Frontend
 
* Moduł quizów
 
  * lista quizów
  * rozpoczęcie quizu
  * przebieg quizu
  * wynik końcowy
 
* Moduł pytań
 
  * wyświetlanie treści pytania
  * obsługa wyboru odpowiedzi
 
* Moduł nawigacji
 
  * routing pomiędzy widokami
 
Backend (NestJS)
 
* Moduł Quizzes
 
  * lista quizów
  * szczegóły quizu
 
* Moduł Results
 
  * zapis wyniku
  * historia wyników
 
W przyszłości
 
* moduł Auth (rejestracja/logowanie)
* moduł Users/Profile
* statystyki i rankingi
 
---
