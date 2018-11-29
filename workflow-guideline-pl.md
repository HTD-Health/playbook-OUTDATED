## Workflow
- Commituj często, oraz dobrze opisuj zmiany w commit message. Lista Twoich commitów powinna być czytelnym changelogiem dla osób robiących review.
- Pull requesty powinny być możliwie małe i skupione wokół jednej funkcjonalności 
   - Jeśli w trakcie pracy nad jaką funkcjonalnością znajdujesz buga, który nie dotyczy bezpośrednio Twojego zadania, dodaj kartę do backlogu. Jeśli bug jest poważny, ustal z zespołem kto powinien się nim zająć. Poprawka powinna być wdrożona przez dedykowaną branch
- Każdy developer jest odpowiedzialny za swój PR od początku do końca tj.
   - Nazwa brancha powinna podążać za konwencja: feature/nut-123-style-appointment-screen
   - Stosować się do Pull Request template (ustalany indywidualnie dla projektu)
   - Przetestowanie i zadbanie o czystość kodu przed poproszeniem innych developerów o review. Pull request może być stworzony w celu wcześniejszej prezentacji pozostałym członkom zespołu, w takim wypadku przypisz mu label ‘Work In Progress’ aby było jasne że nie należy go mergować. Pull request w githubie jest również dobrym narzędziem do obejrzenia diffu własnego kodu i self-review.
   - Przypominać o wiszącym PR jeśli code review nie jest robione przez długi czas
   - Jakość w projekcie jest odpowiedzialnością zespołu, każdy powinien dbać o zrobienie code review, przetestowanie oraz dostarczenie kompletnego feature
   - Zadbaj o czystą historię swoich commitów
   - Usunięcie branchy po skończeniu taska
   - Aktualizacja tablicy z zadaniami po skończeniu taska




## Code review 
- Przede wszystkim nie przywiązuj się do swojego kodu :) Code review ma na celu poprawę jakości kodu w projekcie oraz wzajemną naukę i wymianę opinii pomiędzy developerami. Uwagi do kodu nie są personalnym atakiem nie zrażaj się więc jeśli Twój PR zostanie odrzucony.
- Nie bój się zadawać pytań! Jeśli nie rozumiesz jakiejś części kodu poprosić jego autora o wytłumaczenie. Kod powinien być przede wszystkim czytelny i zrozumiały. Może wypracujecie w ten sposób bardziej przejrzyste rozwiązanie?
- Jako osoba robiąca review staraj się sugerować zmiany i rozpoczynać dyskusję. Nie wytykaj błędów w agresywny sposób oraz nie krytykuj innych, w końcu każdy może mieć gorszy dzień :)
- Code review nie powinno być blokujące dla pracy innych, staraj się nie odwlekać go i przejrzy ich kod w najbliższym wolnym przebiegu.
- Przed poproszeniem o review upewnij się że proces CI przeszedł bez błędów.
- Każdy otwarty PR oznacza gotowość do review, chyba że został mu przypisany label Work In Progress. Review może zostać wykonane przez każdego członka zespołu. Jeśli potrzebujesz review konkretnej osoby przypisz go jako Reviewer w githubie.
- Jeśli robisz review, nie zostawiaj pustych komentarzy. Jeśli chcesz dać feedback, oznacz PR jako rejected jeśli wymaga poprawek przed domergowaniem lub approved jeśli wszystko jest w porządku lub uwagi nie są znaczące.
- Aby domergować PR do głównej branchy powinien być przynajmniej 1 approval w zespołach 2-3 osobowych lub 2 approvale w zespołach 4 osobowych i większych.




## Dyscyplina w pracy
- CI na głównej branchy powinno być utrzymywane na zielono przez cały czas, nie mergujemy oraz nie robimy deployu z branchy na której nie przeszedł poprawnie build
- Code review i testy są wymogiem utrzymywania jakości i integralną częścią pracy w projekcie. Nie powinny być pomijane ze względu na opóźnienie dostarczenia funkcjonalności, powinniśmy uznawać taką rzecz za równie niekompletną jak funkcjonalność która nie działa
- Testy powinny być dopisywane na bieżąco jako integralna część pracy nad zadaniem. Nie będzie dobrego czasu na dopisanie testów “później” :)
- Pracuj tylko nad rzeczami z kolumny “To Do” które zaplanowaliście podczas sprint planningu lub groomingu. Staraj się zachować skupienie nad konkretną kartą którą aktualnie masz przypisaną. Jeśli po drodze znajdziesz dodatkowe bugi lub miejsca do refactoru oznacz je np poprzez stworzenie karty w backlogu, wrócicie do nich w odpowiednim czasie
- Kolumna To Do powinna zawierać jedynie taski które posiadają kompletne informacje do ich zrealizowania np przygotowane grafiki lub API
- Pracuj maksymalnie nad dwoma zadaniami na raz i staraj się doprowadzić je do końca jak najszybciej. Nie rozpoczynaj kolejnych zadań dopóki nie domergujesz oraz nie zaktualizujesz tablicy zadań. Jeśli blokuje Cię code review, przypomnij się osobom odpowiedzialnym. W wolnym czasie możesz pomyśleć o miejscach w aplikacji które można poprawić, dopisać testy, zadbać o porządek w dokumentacji lub cokolwiek co przyniesie korzyści zespołowi
- Staraj się kończyć zadania tego samego dnia w którym je zacząłeś. Staraj się rozplanować pracę w taki sposób aby na koniec dnia mieć wszystkie taski w kolumnie ‘Code Review’.


