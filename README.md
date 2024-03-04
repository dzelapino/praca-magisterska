# praca-magisterska

## zarys + pomysły - żebym nie zapomniał

praca ma opierać się na porównaniu scope aplikacji

w pracy używam głównie 3 scope
- @ViewScope
- @SessionScope
- @ApplicationScope

jest jeszcze więcej scope których nie znam więc warto się zagłębić w ten temat

dodatkowo fajnie będzie pomyśleć o np jakimś interfejsie albo klasie abstrakcyjnej implementujących metody zwalniania pamięci
robimy uniwersalny helthcheck i sprawdzamy które obiekty są dłuższe niż x czasu, plus ich priorytet jest niski to je zabijamy

np jakiś obiekt z session scope istnieje i jego czas tworzenia podczas sprawdzania byl ponad godzinę temu to
robimy wymuszone odświeżenie obiektu

też warto pokminić jakieś przypadki użycia w sensie podczas modelowania apki ustalamy że dlaczego to zrobić lepiej sesyjne z np
mechanizmem zwalniania memory zamiast view i ciągle tworzyć na nowo te same obiekty

spoko pomysłem może być też sesyjna lista z danymi, puszczamy ograniczone query porównujące + sortujące same klucze w tablicy i porównujemy ich timestampy
jeśli różnią się to lecimy geta w innym wypadku nic nie robimy

ogólnie fajnie robić coś co może mi się przydać w robocie ale najważniejsze jest żeby podpiąć tam coś mającego merytoryczne znaczenie a nie sam łysy kod i finito
