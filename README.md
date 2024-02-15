
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

![image](https://github.com/AnnaPielok/STUDENT/assets/124499788/1443bd2a-46d0-4369-b3f5-f73cf35606f7)


2. POST /create:

Tworzy nowy rekord studenta w tabeli "student".
Oczekuje JSONa w treści żądania z polami "Name" i "Email".
Zwraca obiekt JSON z nowo utworzonym studentem, w tym z wygenerowanym ID.

![image](https://github.com/AnnaPielok/STUDENT/assets/124499788/b71d21c7-99de-4959-aae5-698984eb8718)


3. PUT /update/:id:

Aktualizuje istniejący rekord studenta w tabeli "student".
Oczekuje JSONa w treści żądania z polami "Name" i "Email".
Wymaga parametru :id w ścieżce URL, który odpowiada ID studenta do zaktualizowania.

![image](https://github.com/AnnaPielok/STUDENT/assets/124499788/2c303ef2-6d01-4abf-926b-304d969c079a)

4. DELETE /student/:id:

Usuwa rekord studenta z tabeli "student".
Wymaga parametru :id w ścieżce URL, który odpowiada ID studenta do usunięcia.

