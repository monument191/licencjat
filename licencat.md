Co to jest krypto waluta? Pytanie coraz częściej zadawane w dzisiejszych
czasach z powodu ich znaczenia na rynku. W 2008 został wypuszczony
Bitcoin, „Peer-to-Peer" system platnosci electronicznej". Nie
potrzebowal on serwera, ani centralnej administracji. Była to pierwsza
waluta wykorzystujaca ten system, od lat dziewiedziestiatych, przez cala
dekade proby wykozystania tego systemu były podejmowane, lecz wszystkie
skonczyly się niepowodzeniem. Dzieki pomysłowi Saotshi Nakamoto Bitcoin
stal się dość popularna waluta, kiedy zabierzemy caly marketing będzie
to porpostu wartość w bazie danych, czyli jak pieniądze na naszych
kontach w banku.\
Jak to działa?

Tutaj nei ma ustalonej wartości, sama waluta nie ma swojego odpowiednika
w przedmiotach materialnych, jest tam wiara w system, gdyż sa to tylko
wartości w bazie danych, wielkim plusem takiego sposobu jest brak
administracji oraz udziału państw. \[problem4\] . Dzieki temu poporstu
ogłaszamy ze chcemy zrobić transfer z danego konta na inne konto podajac
jego dane oraz wartrosc przeslanej waluty. Aby zapobiec podszywaniu się
pod innych uzytkownikow, gdyż wszytkei numery sa publiczne, używane sa
klucze prywatne dzięki którym może zostać wygenerowany elektroniczny
podpis które odpowiadają podpisowi w czekach i wekslach. Pozwala ona
innym użytkownika potwierdzić ze ta tranzakcja została wyslana przez
wlasnie tego użytkownika i wlasnie do tej transakcji. Sa one unikalne
dla każdej transakcji wiec nie jest to system w którym latwo możemy
podrobić czyjs podpis. Ten podpis mowi kto wysłał tranzakcje lecz nie
keidy ja wysłal. Jest to problematycz gdyż ktoś moglby wyslac dwie
tranzakcje, lecz mieć srodki tylko na jedna. Stwaza to problem bo rozne
osoby na swiecie moglyby posiadac rozne wartości w swojej bazie przez
opóźnienia przesyłowe. Bitcoin i inne waluty zapobiegają temu poprzez
tworzenie lancucha transakcji który ustala kolejność tych transakcji.
Kolejnosc tych transakcji zależy trochę od matematycznej loterii. Każdy
uczestnik tej loterii wybiera jedna tranzakcje i proboje ja rozwiazac.
Ten kto pierwszy rozwiaze otrzymany problem dodaje swoja tranzakcje do
lancucha jako ostatnia tranzakcja.

Wszsytko opiera się na technologii zwanej blockchain, jest to rosnaca
lista rekordow nazywanych blockami. Blocki te mogą być przechowywane
jako plik lub prosta baza danych. Blocki sa połączone ze sobą, odnoszą
się one do poprzedniego bloku w łańcuchu. Są one przedstawiane jako
bloczki ustawione jeden nad drugim gdzie jego wysokość określa odleglosc
od pierwszego bloku, takei przedstawienie jest odmiana drzewka Merkle.
Każdy blok może zostać zidentyfikowany po hash'u który jest generowany
przy pomocy SHA256 cryptographic hash algorithm w nagłówku każdego
blocku. Każdy blok zna swojego „rodzica" dzięki polu „hash poprzedniego
blocku" (z ang. „previous block hash")w jego nagłówku. Łańcuch ten
ciągnie się az do pierwszego bloku który został stworzony w bitcoinie
nazywanym „Genesis block". W czasie aktualizacji systemu lub wytworzeniu
dwóch blokow na tym samym rodzicu powstają fork'i. Musimy pamietac ze
technologia blockchain bazuje na wspólnym działaniu wielu komputerow .
Każdy z pojedynczych komputerow którego celem jest weryfikacja
blockchainowych rejestrow publicznych i utrzymywanie sieci bezpiecznej
jest potocznie zwany „full node". Aby było to możliwe każdy full node
musi pracować na tej samej wersji oprogramowania, aby uzyskac dostep do
tych samych rejestrow. Dla przykładu full node operujący na systemie
Bitcoin Core ma dostep do rejestrow blockchainowych Bitcoina, dzięki
czemu może zweryfikować transakcje Bitcoinowe i mieć dostep do historii
transakcji, lecz system operujący na oprogramowaniu Go-etherum nie mogą
uzyskac dostępu do blockchaina Bitcoin'a. Istnieja dwa rodzaje:\
Hard Frok -- Istnieje on wtedy gdy powstają dwie różne wersje, ta w
której obowiazuje wszystkie stare prawa i ta w której obowiazuja nowe,
są one całkowicie od siebie niezależne, nie ma pomiędzy nimi transportu
danych ani komunikacji, maja one dostęp do tej samej historii transakcji
lecz od momenut podziału ich historie się nie będą pokrywać.
![E:\\pobrane\\licencjat\\RmGZ.png](media/image1.png){width="5.8125in"
height="2.5625in"}\
\
Soft Fork -- Dzieje się tak kiedy wprowadzamy nowe protokoły które sa
kompatybilne
wstecz.![E:\\pobrane\\licencjat\\RH3J.png](media/image2.png){width="6.291666666666667in"
height="2.4895833333333335in"}

