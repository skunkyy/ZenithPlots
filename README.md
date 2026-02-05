<div align="center">

<img src="https://i.imgur.com/kFY5DFI.png" alt="ZenithPlots Banner" width="1000"/>

# ✨ ZenithPlots ✨
### _Definicja nowoczesnego systemu działek dla serwerów Minecraft 1.21+_

![Java](https://img.shields.io/badge/Java-21-blue?style=for-the-badge&logo=openjdk)
![Platform](https://img.shields.io/badge/Platform-Paper%201.21+-orange?style=for-the-badge&logo=spigotmc)
![Version](https://img.shields.io/badge/Wersja-1.0-brightgreen?style=for-the-badge)
![Database](https://img.shields.io/badge/Baza-SQLite%20%7C%20MariaDB-lightgrey?style=for-the-badge&logo=mysql)

</div>

---

## 👋 O co chodzi z ZenithPlots?

Wyobraź sobie system działek, który nie irytuje graczy, a administratorom daje spokój ducha. **ZenithPlots** to nie jest kolejny fork starego pluginu. To napisany od zera silnik, który stawia na **wydajność** (działa asynchronicznie), **estetykę** (wszystko w GUI) i **elastyczność**.

Nieważne, czy robisz serwer Survival, Freebuild czy RPG – ten plugin daje graczom kawałek świata, nad którym mają pełną kontrolę, a Ty masz pewność, że nikt tego nie zepsuje.

---

## 🔥 Dlaczego pokochasz ten plugin?

### 💎 Dla Graczy (User Experience)
*   **Koniec z komendami:** Zapomnij o `/plot flag set pvp true`. Gracz wpisuje `/dzialka panel` i ma wszystko pod ręką w pięknym menu.
*   **Inteligentny Scoreboard:** Wchodzisz na działkę? Scoreboard zmienia się automatycznie, pokazując kto jest właścicielem, ile ma punktów i kiedy działka wygasa. Wychodzisz? Wraca stary scoreboard (dzięki integracji z TAB).
*   **System Ulepszeń:** Działka to nie tylko teren. To inwestycja. Gracze wydają pieniądze na powiększanie terenu, limity hopperów, spawnerów, a nawet efekty takie jak Haste czy Fly.
*   **Latanie:** Tak, gracz może latać, ale **tylko** nad swoją działką. Wyleci poza nią? Fly się wyłącza. Proste i uczciwe.

### 🛡️ Dla Adminów (Security & Performance)
*   **Pancerna Ochrona:**
    *   **Anti-Potion Spam:** Nasz autorski system "Obrony Przeciwlotniczej" usuwa wrogie mikstury rzucone z zewnątrz jeszcze w powietrzu. Żadnego trucia graczy na spawnie czy zza granicy działki.
    *   **Blokada Tłoków & Redstone:** Maszyny lagujące serwer? Nie tutaj. Limity bloków redstone są ściśle przestrzegane.
    *   **PvP Control:** Walka jest możliwa tylko w dziczy. Jeśli ktokolwiek (atakujący lub ofiara) stoi na działce – obrażenia są anulowane.
*   **Asynchroniczność:** Zapisywanie działek do bazy (SQLite/MySQL), skanowanie terenu przy zakładaniu działki, przeliczanie rankingu – to wszystko dzieje się w tle. Zero lagów przy autosave.
*   **Pełna Kontrola:** Komendy `/dzialkaadmin` pozwalają Ci na wszystko – od zmiany właściciela, przez edycję ulepszeń, aż po "teleportację właściciela" do Ciebie.

---

## 🚀 Szczegółowy Opis Funkcji

### 🏆 System Rankingowy (Topki)
To nie jest zwykły licznik. ZenithPlots skanuje bloki na działce i przyznaje punkty.
*   **Konfigurowalne wartości:** Ty ustalasz, że `DIAMOND_BLOCK` daje 100 pkt, a `BEACON` 1000 pkt.
*   **Poziomy:** Punkty przekładają się na poziom działki.
*   **Asynchroniczne przeliczanie:** Gracz wpisuje `/dzialka przelicz` i dostaje raport: *"Twój poziom wzrósł z 5 na 6! (Awans)"*.
*   **Placeholdery:** Wyświetl topkę na spawnie używając PlaceholderAPI.

### 👥 Zaawansowane Zarządzanie Członkami
Właściciel działki to nie jedyna osoba. Mamy role:
1.  **Właściciel** (Pełna władza)
2.  **Współwłaściciel** (Prawie pełna władza)
3.  **Zaufany** (Budowanie, ale bez zarządzania)
4.  **Członek** (Podstawowe akcje)
5.  **Odwiedzający** (Tylko zwiedzanie)

Co najlepsze? **Właściciel może edytować uprawnienia każdej roli w grze!** Chcesz, żeby Zaufany mógł wyrzucać innych? Klikasz w GUI i gotowe.

### 🔮 Wizualizacje (Hologramy i Bordery)
*   **Hologramy:** Nad centrum działki (blokiem serca) unosi się hologram ze statystykami. Wspieramy **DecentHolograms** i **FancyHolograms**.
*   **Border:** Gracz może włączyć wizualizację granic swojej działki. Cząsteczki (particles) pokażą mu dokładnie, dokąd sięga jego teren. Kolor bordera? Też do wyboru w GUI!

### ⏳ System Wygasania
Działki nie są wieczne.
*   Każda działka ma czas życia (np. 30 dni).
*   Właściciel musi wejść w panel i opłacić przedłużenie.
*   Jeśli zapomni? Działka wygasa, blok serca znika, a teren wraca do puli wolnych (lub zostaje wyczyszczony - zależy od Ciebie).
*   **Powiadomienia:** Gracze dostają ostrzeżenia, gdy ich działka jest bliska wygaśnięcia.

---

## 💻 Komendy

<details>
<summary><b>Dla Graczy (Kliknij, aby rozwinąć)</b></summary>

| Komenda | Opis |
| :--- | :--- |
| `/dzialka stworz <nazwa>` | Tworzy nową działkę w miejscu, w którym stoisz. |
| `/dzialka panel` | Otwiera główne centrum dowodzenia działką. |
| `/dzialka dom` | Teleportuje Cię bezpiecznie do Twojej działki. |
| `/dzialka odwiedz <nazwa>` | Odwiedź działkę znajomego (jeśli jesteś dodany). |
| `/dzialka informacje [nazwa]` | Pokazuje techniczne dane (rozmiar, wygasanie, ID). |
| `/dzialka ranking` | Wyświetla topkę najlepszych działek. |
| `/dzialka przelicz` | Przelicza punkty Twojej działki (z cooldownem). |
| `/dzialka bloki` | Lista bloków, które dają punkty do rankingu. |
| `/dzialka latanie` | Włącz/wyłącz latanie na swoim terenie. |
| `/dzialka dodaj <gracz>` | Wyślij zaproszenie do innego gracza. |
| `/dzialka akceptuj/odrzuc` | Reakcja na zaproszenie. |
| `/dzialka wyrzuc <gracz>` | Usuń gracza z listy członków. |
| `/dzialka zablokuj <gracz>` | Zbanuj gracza na swojej działce (nie wejdzie). |
| `/dzialka odblokuj <gracz>` | Zdejmij bana. |
| `/dzialka ustawdom` | Zmień miejsce teleportu `/dzialka dom`. |
| `/dzialka zmiennazwe <nowa>` | Zmień nazwę swojej działki (kosztuje!). |
| `/dzialka usun` | Usuń swoją działkę na zawsze. |

</details>

<details>
<summary><b>Dla Administratora (Kliknij, aby rozwinąć)</b></summary>

| Komenda | Opis |
| :--- | :--- |
| `/dzialkaadmin bypass` | **Tryb Boga:** Buduj, niszcz i otwieraj skrzynie na cudzych działkach. |
| `/dzialkaadmin panel <nazwa>` | Otwórz panel zarządzania czyjejś działki. |
| `/dzialkaadmin info <nazwa>` | Pełne dane techniczne (UUID, dokładne koordynaty, poziomy ulepszeń). |
| `/dzialkaadmin lookup <gracz>` | Zobacz, jakie działki ma dany gracz (i gdzie jest członkiem). |
| `/dzialkaadmin setowner <działka> <gracz>` | Przenieś własność działki na kogoś innego. |
| `/dzialkaadmin teleport <nazwa>` | Teleport do działki. |
| `/dzialkaadmin teleportwlasciciel <gracz>` | Teleport do działki danego gracza. |
| `/dzialkaadmin fly` | Włącz latanie admina na dowolnej działce (omija zasady). |
| `/dzialkaadmin przelicz <nazwa|*>` | Wymuś przeliczenie rankingu dla jednej lub wszystkich działek. |
| `/dzialkaadmin przedluz <nazwa> <czas>` | Dodaj czas życia działce (np. `30d`). |
| `/dzialkaadmin ulepszenia <nazwa> <typ> set <poziom>` | Ręcznie ustaw poziom ulepszenia. |
| `/dzialkaadmin usun <nazwa>` | Usuń działkę gracza (z bazy i hologramu). |
| `/dzialkaadmin dodaj/wyrzuc` | Zarządzaj członkami cudzych działek. |
| `/zenithplots reload` | Przeładuj wszystkie pliki konfiguracyjne. |

</details>

---

## 🛠️ Instalacja i Wymagania

### 📦 Wymagane Pluginy
Bez tego nie ruszymy:
1.  **[Vault](https://www.spigotmc.org/resources/vault.34315/)** - Do obsługi ekonomii i uprawnień.
2.  **Plugin Ekonomii** - Np. *EssentialsX*, *CMI*, *TheNewEconomy*. (Działki kosztują!).

### 🧩 Zalecane (Dla pełnego efektu)
1.  **[PlaceholderAPI](https://www.spigotmc.org/resources/placeholderapi.6245/)** - Żeby wyświetlać dane na chacie/scoreboardzie.
2.  **[TAB](https://github.com/NEZNAMY/TAB)** - Aby działał nasz **dedykowany scoreboard działkowy**.
3.  **[WorldGuard](https://dev.bukkit.org/projects/worldguard)** - Aby zablokować tworzenie działek na spawnie.
4.  **[DecentHolograms](https://www.spigotmc.org/resources/96927/)** lub **FancyHolograms** - Do wyświetlania statystyk nad działką.
5.  **[ZenithCombatLog](https://github.com/skunkyy/ZenithCombatLog)** (lub inny kompatybilny) - Do blokowania ucieczki na działkę podczas walki.

### ⚙️ Instrukcja
1.  Pobierz `ZenithPlots-1.0.jar`.
2.  Wrzuć do folderu `/plugins`.
3.  Zrestartuj serwer.
4.  (Opcjonalnie) Skonfiguruj połączenie z bazą danych w `config.yml` (domyślnie SQLite - plik lokalny).
5.  Edytuj `messages.yml`, `upgrades.yml` i pliki GUI według własnego uznania.
6.  Wpisz `/zenithplots reload`. Gotowe!

---

## 📂 Pliki Konfiguracyjne

Plugin generuje bogate pliki konfiguracyjne:
*   `config.yml` - Główne ustawienia (baza danych, limity, koszty).
*   `messages.yml` - **Każda** wiadomość jest do przetłumaczenia.
*   `roles.yml` - Definicje ról i ich domyślnych uprawnień.
*   `ranking.yml` - Wartości punktowe bloków i wzór na poziomy.
*   `upgrades.yml` - Koszty i wartości dla każdego poziomu ulepszeń.
*   `guis/*.yml` - Wygląd każdego menu (itemy, sloty, nazwy, lore).

---

## 📊 Placeholdery (PAPI)

Chcesz użyć danych z pluginu na scoreboardzie, tabliście lub chacie? Proszę bardzo:

| Placeholder | Opis |
| :--- | :--- |
| `%zenithplots_current_plot_name%` | Nazwa działki, na której stoisz. |
| `%zenithplots_current_plot_owner%` | Właściciel działki, na której stoisz. |
| `%zenithplots_current_plot_level%` | Poziom działki. |
| `%zenithplots_current_plot_points%` | Punkty rankingu. |
| `%zenithplots_current_plot_expire_timeleft%` | Czas do wygaśnięcia (np. "2d 4h"). |
| `%zenithplots_current_plot_size_formatted%` | Rozmiar działki (np. "32x32"). |
| `%zenithplots_current_plot_members_current%` | Liczba członków. |
| `%zenithplots_owned_plot_name%` | Nazwa Twojej działki (gdziekolwiek jesteś). |
| `%zenithplots_ranking_1_name%` | Nazwa działki TOP 1. |
| `%zenithplots_ranking_1_owner%` | Właściciel działki TOP 1. |
| `%zenithplots_plot_count%` | Ile działek posiadasz. |

---

<div align="center">

**Projekt tworzony z pasją.**
Masz pomysł? Znalazłeś błąd? Pisz śmiało!

Copyright © 2026 **skunkyy**. Wszelkie prawa zastrzeżone.

</div>
