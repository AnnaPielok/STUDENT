REJESTR STUDENTÓW

Backend aplikacji to system CRUD, który demonstruje podstawowe mechanizmy tworzenia aplikacji webowych z wykorzystaniem Node.js, Express.js i MySQL.

API udostępnia podstawowe funkcje CRUD (Create, Read, Update, Delete) dla zarządzania danymi studentów. Używa standardowych kodów odpowiedzi HTTP i formatu JSON do wymiany danych.


Technologia:

Backend aplikacji jest napisany w języku JavaScript i wykorzystuje następujące technologie:

-Node.js: Platforma do uruchamiania aplikacji JavaScript po stronie serwera.

-Express.js: Framework webowy ułatwiający tworzenie serwerów HTTP w Node.js.

-MySQL: System zarządzania bazami danych (DBMS) do przechowywania danych studentów.

Architektura:

Backend składa się z następujących elementów:

Opis API
Metody:

API udostępnia cztery metody HTTP:

1. GET /:

Pobiera wszystkie rekordy z tabeli "student".
Zwraca listę obiektów JSON, z których każdy reprezentuje jednego studenta.

2. POST /create:

Tworzy nowy rekord studenta w tabeli "student".
Oczekuje JSONa w treści żądania z polami "Name" i "Email".
Zwraca obiekt JSON z nowo utworzonym studentem, w tym z wygenerowanym ID.

3. PUT /update/:id:

Aktualizuje istniejący rekord studenta w tabeli "student".
Oczekuje JSONa w treści żądania z polami "Name" i "Email".
Wymaga parametru :id w ścieżce URL, który odpowiada ID studenta do zaktualizowania.

4. DELETE /student/:id:

Usuwa rekord studenta z tabeli "student".
Wymaga parametru :id w ścieżce URL, który odpowiada ID studenta do usunięcia.
