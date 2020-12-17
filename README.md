# FiveM_Roleplay_Pack
Cześć. Publikuję pakiet skryptów na serwer FiveM RolePlay. Jest przerobiony przeze mnie. Pakiet jest dobrze zoptymalizowany. Jest wiele interesujących skryptów, samochodów, wnętrz, kostiumów i wiele więcej. Wszystko jest gotowe do działania. Przesyłam ci również poradnik, jak zmienić sobie nazwy w skryptach

# Jak uruchomić serwer
- Nie będę pisał o uruchamianiu artefaktów itp. W internecie jest tego sporo, np. Na fivem forum i youtube.

1. Jeśli masz już artefakty i wszystko jest skonfigurowane do przesyłania pakietu, pobierz mój pakiet i prześlij go do folderu cfx-server-data.
2. Wpisz server.cfg i skonfiguruj:
- przejdź do server.cfg i odpowiednio uzupełnij linie. Powyżej opisałeś, co jest z czego
3. Po utworzeniu server.cfg możesz początkowo uruchomić serwer. Dowiedz się co i jak, sprawdź, czy wszystko Ci się podoba. Po jakimś czasie zapewne zauważysz, że na przykład w kluczykach samochodu wyświetla się napis „YOURSERVER”. Możesz to zmienić, na przykład nazwę serwera. W kolejnych wierszach dowiesz się, które skrypty wymagają tego ustawienia

# Nazwa serwera
1. Tutaj się dowiesz jak zmieniać kolor czcionki w nazwie serwera. Niestety do tego potrzebujesz minimum patrona agrumentum: https://forum.cfx.re/t/how-to-change-your-servernames-color/200

# Startowanie zasobów
- Aby wystartować zasób wpisujemy start/ensure (nazwa skryptu) | Przykład: start EasyAdmin
- Pamiętaj aby dobrze wpisać wszystkie znaki
- Osobiście polecam zachować porządek w plikach. Zawsze dopisuj startowanie zasobu w odpowiedniej kategorii np. #prace#

# Status na discordzie
Aby zmienić status na discordzie podczas grania na twoim serwerze, Musisz wejść do /[detale]/discord/client.lua
1. Zmieniamy tam client ID naszego discord APP (linijka SetDiscordAppId)
2. Zmieniamy nazwe tekstu który będzie się wyświetlał po najechaniu na duże logo (np. nazwa serwera) SetDiscordRichPresenceAssetText
3. Zmieniamy nazwe tekstu który będzie się wyświetlał po najechaniu na małe logo (np. discord serwera) SetDiscordRichPresenceAssetSmallText
4. Zmieniamy nazwę zdjęcia który będzie dużym logiem SetDiscordRichPresenceAssetText
5. Zmieniamy nazwę zdjęcia który będzie małym logiem SetDiscordRichPresenceAssetSmall

# Jak stworzyć discord APP do statusu?
- Wchodzimy na https://discord.com/developers/applications
- Logujemy się
- Tworzymy aplikację o nazwie np. Nazwa serwera
- Klikamy na utworzoną aplikację
- Kopiujemy Client ID i dajemy w linijke która jest opisane w #status na discordzie 1.
- Klikamy po lewej w Rich Presence
- Pod Rich Presence Assets dodajemy dwa zdjęcia w odpowiednich rozmiarach. Nazywamy je tak jak w #status na discordzie 2. oraz 3.
- Gotowe
