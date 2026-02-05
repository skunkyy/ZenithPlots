<div align="center">

<img src="https://i.imgur.com/kFY5DFI.png" alt="ZenithPlots Banner" width="1000"/>

# ✨ ZenithPlots ✨
### _Nowoczesny, w pełni konfigurowalny system działek dla serwerów Minecraft 1.21+_

**ZenithPlots** to zaawansowany plugin, który przekształca zarządzanie działkami w intuicyjne i potężne doświadczenie. Stworzony z myślą o serwerach Survival, RPG i Freebuild, oferuje graczom pełną kontrolę nad swoimi terenami za pomocą estetycznych menu GUI, a administratorom daje niezrównane narzędzia do moderacji i konfiguracji.

<p align="center">
  <img src="https://img.shields.io/badge/Java-21-blue?style=for-the-badge&logo=openjdk" alt="Java 21" />
  <img src="https://img.shields.io/badge/API-Paper_1.21+-orange?style=for-the-badge" alt="Paper 1.21+" />
  <img src="https://img.shields.io/badge/Wersja-1.0-brightgreen?style=for-the-badge" alt="Version 1.0" />
</p>

</div>

---

## 🌟 Dlaczego ZenithPlots?

ZenithPlots został zaprojektowany od podstaw, aby rozwiązać problemy starszych systemów działek. Naszym celem było stworzenie pluginu, który jest jednocześnie **potężny** dla administratorów i **prosty w obsłudze** dla graczy.

-   **🎮 Skupiony na Graczu:** Wszystkie kluczowe funkcje są dostępne przez interaktywne menu GUI. Koniec z zapamiętywaniem dziesiątek skomplikowanych komend.
-   **🔧 Totalna Konfiguracja:** Każdy aspekt pluginu, od wiadomości po wygląd GUI i scoreboardu, może być zmieniony. Dostosuj ZenithPlots idealnie do swojego serwera.
-   **⚡ Zbudowany dla Wydajności:** Asynchroniczne operacje (zapis, skanowanie terenu), inteligentne cache'owanie chunków i zoptymalizowane listenery zapewniają minimalny wpływ na wydajność serwera.

---

## 🚀 Główne Funkcje

| Funkcja                        | Opis                                                                                                                                              |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| **💎 Intuicyjne GUI**          | Prawie wszystkie akcje wykonuje się w estetycznych i w 100% konfigurowalnych menu, zaprojektowanych z dbałością o detale.                           |
| **🛡️ Zaawansowana Ochrona**    | Wielowarstwowy system ochrony przed griefingiem, wybuchami, PvP (blokada ataku z bezpiecznej strefy) oraz spamem miksturami.                       |
| **👑 System Ról i Uprawnień**  | Przypisuj role (`Współwłaściciel`, `Zaufany`, `Członek`) i deleguj zadania.                                                                        |
| **✏️ Edytor Uprawnień w Grze** | Właściciele działek mogą dostosować **każdą** z ponad 40 permisji dla każdej roli, tworząc unikalne zestawy uprawnień bez edycji plików.            |
| **📈 Ulepszenia Działki**       | Rozwijaj swoją działkę, kupując kolejne poziomy ulepszeń dla rozmiaru, limitu lejów, spawnerów, członków, efektów (Haste, Fly) i wielu innych.     |
| **🏆 Rankingi Działek**         | Wbudowany, asynchroniczny system rankingów oparty na wartości postawionych bloków. Motywuje do rywalizacji i promuje najlepsze budowle.            |
| **📊 Dedykowany Scoreboard**    | Automatyczny scoreboard wyświetlany po wejściu na działkę (wymaga pluginu TAB), pokazujący statystyki, właściciela i czas wygaśnięcia.             |
| **🕊️ Latanie na Działce**       | Możliwość włączenia trybu latania (`/dzialka fly`) wyłącznie na terenie własnej działki.                                                           |
| **⏳ System Wygasania**         | Działki mają datę ważności, którą można przedłużać, co zapobiega powstawaniu opuszczonych i zaniedbanych terenów.                                 |
| **🔮 Konfigurowalny Border**   | Włącz wizualny border z cząsteczek, aby oznaczyć granice swojej działki i wybierz jego kolor w GUI.                                                 |
| **🔔 Alarm Wejścia**            | Otrzymuj powiadomienia na czacie (lub Title/Actionbar), gdy obcy gracz wejdzie na Twoją działkę.                                                    |
| **🌐 Integracje**               | Pełne wsparcie dla **Vault**, **PlaceholderAPI**, **WorldGuard**, **TAB**, **DecentHolograms/FancyHolograms** oraz **ZenithCombatLog**.             |
| **💾 Wsparcie dla Baz Danych**   | Wybierz między lekkim **SQLite** (domyślnie) a potężnym **MariaDB/MySQL** dla większych serwerów.                                                  |
| **🕶️ Tryb Bypass dla Admina**   | Administratorzy mogą swobodnie zarządzać każdą działką bez ograniczeń, wchodzić w tryb budowania i ignorować blokady.                              |

---

## 📋 Komendy i Uprawnienia