Jak to się odnosi do naszego tematu? W krypto walutach potwierdzenie
jest czyms co pozwala na temu systemowi dzialac. Dopuki tranzakcja jest
oczekujaca nie oznacza ona nic dla systemu, może ona zostać dowolnie
zmieniona, lecz jeżeli zostanie potwierdzoan wszyscy w systemie będą
wiedzieć ze została zrealizowana, oznacza to ze każdy użytkownik będzie
widział zmiane jaka wprowadzila ona na nasze konto jak i na konto
drugiej strony transakcji.\
Jeżeli nie mamy serwera, ani administracji jak możemy potwierdzać nasze
tranzakcje? Czy każdy będzie musial uzwiezyc nam na slowo? Problem ten
jest rozwiązany przez kopaczy którzy w naszym systemie. Dekoduja oni
tranzakcje tak, aby zweryfikować ich uczciwość. Po potwiedzeniu
tranzakcja kazda czesc wezlu musi dodac ja do swojej bazy danych. Wtedy
dopiero staje się ona czescia łańcucha blokowego.

Po wykonainu tej pracy kopacze dostają zaplate w formie tokenu
odpowiedniej kryptowaluty na której rzecz pracują, np. bitcoin,
electrum.

Kopaczem kryptowaluty może być każdy. Przez brak centralnej jednostki
zarzadzajace nie ma srodkow ani osob które moglyby to zlecac. Aby nie
spowodować katastrofy która by powstala przez podrabianie kluczy przy
pomocy tysięcy urzadzen, tworca zadecydowal ze kazda tranzakcja laczy
się z opciazeniami na naszym komputerze. W jaki sposób to osiagnal?
Postawil zasade która musi być spelniona aby tranzakcja mogla zostać
zrealizowana. Żeby to osiagnac musza oni wygenerowac hash dzięki któremu
można polaczcy nowy block z poprzednimi w lancuchu. Nazwal to
Proof-of-Work. W przypadku bitcoin'a najpopularniejszej kryptowaluty
jest to algorytm nazwany SHA 256 Hash.\
Polega to na kodowaniu tekstu tak aby nikt bez sekretnego kodu nie mogl
go odczytac. Po znalezieniu rozwiązania kopacz może stworzyć blok i
dodac go do lancucha blkowego. Jako nagroda za wykonanie tej pracy
dostaje on na swoje konto prederminowana liczbe kryptowaluty. Jest to
jedyny sposób na utworzenie ważnego Bitcoina. Trudnosc tych kodow jest
zwiekszana z iloscia komputerow w całej sieci kopaczy, zapobiega to
tworzeniu nieskończonej ilości waluty. Dzieki takim działania
zapobiegawczym w danym momencie można wytworzyć tylko okreslona liczbe
kryptowaluty. Jest to zasada która nei może zostać zlamana przez nikogo.

Dlaczego ludzie inwestują w kryptowaluty?

Jest to najlepszy przykład ze ludzie nie potrzebują państwa aby mieć
walute. Sa one zbudowane na cryptografi przez co nie musimy ufac zadnej
partii rzadzacej lub innym osoba, lecz matematyce. Zawieraja tez wiele
potrzebnych i ważnych elementow waluty.\
Piewrwszym sa właściwości tranzakcyjne gdzie wyroznaimy cztery
najważniejsze.\
Nieodwracalnosc, po potwierdzeniu nie da się cofnac transakcji jak to
jest możliwe w przypadku banku lub innych instytucjach. Jeżeli stracimy
je w jakiś stopniu nie możemy ich cofnac, jest to problematyczne jeżeli
zostanie nam wykradzione dane logowania. Wiec niestety to rozwiązanie
posiada plus jak i minusy.

