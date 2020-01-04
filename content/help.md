# Gdzie są teraz historyczne dane?

W dwóch miejscach:

  * Wcześniejsze wydarzenie na <a href="https://sites.google.com/site/agilewarsaw/" target="_blank">Google Sites </a>
  * Późniejsze na <a href="https://www.meetup.com/AgileWarsaw/events/past/" target="_blank"> Meetup.com </a>

## Które wydarzenia są już dodane?

Zajrzyj tutaj na [events](/events)

# Jak dodać wydarzenie?

## Najprostszy sposób:

Najprostszy dla Ciebie sposób to przesłanie nam wypełnionej formatki wydarzenia i ewentualnie zdjęć czy innych plików, które przynależą do spotkania.

   * Formatka (zwyły tekst) znajduje się <a href="https://raw.githubusercontent.com/AgileWarsaw/netlify/devel-www/themes/agilewarsaw/archetypes/event.md" target="_blank">tutaj</a>.

   * Wypełnij informacje o wydarzeniu według wskazówek w formatce.

   * Prześlij nam wypełnioną formatkę i pliki.

## Przez github:

Jeśli nie boisz się GitHub-a albo chcesz spróbować z niego skorzystać możesz zaoszczdzić nam (organizatorom) pracy samodzielnie dołączając informacje do tej strony.

### TODO: opisać jak stworzyć wydarzenie posługując się tylko stroną GitHub.

## Wersja idealna czyli wszystko sprawdzone przez Ciebie:

Potrzebny Ci będzie klient Git, żeby móc pracować na lokalnych plikach oraz `Hugo` czyli program, który generuje tę stronę z danych.

Instalacja Hugo jest <a href="https://gohugo.io/getting-started/installing#quick-install" target="_blank">prosta na każdym systemie operacyjnym</a>. Możesz nawet ściągnąć jeden plik wykonywalny i użyć go bez instalacji.

1. Sklonuj lokalnie repozytorium `https://github.com/AgileWarsaw/netlify.git`

1. Sprawdź, czy jesteś na branch-u `?`

1. Sprawdź numer wydarzenia, które chcesz dodać.

2. W terminalu w folderze repozytorium wpisz:  
   `hugo new events/NUMER/index.md -k event`  
   zamieniająć `NUMER` na właściwy numer wydarzenia.

3. Program stworzy nowy podkatalog `NUMER` w katalogu `content` a w nim formatkę wydarzenia.

4. Wypełnij formatkę.

5. Jeśli chcesz dołączyć dodatkowe pliki umieść je w tym samym katalogu.  
   Zdjęcie pod nazwą `hero.jpg` zostanie użyte jako "wizytówka" wydarzenia.

6. W terminalu wpisz:  
   `hugo server --watch`  
   i w przeglądarce (zwykle pod adresem `http://localhost:1313`) będziesz mógł przejrzeć stronę z Twoimi zmianami.

7. Jeśli wszystko jest dobrze, stwórz `pull request`.