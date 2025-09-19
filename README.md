<div align="center">

# ✨ ZenithPlots ✨
### _Najbardziej zaawansowany plugin na działki dla serwerów Minecraft 1.21+_

**ZenithPlots** to nowoczesny, w pełni konfigurowalny i zoptymalizowany plugin na działki, stworzony z myślą o serwerach Survival, RPG Oferuje graczom intuicyjny system zarządzania swoimi terenami za pomocą menu GUI, a administratorom daje potężne narzędzia do kontroli i moderacji.

![Java](https://img.shields.io/badge/Java-21-blue?style=for-the-badge&logo=openjdk)
![API](https://img.shields.io/badge/API-Paper_1.21-orange?style=for-the-badge&logo=server)
![Wersja](https://img.shields.io/badge/Wersja-1.0-brightgreen?style=for-the-badge)

</div>

---

## 🚀 Główne Funkcje

-   **Intuicyjne GUI:** Prawie wszystkie akcje wykonuje się w estetycznych i w pełni konfigurowalnych menu.
-   **System Ról i Uprawnień:** Daj swoim znajomym jedną z wielu ról (`Współwłaściciel`, `Moderator`, `Zaufany`, `Członek`, `Odwiedzający`) i zarządzaj ich uprawnieniami na swojej działce.
-   **Edytor Uprawnień:** Właściciele działek mogą dostosować każdą permisję dla każdej roli, tworząc unikalne zestawy uprawnień.
-   **Ulepszenia Działki:** Zwiększaj rozmiar działki, limity skrzyń, lejów i członków, inwestując zarobione pieniądze.
-   **Bank Działki:** Wspólny skarbiec, do którego członkowie mogą wpłacać środki na rozwój działki.
-   **System Wygasania:** Działki mają datę ważności, którą można przedłużać, co zapobiega powstawaniu opuszczonych terenów.
-   **Konfigurowalny Border:** Włącz wizualny border z cząsteczek, aby oznaczyć granice swojej działki i wybierz jego kolor.
-   **Ochrona Terenu:** Zaawansowana ochrona przed budowaniem, niszczeniem, interakcjami i PvP.
-   **Pełna Konfiguracja:** Dostosuj każdą wiadomość, wygląd każdego menu, koszty ulepszeń i zasady w plikach `.yml`.
-   **Wsparcie dla Baz Danych:** Wybierz między lekkim **SQLite** a potężnym **MariaDB/MySQL**.
-   **Tryb Bypass dla Admina:** Administratorzy mogą swobodnie zarządzać każdą działką bez ograniczeń.
-   **Optymalizacja:** Plugin został napisany z myślą o wydajności, wykorzystując asynchroniczne zadania i zoptymalizowane eventy.

---

## 📋 Komendy

### Komendy dla Graczy (`/dzialka`)
-   `/dzialka stworz <nazwa>` - Tworzy nową działkę.
-   `/dzialka panel` - Otwiera główny panel zarządzania działką, na której stoisz.
-   `/dzialka dom <nazwa>` - Teleportuje do domu Twojej działki.
-   `/dzialka informacje [nazwa]` - Wyświetla szczegółowe informacje o działce.
-   `/dzialka dodaj <gracz>` - Zaprasza gracza do działki.
-   `/dzialka wyrzuc <gracz>` - Wyrzuca gracza z działki.
-   `/dzialka usun` - Usuwa Twoją działkę (wymaga potwierdzenia).

### Komendy dla Administratorów (`/dzialkaadmin`)
-   `/dzialkaadmin bypass` - Włącza/wyłącza tryb pełnego dostępu do wszystkich działek.
-   `/dzialkaadmin panel <nazwa>` - Otwiera panel administracyjny wybranej działki.
-   `/dzialkaadmin teleport <nazwa>` - Teleportuje do wybranej działki.
-   `/dzialkaadmin przedluz <nazwa> <czas>` - Przedłuża ważność działki (np. `30d`, `12h`).
-   `/dzialkaadmin usun <nazwa>` - Usuwa działkę (wymaga potwierdzenia).
-   `/dzialkaadmin zmiennazwe <stara> <nowa>` - Zmienia nazwę działki.

### Główna Komenda (`/zenithplots` lub `/zp`)
-   `/zenithplots reload` - Przeładowuje wszystkie pliki konfiguracyjne.
-   `/zenithplots about` - Wyświetla informacje o pluginie.

---

## 🛠️ Instalacja i Konfiguracja

1.  Pobierz najnowszą wersję pluginu z sekcji [Releases](https://github.com/skunkyy/ZenithPlots/releases).
2.  Umieść plik `ZenithPlots-1.0.jar` w folderze `plugins/` na swoim serwerze.
3.  Upewnij się, że masz zainstalowane zależności: **Vault** oraz plugin ekonomii (np. EssentialsX).
4.  Uruchom serwer, aby wygenerować domyślne pliki konfiguracyjne.
5.  Dostosuj pliki `config.yml`, `messages.yml`, `roles.yml` oraz pliki w folderze `guis/` do swoich potrzeb.
6.  Użyj komendy `/zenithplots reload`, aby zastosować zmiany.

---

## 🤝 Wsparcie i Społeczność

Masz pomysł na nową funkcję, znalazłeś błąd lub po prostu chcesz porozmawiać? Dołącz do naszego serwera Discord!

**[Dołącz do naszego Discorda!](https://discord.gg/kiedys)**

---
<div align="center">
  <em>Stworzone z ❤️ przez **skunkyy**</em>
</div>