Anonimowosc, ani tranzakcja, ani konto nie jest powiazane do czegos co
ma odpowiednik w naszym siwecie, nie jest podpisane do sooby tak jak to
bywa w bankach, a wartości na nim nie odpowiadaj niczym fizycznym jak np
rezerwa zlota. Zazwyczaj możemy przeanalizować ze tranzakcja się odbyla
nie zawsze mozmey przypisac to do ludzi którzy dokonali tych transakcji.
Jest to przydatne dla ludzi którym panastwo zakazuje kupowania lub
sprzedaży niektórych produktów. Lecz tak jak w poprzednim przykładzie
jest to miecz obusieczny gdyż może zostać wykozystany np. rpzez
terroystow do zakupow broni.

Szybkosc i ogolnosiwatowsc, tranzakcje sa prawie natychmiastowo
rozporwadzane bo sieci, ich potwierdzenei zajmuje więcej czasu ale tez
nei jest to zazwyczaj czas dłuższy niż czas potwieredznia przelewu
bankowego. Nie zaleza tez one od przynaznosci do kraju lub miejsca
zamieszkania, sa tak samo szybko rozpatrzywane bez względu na lokacje.

Bezpieczenstwo, jedynie wlasciciel prywatnego klucza, czyli wlasciciel
konta, może wyslac krypto walute. Dzieki zabezpieczenia kryptograficznym
jest to niemożliwe z naszymi możliwościami do zlamiania. Jest on
trudniejszy do złamania niż hasla i loginy do stron bankowych.

Nie wymaga zezwolenia, kryptowaluty nie wymagaj zadnego zezwolenia, aby
moc z nich kozystac. Najczesciej użytkownik może zazac przez zwykle
pobranie programu. Po zainstalowaniu możemy już wysylac i otrzymywać
wszystkie kryptowaluty. Nie mogą być na użytkownika nalozne działania
prewencyjne, nie ma jak w banku wymogu posiadania 13 lat i mogą to robic
osoby którym prawnie zabrano możliwość dokonywania transakcji.

Właściwości monetrane\
Kontrolowana wartość, wiekszsoc kryto walut ogranicza ilość tokenow
jakimi operuje. Na ten przykład bitcoin zmniejsza ilość tokenow
dostarczanych i tych nagradzanych za prace. Osiagna oni swój limit około
roku 2140. Wszystkei kryptowaluty kontrolują zasob tokenow przez plan
napisany w kodzie. Oznacza to ze nie jest on nieskończony i może zostać
określony już na początku. Dzięki temu nie musimy polegać na niewiadomej
liczbie maksymalnej token, lecz po jej określeniu możemy zobaczyć ile
jest w tym momencie w obiegu.

Nie są one długiem. W przypadku banków i innych instytucji nie operujemy
na walucie lecz na długu który posiada wobec nas bank lub państwo.
Kryptowaluty przez swój zamysl nie sa długiem, lecz waluta sama w sobie
nie odpowiadająca długowi, lecz tak jak w średniowieczu zlote monety,
których wartością były one same, kosztowały tyle samo co ich surowce.

Reolucjonalny wpływ kryptowalut jest zasluga obu tych wartość.
Kryptowaluty sa nieodwracalne, nie wymagające zezwoleń i pozwalajaca
uzywac pseudonimu dzięki czemu ich uzytkownicy nie sa zalezno od zadnego
banku ani rządu. Nie można utrudniać dostępu do kryptowalut, nie można
zabronić komus ich otrzymywać ani nie można cofnac ich transakcji.

Jako waluta z limitowa, kontrolwoana ilsocia która nie mzoe zostać
zmieniona przez bank, rząd lub inne centralnej instytucji, kryptowalut
sprzeciwia się zakresowi polityki pienierznej. Zabiera tez możliwość
sztucznej inflacji lub deflacji przez zmiany w ilości dostępnych
pieniędzy.

Teoria portfela Markowitz\
\
Markowitz opublikowal swoją pracę „Portfolio Selection" na temat
portfela w roku 1952 w renomowanym piśmie „Journal of Fiance". W tych
pracach zawarł on podstawy na których których kbazujemy wszystkie
nowoczesne modele. Rewolucji tej dokonal podczas badań na dotychcasz
istniejący model wartości obencej Johna Burr Williamsa. Markowitz
zauważył problem w tej teorii przez brak analizy wpływu ryzyka, który
był pomijany. Nawiazał on tez do zależności pomiędzy zyskami a ryzykiem,

[[https://blockgeeks.com/guides/what-is-cryptocurrency/\#What\_Are\_Miners\_Doing]{.underline}](https://blockgeeks.com/guides/what-is-cryptocurrency/#What_Are_Miners_Doing)

[[https://cryptocurrencyfacts.com/how-does-cryptocurrency-work-2/]{.underline}](https://cryptocurrencyfacts.com/how-does-cryptocurrency-work-2/)
