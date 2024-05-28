# BEMSI
projekt BEMSI 2024 Szablon aplikacji WEB - uwierzytelnienie wieloetapowe
Opis rozwiązania z Pytaniem
Chciałbym spróbować napisać aplikację na architekturze mikroserwisów i wykorzystać do tego zadania technologię kontenerową co pozwoliłoby na szybkie stawianie, rozwój czy poprawki w projekcie. Chętnie dowiedziałbym się co Pan Profesor myśli o takim pomyśle i czy jako projekt jednoosobowy z terminem na za 2 miesiące nie jest to zbyt ambitny pomysł. 

Przykładowa architektura:
serwer www
frontend
React
jeden kontener zawierający całą warstwę uwierzytelniającą 
.NET lub Python (Flask lub Django)
baza danych Ldap
i potencjalne inne kontenery potrzebne do takiego rozwiązania (o których w tym momencie nie wiem)
Proces uwierzytelniania: 
1.logowanie “klasyczne” - Nazwa użytkownika plus hasło przechowywane w bazie danych (oczywiście zahaszowane)
2. WebAuth - wykorzystanie biblioteki fido2-net-lib do autentykacji kluczem na urządzeniu mobilnym bądź usb flash
3  Kod TOTP - wykorzystanie biblioteki Otp.NET do autentykacji jednorazowym kodem czasowym

Prowadzenie projektu
Projekt będzie prowadzony za pośrednictwem GitLab chyba, że mógłbym korzystać z GitHub a jedynie oddać na koniec na GitLabie
