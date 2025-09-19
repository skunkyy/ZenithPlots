<div align="center">

<img src="https://i.imgur.com/kFY5DFI.png" alt="ZenithPlots Banner" width="1000"/>

# ✨ ZenithPlots ✨
### _Nowoczesny, w pełni konfigurowalny system działek dla serwerów Minecraft 1.21+_

**ZenithPlots** to zaawansowany plugin, który przekształca zarządzanie działkami w intuicyjne i potężne doświadczenie. Stworzony z myślą o serwerach Survival, RPG i Skyblock, oferuje graczom pełną kontrolę nad swoimi terenami za pomocą estetycznych menu GUI, a administratorom daje niezrównane narzędzia do moderacji i konfiguracji.

![Java](https://img.shields.io/badge/Java-21-blue?style=for-the-badge&logo=openjdk)
![API](https://img.shields.io/badge/API-Paper_1.21+-orange?style=for-the-badge)
![Wersja](https://img.shields.io/badge/Wersja-1.0-brightgreen?style=for-the-badge)

</div>

---

## 🚀 Główne Funkcje

-   **💎 Intuicyjne GUI:** Prawie wszystkie akcje wykonuje się w estetycznych i w 100% konfigurowalnych menu, zaprojektowanych z dbałością o detale.
-   **🛡️ System Ról i Uprawnień:** Przypisuj role (`Współwłaściciel`, `Moderator`, `Zaufany`, `Członek`, `Odwiedzający`) i deleguj zadania.
-   **✏️ Edytor Uprawnień w Grze:** Właściciele działek mogą dostosować **każdą** z ponad 30 permisji dla każdej roli, tworząc unikalne zestawy uprawnień bez edycji plików.
-   **📈 Ulepszenia Działki oparte na Poziomach:** Rozwijaj swoją działkę, kupując kolejne poziomy ulepszeń dla rozmiaru, limitu skrzyń, lejów, spawnerów i członków.
-   **💰 Bank Działki:** Wspólny skarbiec, do którego członkowie mogą wpłacać środki na rozwój i utrzymanie działki.
-   **⏳ System Wygasania:** Działki mają datę ważności, którą można przedłużać, co zapobiega powstawaniu opuszczonych i zaniedbanych terenów.
-   **🔮 Konfigurowalny Border:** Włącz wizualny border z cząsteczek, aby oznaczyć granice swojej działki i wybierz jego kolor.
-   **🔔 Alarm Wejścia:** Otrzymuj powiadomienia na czacie, gdy obcy gracz wejdzie na Twoją działkę.
-   **🌐 Integracja z WorldGuard:** Plugin respektuje flagi globalne (`lava-flow`, `water-flow`) i pozwala na blokowanie tworzenia działek w określonych regionach i światach.
-   **⚙️ Pełna Konfiguracja:** Dostosuj **każdą wiadomość**, wygląd **każdego menu**, koszty i wartości ulepszeń oraz zasady w plikach `.yml`.
-   **💾 Wsparcie dla Baz Danych:** Wybierz między lekkim **SQLite** (domyślnie) a potężnym **MariaDB/MySQL** dla większych serwerów.
-   **🕶️ Tryb Bypass dla Admina:** Administratorzy mogą swobodnie zarządzać każdą działką bez ograniczeń.
-   **⚡ Optymalizacja:** Plugin został napisany z myślą o wydajności, wykorzystując asynchroniczne zadania, zoptymalizowane listenery i bezpieczne operacje na bazie danych.

---

## 📋 Komendy

### Komendy dla Graczy (`/dzialka`)
-   `/dzialka stworz <nazwa>` - Tworzy nową działkę.
-   `/dzialka panel` - Otwiera główny panel zarządzania działką, na której stoisz.
-   `/dzialka dom <nazwa>` - Teleportuje do domu działki, której jesteś członkiem.
-   `/dzialka informacje [nazwa]` - Wyświetla szczegółowe informacje o działce.
-   `/dzialka dodaj <gracz>` - Zaprasza gracza online do działki (otrzymuje rolę `MEMBER`).
-   `/dzialka wyrzuc <gracz>` - Wyrzuca gracza z działki.
-   `/dzialka usun` - Usuwa Twoją działkę (wymaga potwierdzenia).

### Komendy dla Administratorów (`/dzialkaadmin`)
-   `/dzialkaadmin bypass` - Włącza/wyłącza tryb pełnego dostępu do wszystkich działek.
-   `/dzialkaadmin panel <nazwa>` - Otwiera panel administracyjny wybranej działki.
-   `/dzialkaadmin teleport <nazwa>` - Teleportuje do wybranej działki.
-   `/dzialkaadmin przedluz <nazwa> <czas>` - Przedłuża ważność działki (np. `30d`, `12h`).
-   `/dzialkaadmin usun <nazwa>` - Usuwa działkę (wymaga potwierdzenia).
-   `/dzialkaadmin ulepszenia <nazwa> <typ> set <poziom>` - Ustawia poziom ulepszenia.
-   `/dzialkaadmin zmiennazwe <stara> <nowa>` - Zmienia nazwę działki.

### Główna Komenda (`/zenithplots` lub `/zp`)
-   `/zenithplots reload` - Przeładowuje wszystkie pliki konfiguracyjne.
-   `/zenithplots about` - Wyświetla informacje o pluginie.

---

## 🔑 Uprawnienia (Permissions)

Plugin posiada szczegółowy system uprawnień, który pozwala na precyzyjną kontrolę.
-   **`zenithplots.*`** - Daje dostęp do wszystkich funkcji i komend.
-   **`zenithplots.admin`** - Daje dostęp do wszystkich komend administracyjnych.
-   **`zenithplots.admin.<komenda>`** - Daje dostęp do konkretnej subkomendy, np. `zenithplots.admin.teleport`.

---

## 🛠️ Instalacja i Konfiguracja

1.  Pobierz najnowszą wersję pluginu z sekcji [Releases](https://github.com/skunkyy/ZenithPlots/releases).
2.  Umieść plik `ZenithPlots-1.0.jar` w folderze `plugins/` na swoim serwerze.
3.  Upewnij się, że masz zainstalowane zależności: **Vault** oraz plugin ekonomii (np. EssentialsX). Dla pełnej funkcjonalności zalecany jest również **WorldGuard**.
4.  Uruchom serwer, aby wygenerować domyślne pliki konfiguracyjne.
5.  Dostosuj pliki `config.yml`, `messages.yml`, `roles.yml`, `upgrades.yml` oraz pliki w folderze `guis/` do swoich potrzeb.
6.  Użyj komendy `/zenithplots reload`, aby zastosować zmiany.

---

## 🤝 Wsparcie i Społeczność

Masz pomysł na nową funkcję, znalazłeś błąd lub po prostu chcesz porozmawiać? Dołącz do naszego serwera Discord!

**[Dołącz do naszego Discorda!](https://discord.gg/XYxj8byb8T)**

---
<div align="center">
  <em>Stworzone z ❤️ przez **skunky**</em>
</div>
