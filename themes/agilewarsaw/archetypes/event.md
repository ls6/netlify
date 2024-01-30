---
number: "Numer wydarzenia bez znaku `#`"
date: "{{ .Date }}"
title: "Tytuł. Uwaga na cudzysłowy w tytule, trzeba je poprzedzić ukośnikiem \"tak\" ."
speakers: "Imię Nazwisko, Imię2 Nazwisko2"
lang: "Wpisz pl albo en"
sponsors: ["sponsor1", "sponsor2"]
videoURL: ""
draft: false
---

Format daty (i godziny) wydarzenia do wpisania w nagłówku powyżej:
 "2023-12-14T19:00:00+01:00"

Opis wydarzenia robimy w formacie Markdown.

Ściągawka z Markdown w sieci:
<a href="https://learn.microsoft.com/pl-pl/training/modules/communicate-using-markdown/2-what-is-markdown" target="_blank">Ściągawka z Markdown-a</a>.

Najczęściej używane formatowanie:

Paragrafy oddzielamy pustą linią.

Nową linię bez tworzenia nowego paragrafu zrobisz wpisując dwie spacje   
na końcu łamanej linii.

# Nagłówek 1
## Nagłówek 2
itd.

Lista:

  * bullet
  * bullet

  1. numerowana
  2. numerowana

Linki zewnętrzne (jeśli mają otwierać się w nowym oknie) opisujemy HTMLem:
<a href="https:link" target="_blank">Opis</a>.

Linki, które mają otworzyć się w tym samym oknie możesz opsiać w Markdown: [opis](https://link)

## galeria / miniatury

Mamy nasz własny skrót na utworzenie miniatury zdjęcia (thumbnail), który po kliknięciu otwiera zdjęcie w pełnej wielkości.

Plik z grafiką umieść w tym samym katalogu, w którym jest opis i w treści wstaw kod:

{{< thumbnail src="nazwa-pliku.xxx" alt="Podpis pod miniaturką" >}}

Możesz wstawić dowolną liczbę takich miniaturek.

## Ikonki

{{% icon-flag-pl %}}
{{% icon-flag-en %}}
{{% icon-yt-red %}}
{{% icon-yt-gray %}}
