# CodersCamp 2020 - Projekt TypeScript
**CodersCamp (coderscamp.edu.pl) - Największy otwarty kurs programowania webowego** 

![Szachy - Ekrany](./.github/images/SzachyEkrany.png)
Proponowany projekt — Szachy (opis poniżej).

### Zasady wykonywania projektu (wspólne dla wszystkich grup i mentorów): 

##### W projekcie każdy z uczestników powinien zaprezentować praktyczną znajomość poniższych zagadnień związanych z TypeScript:
- typy podstawowe
- definiowanie własnych typów
- składanie typów
- typy / klasy / interfejsy
- implementacja / dziedziczenie / kompozycja / implementacja interfejsu
- modyfikatory dostępu 
- typy generyczne
- testy jednostkowe i TDD

##### W trakcie trwania projektu należy wyznaczyć w zespole następujące role
tak jak opisano w przypadku poprzedniego projektu.

##### Sposób oceny projektu (i wszystkich kolejnych projektów na CodersCamp)
tak jak opisano w przypadku poprzedniego projektu.

## Gra w Szachy
Teraz przechodzimy do przykładowego projektu, który został przygotowany przez organizatorów kursu.
Proponowany projekt pozwala na zastosowania większości umiejętności, jakie powinniście posiąść w trakcie przerabiania działu.
Jednakże jeśli macie pomysł na projekt podobnej skali, który spełni opisane na górze wymagania i czujecie się na siłach
w zdefiniowaniu funkcjonalności, przygotowaniu ekranów i podzieleniu go na zadania — to nic nie stoi na przeszkodzie,
aby wykonać np. coś związanego z zainteresowaniami Waszej grupy :)
Przykładem może być też jakaś inna gra — np. Chińczyk. Niech nic nie stoi na przeszkodzie waszej kreatywności.
Pamiętajcie tylko, że czas jest ograniczony i musicie zdążyć z aplikacją do prezentacji. Powodzenia!
 
Czas porzucić narrację CodersCamp i wcielić się w członka zespołu projektowego...

### Założenia projektowe
W trakcie projektu stajecie przed większym (lub mniejszym — jak kto woli) wyzwaniem.
Teraz nie macie niestety ani linijki już gotowego kodu. Swoją pracę zaczynacie w tzw. projekcie greenfield, czyli totalnie od zera.
Pozwala to na większą dowolność, ale też wymaga na początku większego nakładu pracy i jest wąskim gardłem. 
Jako zespół musicie podjąć odpowiednie decyzje na samym początku i postarać się jak najszybciej umożliwić pracę wielu osobom naraz.

Szachy są coraz bardziej popularne wśród przedsiębiorców. Odbywają się nawet Mistrzostwa Polski dla osób prowadzące własne działalności.
Niestety, obecna sytuacja z pandemią pokrzyżowała trochę plany zorganizowania kolejnych mistrzostw.
Po sukciesie waszego ostatniego projektu wiele osób z tego środowiska usłyszało o waszych usługach.
Dlatego wasz zespół został poproszony o przygotowanie mechanizmu szachów, który pomógłby w organizacji tych mistrzostw online.
Oczywiście jest to o wiele większy projekt, dlatego Wy odpowiadacie tylko za sam mechanizm szachów w przeglądarce.
Nie skupiacie się na kwestiach gry wielu graczy przez internet itp.

