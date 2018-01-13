# ABELight
Strona www konferencji ABE Light 2018

# Jak wprowadzić zmiany?

## Mechanika:

   1. Sklonuj to repo.
   2. Ściągnij odpowiednią wersję Hugo (generator statycznych stron) stąd: https://github.com/gohugoio/hugo/releases
   3. Lokalny podgląd: `hugo server --watch`
   4. Jeśli chcesz wprowadzić zmiany na stronie (a nie tylko u siebie lokalnie), wygeneruj nową statyczną wersję strony: `hugo` (pliki lądują w katalogu `docs`, który jest skonfigurowany jako źródło strony pod adresem `https://agilewarsaw.github.io/ABELight/`)
   5. Popchnij zmiany na github.

## Treść:

Większość treści znajduje się w pliku konfiguracyjnym `config.yml`

Inne miejsca:

  * Treść sekcji "O konferencji" jest w pliku `themes\hugo-conference\layouts\partials\about.html`

Na podstawie:
https://github.com/jweslley/hugo-conference
