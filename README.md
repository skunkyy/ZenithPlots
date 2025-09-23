<div align="center">

<img src="https://i.imgur.com/kFY5DFI.png" alt="ZenithPlots Banner" width="1000"/>

# ✨ ZenithPlots ✨
### _Nowoczesny, w pełni konfigurowalny system działek dla serwerów Minecraft 1.21+_

**ZenithPlots** to zaawansowany plugin, który przekształca zarządzanie działkami w intuicyjne i potężne doświadczenie. Stworzony z myślą o serwerach Survival, RPG, oferuje graczom pełną kontrolę nad swoimi terenami za pomocą estetycznych menu GUI, a administratorom daje niezrównane narzędzia do moderacji i konfiguracji.

<p align="center">
  <img src="https://img.shields.io/badge/Java-21-blue?style=for-the-badge&logo=openjdk" alt="Java 21" />
  <img src="https://img.shields.io/badge/API-Paper_1.21+-orange?style=for-the-badge" alt="Paper 1.21+" />
  <img src="https://img.shields.io/badge/Wersja-1.0-brightgreen?style=for-the-badge" alt="Version 1.0" />
</p>

</div>

---

## 🌟 Dlaczego ZenithPlots?

ZenithPlots został zaprojektowany od podstaw, aby rozwiązać problemy starszych systemów działek. Naszym celem było stworzenie pluginu, który jest jednocześnie **potężny** dla administratorów i **prosty w obsłudze** dla graczy.

-   **🎮 Skupiony na Graczu:** Wszystkie kluczowe funkcje są dostępne przez interaktywne menu. Koniec z zapamiętywaniem dziesiątek skomplikowanych komend.
-   **🔧 Totalna Konfiguracja:** Każdy aspekt pluginu, od wiadomości po wygląd GUI, może być zmieniony. Dostosuj ZenithPlots idealnie do swojego serwera.
-   **⚡ Zbudowany dla Wydajności:** Asynchroniczne operacje, inteligentne cache'owanie i zoptymalizowane listenery zapewniają minimalny wpływ na wydajność serwera.

---

## 🚀 Główne Funkcje

| Funkcja                        | Opis                                                                                                                                              |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| **💎 Intuicyjne GUI**          | Prawie wszystkie akcje wykonuje się w estetycznych i w 100% konfigurowalnych menu, zaprojektowanych z dbałością o detale.                           |
| **🛡️ System Ról i Uprawnień**  | Przypisuj role (`Współwłaściciel`, `Moderator` itp.) i deleguj zadania.                                                                              |
| **✏️ Edytor Uprawnień w Grze** | Właściciele działek mogą dostosować **każdą** z ponad 40 permisji dla każdej roli, tworząc unikalne zestawy uprawnień bez edycji plików.            |
| **📈 Ulepszenia Działki**       | Rozwijaj swoją działkę, kupując kolejne poziomy ulepszeń dla rozmiaru, limitu skrzyń, lejów, spawnerów i członków.                                 |
| **💰 Bank Działki**             | Wspólny skarbiec, do którego członkowie mogą wpłacać środki na rozwój i utrzymanie działki.                                                       |
| **🏆 Rankingi Działek**         | Wbudowany, asynchroniczny system rankingów (np. najbogatszych działek) motywuje do rywalizacji i promuje najlepsze budowle na serwerze.              |
| **⏳ System Wygasania**         | Działki mają datę ważności, którą można przedłużać, co zapobiega powstawaniu opuszczonych i zaniedbanych terenów.                                 |
| **🔮 Konfigurowalny Border**   | Włącz wizualny border z cząsteczek, aby oznaczyć granice swojej działki i wybierz jego kolor.                                                       |
| **🔔 Alarm Wejścia**            | Otrzymuj powiadomienia na czacie, gdy obcy gracz wejdzie na Twoją działkę.                                                                          |
| **🌐 Integracje**               | Pełne wsparcie dla **Vault**, **PlaceholderAPI** i **WorldGuard**.                                                                                  |
| **💾 Wsparcie dla Baz Danych**   | Wybierz między lekkim **SQLite** a potężnym **MariaDB/MySQL** dla większych serwerów.                                                              |
| **🕶️ Tryb Bypass dla Admina**   | Administratorzy mogą swobodnie zarządzać każdą działką bez ograniczeń.                                                                            |

