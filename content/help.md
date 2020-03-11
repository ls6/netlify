# Gdzie są teraz historyczne dane?

W dwóch miejscach:

  * Wcześniejsze wydarzenie na <a href="https://sites.google.com/site/agilewarsaw/" target="_blank">Google Sites </a>
  * Późniejsze na <a href="https://www.meetup.com/AgileWarsaw/events/past/" target="_blank"> Meetup.com </a>

## Które wydarzenia są już dodane?

Zajrzyj tutaj na [events](/events)

# Jak dodać wydarzenie?

## Najprostszy sposób:

Najprostszy dla Ciebie sposób to przesłanie nam wypełnionej formatki wydarzenia i ewentualnie zdjęć czy innych plików (na przykład zdjęcie tytułowe czy prezentacja), które przynależą do spotkania.

   * Formatka (zwyły tekst) znajduje się <a href="https://raw.githubusercontent.com/AgileWarsaw/netlify/devel-www/themes/agilewarsaw/archetypes/event.md" target="_blank">tutaj</a>.
	
   * Zapisz sobie lokalnie lub skopiuj tekst z tej strony i otwórz przy wykorzystaniu np. notatnika.

   * Wypełnij informacje o wydarzeniu według wskazówek w formatce. Pamiętaj że edytujesz treść wewnątrz cudzysłowu, sam cudzysłów zostaje.

   * Przykładowy wygląd wiersza z datą: `date: "2013-10-28T19:00:00+01:00"`
   
   * Jeśli brak sponsora pozostawiamy puste nawiasy: `[]`

   * To czy było nagranie i link do niego znajdziesz na <a href="https://www.youtube.com/playlist?list=PLXRBM3VxEbfPF2-ScvE03bQ6pNS-mli99">YouTube</a> - wklej adres url nagrania do formatki.

   * Jeżeli do wydarzenia były załączone jakieś zdjęcia lub inne pliki pobierz je ze strony (np. meetup, czasem bywają w komentarzach), zapisz lokalnie.

   * Prześlij nam wypełnioną formatkę i pliki na adres: `team@agilewarsaw.com`

## Przez github:

Jeśli nie boisz się GitHub-a albo chcesz spróbować z niego skorzystać możesz zaoszczędzić nam (organizatorom) pracy samodzielnie dołączając informacje do tej strony.

### TODO: opisać jak stworzyć wydarzenie posługując się tylko stroną GitHub.

## Wersja idealna czyli wszystko sprawdzone przez Ciebie:

Potrzebny Ci będzie klient Git, żeby móc pracować na lokalnych plikach oraz `Hugo` czyli program, który generuje tę stronę z danych.

Instalacja Hugo jest <a href="https://gohugo.io/getting-started/installing#quick-install" target="_blank">prosta na każdym systemie operacyjnym</a>. Możesz nawet ściągnąć jeden plik wykonywalny i użyć go bez instalacji.

1. Sklonuj lokalnie repozytorium `https://github.com/AgileWarsaw/netlify.git`

1. Sprawdź, czy jesteś na branch-u `?`

1. Sprawdź numer wydarzenia, które chcesz dodać.

2. W terminalu w folderze repozytorium wpisz:  
   `hugo new events/NUMER/index.md -k event`  
   zamieniając `NUMER` na właściwy numer wydarzenia.

3. Program stworzy nowy podkatalog `NUMER` w katalogu `content` a w nim formatkę wydarzenia.

4. Wypełnij formatkę.

5. Jeśli chcesz dołączyć dodatkowe pliki umieść je w tym samym katalogu.  
   Zdjęcie pod nazwą `hero.jpg` zostanie użyte jako "wizytówka" wydarzenia.

6. W terminalu wpisz:  
   `hugo server --watch`  
   i w przeglądarce (zwykle pod adresem `http://localhost:1313`) będziesz mógł przejrzeć stronę z Twoimi zmianami.

7. Jeśli wszystko jest dobrze, stwórz `pull request`.