### Gracze (`zenithplots.player`)
-   `/dzialka stworz <nazwa>` - Tworzy nową działkę (`.create`).
-   `/dzialka panel` - Otwiera główny panel zarządzania (`.panel`).
-   `/dzialka dom` - Teleportuje do własnej działki (`.home`).
-   `/dzialka odwiedz <nazwa>` - Teleportuje do działki, której jesteś członkiem (`.visit`).
-   `/dzialka informacje [nazwa]` - Wyświetla sformatowane informacje o działce (`.info`).
-   `/dzialka ranking` - Wyświetla globalny ranking działek (`.ranking`).
-   `/dzialka przelicz` - Ręcznie przelicza punkty rankingu Twojej działki (`.recalculate`).
-   `/dzialka bloki` - Wyświetla listę wartości bloków w rankingu (`.blocks`).
-   `/dzialka latanie` (alias `fly`) - Włącza/wyłącza latanie na działce (`.fly`).
-   `/dzialka dodaj <gracz>` - Zaprasza gracza do działki (`.add`).
-   `/dzialka akceptuj` - Akceptuje zaproszenie.
-   `/dzialka odrzuc` - Odrzuca zaproszenie.
-   `/dzialka wyrzuc <gracz>` - Wyrzuca gracza z działki (`.kick`).
-   `/dzialka zablokuj <gracz>` - Blokuje graczowi wstęp na działkę.
-   `/dzialka odblokuj <gracz>` - Odblokowuje gracza.
-   `/dzialka ustawdom` - Zmienia punkt teleportacji (`.sethome`).
-   `/dzialka usun` - Usuwa Twoją działkę (`.delete`).
-   `/dzialka zmiennazwe <nowa_nazwa>` - Zmienia nazwę działki.

*Uprawnienia do komend gracza: `zenithplots.command.player.<subkomenda>`*

### Administratorzy (`zenithplots.admin`)
-   `/dzialkaadmin bypass` - Włącza/wyłącza tryb pełnego dostępu (budowanie wszędzie, ignorowanie blokad).
-   `/dzialkaadmin panel <nazwa>` - Otwiera panel administracyjny dowolnej działki.
-   `/dzialkaadmin info <nazwa>` - Wyświetla szczegółowe, techniczne informacje o działce.
-   `/dzialkaadmin lookup <gracz>` - Sprawdza listę działek gracza (właściciel/członek).
-   `/dzialkaadmin setowner <nazwa> <gracz>` - Przenosi własność działki na innego gracza.
-   `/dzialkaadmin teleport <nazwa>` - Teleportuje do działki.
-   `/dzialkaadmin teleportwlasciciel <gracz>` - Teleportuje do działki danego gracza.
-   `/dzialkaadmin fly` - Włącza latanie administratora na dowolnej działce.
-   `/dzialkaadmin przelicz <nazwa|*>` - Wymusza przeliczenie rankingu dla działki lub wszystkich.
-   `/dzialkaadmin przedluz <nazwa> <czas>` - Przedłuża ważność działki.
-   `/dzialkaadmin usun <nazwa>` - Natychmiastowo usuwa działkę (z bazy i mapy).
-   `/dzialkaadmin dodaj <nazwa> <gracz>` - Wymusza dodanie gracza.
-   `/dzialkaadmin wyrzuc <nazwa> <gracz>` - Wymusza wyrzucenie gracza.
-   `/dzialkaadmin ulepszenia <nazwa> <typ> set <poziom>` - Ustawia poziom ulepszenia.
-   `/dzialkaadmin zmiennazwe <stara> <nowa>` - Zmienia nazwę działki.

*Główne uprawnienie do komend admina: `zenithplots.command.admin`*

### Zarządzanie Pluginem
-   `/zenithplots reload` - Przeładowuje wszystkie konfiguracje i odświeża cache (`.manage`).

*Uprawnienie: `zenithplots.command.admin.manage`*

---

## 🛠️ Instalacja i Konfiguracja

1.  Pobierz najnowszą wersję pluginu z sekcji **[Releases](https://github.com/skunkyy/ZenithPlots/releases)**.
2.  Umieść plik `ZenithPlots-1.0.jar` w folderze `plugins/` na swoim serwerze.
3.  **Upewnij się, że masz zainstalowane wymagane zależności:**
    -   ✅ **[Vault](https://www.spigotmc.org/resources/vault.34315/)**
    -   ✅ Dowolny plugin ekonomii (np. EssentialsX, CMI, TheNewEconomy)
4.  Dla pełnej funkcjonalności **zainstaluj zalecane zależności**:
    -   ⭐ **[PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/)** (Dla placeholderów)
    -   ⭐ **[TAB](https://github.com/NEZNAMY/TAB)** (Dla dedykowanego scoreboardu na działkach)
    -   ⭐ **[DecentHolograms](https://www.spigotmc.org/resources/decentholograms-1-8-1-20-4-papi-support-no-dependencies.96927/)** lub **FancyHolograms** (Dla hologramów nad działką)
    -   ⭐ **[WorldGuard](https://dev.bukkit.org/projects/worldguard)** (Dla blokowania tworzenia działek w regionach)
5.  Uruchom serwer, aby wygenerować domyślne pliki konfiguracyjne.
6.  Dostosuj pliki `config.yml`, `messages.yml`, `roles.yml`, `upgrades.yml`, `ranking.yml` oraz pliki GUI w folderze `guis/` do swoich potrzeb.
7.  Użyj komendy `/zenithplots reload`, aby zastosować zmiany.

---

## 🤝 Wsparcie i Społeczność

Masz pomysł na nową funkcję, znalazłeś błąd lub po prostu chcesz porozmawiać? Dołącz do naszego serwera Discord!

---
<div align="center">
  <em>Stworzone z ❤️ przez **skunky**</em>
</div>