Ponieważ aplikacja ma być sygnowana przez CodersCrew, spróbujcie przygotować ją zgodnie z identyfikacją wizualną stowarzyszenia - Brand Book znajdziecie [TUTAJ](https://www.behance.net/gallery/94155751/Brand-Book-Project). 
Nie jest to konieczność, ale fajna możliwość wypróbowania swojej skuteczności z takim wymaganiem (które jest częste w praktyce). 


Lista funkjonalności, jakie należy zaimplementować w silniku gry:
1. Ruchy wszystkich bierek (wykonanie ruchu, jak i pokazywanie możliwych):
   - Pionek
   - Hetman
   - Wieża
   - Goniec
   - Król.
1. Promowanie pionka na dowolną inną figurę (oprócz króla) na końcu planszy.
1. Roszada: https://pl.wikipedia.org/wiki/Roszada
1. Szachowanie króla: https://pl.wikipedia.org/wiki/Szach_(szachy)
1. Szach mat: https://pl.wikipedia.org/wiki/Mat_(szachy)
1. Możliwość cofania ruchów (aż do początkowego układu).
1. Tekstowe komentarze do gry (przykładowo):
   - `Gracz Biały wykonał ruch "Koń z C1 na D3"`
   - `Gracz Czarny dokonał promocji Pionka na Hetmana na polu A1. Szach białego Króla!`
   - `Gracz Biały wykonał roszadę po stronie królowej.`
1. Możliwość wyboru nieskończonego czasu gry lub szachów błyskawicznych.
1. Odliczanie czasu dla każdej ze stron (cofanie ruchu musi cofać czas do stanu sprzed ruchu) w przypadku szachów błyskawicznych.
1. Dodatkowy czas doliczany do limitu czasowego gracza za każdy ruch (propocjonalny do długości całej patrii). 
1. Kończenie gry przez limit czasowy - gracz, któremu skończył się czas przegrywa. Nie rozpatrujemy przypadku porażki.
1. Wczytywanie i zapisywanie stanu partii (szachownica, czas graczy itp.) - po wczytaniu musi być możliwe cofanie ruchów. Stan partii powinien zapisywać się automatycznie co wykonany ruch.
1. Tworzenie nowej partii z aktualnego stanu partii. Gra nie może być zakończona.

  
Uwaga: Pamiętajcie, że na ruchy bierek, promocja pionka, możliwość roszady wpływa na szachowanie króla. 
Dokładnie poznajcie domenę, w jakiej działa wasze oprogramowanie, czyli grę w szachy, aby nie wprowadzić jakiegoś zachowania niezgodnego z zasadami. 
Starajcie się przewidzieć przypadki brzegowe i zaimplementujcie do nich odpowiednie testy.

**Jeśli macie w swoim zespole osobę chętną na przygotowanie designów, to także możecie UI zrobić kompletnie inaczej.**
A jeśli nie, to możecie się wzorować na przedstawionych [TUTAJ - Link do Figma](https://www.figma.com/file/ZllWbpJCCCCKVl7QEfNWbl/CodersCamp2020.Project.TypeScript.Chess?node-id=4461%3A3896). 
Jednakże brakuje takich rzeczy jak np. wczytywanie / zapisywanie partii, wyświetlanie możliwych ruchów, podświetlanie wybranego pionka, zaznaczenie szachowanego króla czy wybór podczas promowania pionka. Co powinniście zaprojektować w ramach wykonywania aplikacji. Szczegóły ustalcie z klientem.

Waszym zadaniem będzie zaimplementować aplikację, aby działała wg wymagań klienta, a także przygotować i wykonać
wersję responsywną aplikacji (dostosowaną do wyświetlania na Tabletach i Telefonach — możecie przygotować najpierw projekt interfejsu, lub od razu przejść do implementacji).
W celu zaprezentowania działania aplikacja musi być możliwa do odwiedzenia w internecie.
Klient nie chce ponosić za to żadnych dodatkowych kosztów, dlatego należy wykorzystać jedną z usług oferujących darmowe
uruchomienie takiej aplikacji (np. GitHub Pages).
Klient wymaga także, aby aplikacja nie tylko działała, ale była odpowiednio pokryta testami.
Naprawdę macie szczęście co do klienta! Wielu uważa testy za niepotrzebne i jedynie stratę pieniędzy.
A co znaczy „odpowiednio pokryta”, to już należy właśnie ustalić z samym Klientem :) 

## Możliwe usprawnienia i dodatkowe funkcjonalności:
Jeśli starczy czasu, dla własnego rozwoju warto rozważyć wykonanie poniższych funkcjonalności. 

1. Zaimplementuj kończenie gry przez Pat.
1. Dwie wersje językowe gry — Polska i Angielska.
1. Ładowanie stanu początkowego z np. notacji FEN (https://pl.wikipedia.org/wiki/Notacja_Forsytha-Edwardsa) i/lub tablicy emojis.
1. Zaimplementuj różne strategie Pat opisane na Wikipedii: https://pl.wikipedia.org/wiki/Pat Np. stare zasady mówiły, że pat powodował wygraną strony, która zapatowała przeciwnika.
1. Głosowe wykonywanie ruchów. Np. gracz mówi: "Pion na A3".

## Dodatkowe zadania (wykraczające poza zakres kursu):
1. Wykonanie testów E2E, przy użyciu odpowiedniego narzędzia. Proponujemy np. Cypress.

Wszelkie inne dodane przez Was funkcjonalności czy usprawnienia infrastrukturalne należy przedstawić w README.md projektu :)
Template znajdziecie w poprzednim projekcie.

## Porady odnośnie do projektu
- Warto zapozań się z możliwościami kończenia partii szachowych (nie wszystko jest wymagane).
   - [How Chess Games Can End: 8 Ways Explained](https://www.chess.com/article/view/how-chess-games-can-end-8-ways-explained)
- Jako inspirację można wykorzystać też działanie szachów zaimplementowanych przez zespół mentora Marcina Wosia na poprzednim CodersCamp (UWAGA: Wymagania mogły ulec zmianie)
   - https://captainobjective.github.io/chessGame/
- Dla testów może warto wykorzystać trochę reprezentacji wizualnej. Co powiecie na emoji :) ? 
   - [Emoji-Driven Development | ZycieNaKodach.pl](https://zycienakodach.pl/tdd-dsl-szachy-emojis)