---

## 📋 Komendy i Uprawnienia

### Gracze (`zenithplots.player`)
-   `/dzialka stworz <nazwa>` - Tworzy nową działkę (`.create`).
-   `/dzialka panel` - Otwiera główny panel zarządzania (`.panel`).
-   `/dzialka dom <nazwa>` - Teleportuje do domu działki (`.home`).
-   `/dzialka informacje [nazwa]` - Wyświetla szczegółowe informacje (`.info`).
-   `/dzialka ranking` - Wyświetla rankingi działek (`.ranking`).
-   `/dzialka dodaj <gracz>` - Zaprasza gracza do działki (`.add`).
-   `/dzialka wyrzuc <gracz>` - Wyrzuca gracza z działki (`.kick`).
-   `/dzialka usun` - Usuwa Twoją działkę (`.delete`).
-   `/dzialka zmiennazwe <nowa_nazwa>` - Zmienia nazwę działki (wymaga uprawnienia wewnątrz działki).

*Uprawnienia do komend gracza: `zenithplots.command.player.<subkomenda>`*

### Administratorzy (`zenithplots.admin`)
-   `/dzialkaadmin bypass` - Włącza/wyłącza tryb bypass.
-   `/dzialkaadmin panel <nazwa>` - Otwiera panel administracyjny działki.
-   `/dzialkaadmin teleport <nazwa>` - Teleportuje do działki.
-   `/dzialkaadmin przedluz <nazwa> <czas>` - Przedłuża ważność działki.
-   `/dzialkaadmin usun <nazwa>` - Natychmiastowo usuwa działkę.
-   `/dzialkaadmin ulepszenia <nazwa> <typ> set <poziom>` - Ustawia poziom ulepszenia.
-   `/dzialkaadmin zmiennazwe <stara> <nowa>` - Zmienia nazwę działki.

*Główne uprawnienie do komend admina: `zenithplots.command.admin`*

### Zarządzanie Pluginem
-   `/zenithplots reload` - Przeładowuje wszystkie konfiguracje (`.manage`).
-   `/zenithplots about` - Informacje o pluginie (`.manage`).

*Uprawnienie: `zenithplots.command.admin.manage`*

---

## 🛠️ Instalacja i Konfiguracja

1.  Pobierz najnowszą wersję pluginu z sekcji **[Releases](https://github.com/skunkyy/ZenithPlots/releases)**.
2.  Umieść plik `ZenithPlots-1.0.jar` w folderze `plugins/` na swoim serwerze.
3.  **Upewnij się, że masz zainstalowane wymagane zależności:**
    -   ✅ **[Vault](https://www.spigotmc.org/resources/vault.34315/)**
    -   ✅ Dowolny plugin ekonomii (np. EssentialsX, CMI)
4.  Dla pełnej funkcjonalności **zainstaluj opcjonalne zależności**:
    -   ⭐ **[PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/)**
    -   ⭐ **[WorldGuard](https://dev.bukkit.org/projects/worldguard)**
5.  Uruchom serwer, aby wygenerować domyślne pliki konfiguracyjne.
6.  Dostosuj pliki `config.yml`, `messages.yml`, `roles.yml`, `upgrades.yml` oraz pliki w folderze `guis/` do swoich potrzeb.
7.  Użyj komendy `/zenithplots reload`, aby zastosować zmiany.

---

## 🤝 Wsparcie i Społeczność

Masz pomysł na nową funkcję, znalazłeś błąd lub po prostu chcesz porozmawiać? Dołącz do naszego serwera Discord!

---
<div align="center">
  <em>Stworzone z ❤️ przez **skunky**</em>
</div>
