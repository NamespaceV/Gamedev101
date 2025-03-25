# Programista czego się uczyć

Jeśli chodzi o programowanie jest kilka obszarów w których trzeba się rozwijać. Obszary są troche powiązane, a trochę niezależne.

## Spis treści

-   [1 Języki programowania](https://gamedev-pl.fandom.com/pl/wiki/Programista_czego_si%C4%99_uczy%C4%87#J.C4.99zyki_programowania)
-   [2 Biblioteki, frameworki i silniki](https://gamedev-pl.fandom.com/pl/wiki/Programista_czego_si%C4%99_uczy%C4%87#Biblioteki.2C_frameworki_i_silniki)
-   [3 Algorytmy](https://gamedev-pl.fandom.com/pl/wiki/Programista_czego_si%C4%99_uczy%C4%87#Algorytmy)
-   [4 Narzędzia i sposoby organizacji kodu](https://gamedev-pl.fandom.com/pl/wiki/Programista_czego_si%C4%99_uczy%C4%87#Narz.C4.99dzia_i_sposoby_organizacji_kodu)
-   [5 Poradniki](https://gamedev-pl.fandom.com/pl/wiki/Programista_czego_si%C4%99_uczy%C4%87#Poradniki)

## Języki programowania

To lista istotnych języków z krótkim komentarzem

-   Assembler (assembly) - 1950

Asemblery to pierwsze języki programowania. Są to języki najbliżej metalu. Do tego stopnia że każda rodzina procesorów ma inny assembler. Mają tylko drobne ułatwienia i przekładają się na kod maszynowy praktycznie 1-1 Co sprawia że nawet proste małe programy mają dużo linii kodu i nie są łatwe w analizie. Kod w asemblerze generalnei nie ma struktóry, to seria poleceń i można w nim wyrazić wszystko co procesor moze wykonać. Ale często powoduje to małą czytelnosc kodu i duze trudnosci przy wprowadzaniu zmian. W obecnych czasach mało kto pisze w asemblerze, ale jest to ciekawe ćwiczenie żeby zobaczyć jak procesor faktycznie działa. Jest to też język najbliżej kodu maszynowego i jego znajomość przydaje się przy próbach inżynierii wstecznej (reverse engineering) czyli dekompilacji programu i analizy jego działania. Twórcy starszych gier musieli czasem używać tego typu języka by osiągnąć większą wydajność albo zmierzyć się z dziwną architekturą. W obecnych czasach raczej nie jest to praktyczny pomysł.

-   C - 1972

Język C jest podstawą większości popularnych obecnie języków programowania. Język stworzony żeby ułatwić pracę z wczesnymi wersjami Unixa okazał się strzałem w dziesiątkę. Do dziś jego rozszerzone wersje są używane w różnych zastosowaniach. Teraz najczęściej korzysta się z innych języków z większą ilością ułatwień, ale wspólne korzenie w C są bardzo odczuwalne i nauka C ułatwi wejście w inne języki.

-   C++ - 1985

Język "ce plus plus" jest rozwinięciem języka C o koncepcje obiektowe. Obiekty pozwalają poukładać dane i operujące na nich funkcje w grupy. Taka organizacja umożliwia budowę i utrzymanie dużych systemów. C++ przeszedł wiele usprawnień, ale jest odczuwalna jego 40 letnia historia. Niemniej mimo swoich problemów jest to język używany często do dziś. Jest niezastąpiony tam gdzie liczy się wydajność, ponieważ celowo nie ma ułatwień, które tą wydajność mogą obniżyć. Duże silniki takie jak Unreal Engine czy Unity 3D są napisane właśnie w c++.

-   Java - 1995

Zainspirowana sukcesem c++ firma sun postanowiła stworzyć przyjemniejszą w użyciu i bardziej przenośną wersję c++. Język Java nie jest kompilowany do instrukcji procesora, ale do tak zwanego "bytecode" - kodu pośredniego. Potem na każdej platformie odpowiedni interpreter przerabia bytecode na kod maszynowy w locie. Co sprawia ze ten sam program może chodzić na różnych rodzajach procesorów i systemów operacyjnych. Java mocno odświeżyła też sam język pozbywając się plików nagłówkowych. I wymusza stosowanie obiektowości i Garbage Collectora czyli mechanizmu który sprząta nieużywane obiekty. Kiedyś było trochę gier napisanych jako applety Javy. Teraz jest to mało popularny kierunek dla gier, ale dalej sprawdza się w dużych systemach biznesowych.

-   ECMAScript aka Java Script - 1995

W tym samym roku co Java ale kilka miesięcy później programiści przeglądarki Netscape stworzyli język JavaScript. Język ten ma z Javą bardzo mało wspólnego, ale jest często mylony z powodu nazwy, dlatego warto używać terminu ECMAScript od nazwy organizacji która język standaryzuje. Składnia jest mocno oparta na znanym i lubianym C, ale sam język ma diametralnie inne założenia. Służy przede wszystkim do wprowadzania interaktywnych elementów do stron internetowych. Wydajność nigdy nie była istotnym elementem projektu języka. Twórcy starali się też ułatwić pianie programów początkującym programistom, co sprawia ze język toleruje dużo dziwnych zapisów w kodzie programów i nie przejmuje się typami obiektów. O ile trochę to pomaga przy małych programach o tyle przy bardziej rozbudowanym kodzie potrafi chować błędy i utrudniać zrozumienie jak program działa...

Język stał się standardem dla całego internetu w tym gier w przeglądarkach. Google chrome znacznie poprawił wydajność interpretea ECMA Scriptu co umożliwiło budowę bardziej rozbudowanych aplikacji a JS. Z racji popularności doczekał się też możliwości budowy programów poza przeglądarką w tym serwerów, dzięki projektowi "node.js". Do pomocy w budowie większych aplikacji został stworzony TypeScript - nakładka na ECMA script która pozwala lepiej kontrolować typy obiektów w kodzie JS. Język jest wart uwago z racji na aplikacje webowe które go używają.

Jeśli chodzi o strony www w trzeba też wspomnieć o HTML i CSS. Nie są to języki programowania, bo nie można nimi opisywać obliczeń. HTML opisuje treść strony www i trzeba go trochę poznać ponieważ JS będzie zwykle manipulował elementami strony. CSS pozwala opisać jak powinna wyglądać strona, co również będzie niezbędne by stworzyć funkcjonalną aplikację webową.

-   C# - 2000

Czyt. "si szarp" to odpowiedź Microsoftu na Javę. Jest trochę nowszy i wyciągnął trochę wniosków z konstrukcji Javy. Do niedawna był dostępny tylko na systemie operacyjnym Windows, ale od jakiegoś czasu Microsoft uwolnił język i zaczął wspierać inne systemy operacyjne (projekt dot net core). Udostępnił też darmowe środowiska do pracy w tym języku. W świecie gier C# używany jest głównie jako język skryptowy w silniku Unity3D Jest też często spotykany do małych narzędzi przy silniku z racji szybszego tworzenia takich narzędzi niż w c++

Honorable mentions

-   Języki do Shaderów ~2004

Shadery to specjalne programy wykonywane na karcie graficznej. Specjalne języki takie jak HLSL, GLSL są używane do pisania programów, które następnie wysyłane są na kartę graficzną i pozwalają na wykonywanie niestandardowych efektów graficznych. Te języki służą tylko i wyłącznie do programowania efektów graficznych (są też trochę inne języki do wykonywania obliczeń nie związanych z grafiką na kartach graficznych) Przydają się do zaawansowanych efektów graficznych. Często silniki opakowują je w wizualne bloczki które kompilują się do kodu w takim języku tak żeby zapewnić większą przenośność i umożliwić technicznym grafikom korzystanie z możliwości jakie dają wyspecjalizowane shadery bez koniecznosci pisania kodu.

-   LUA - 1993

Lua jest językiem skryptowym, który relatywnie łatwo połączyć z aplikacją w C/C++. Z tego powodu LUA często pojawia się jako język skryptowy w różnych silnikach np [https://en.wikipedia.org/wiki/Category:Lua_(programming_language)-scripted_video_games](https://en.wikipedia.org/wiki/Category:Lua_(programming_language)-scripted_video_games)

-   Python - 1991

Kolejny język skryptowy ogólnego przeznaczenia. Bardzo popularny w wielu zastosowaniach. Są biblioteki umożliwiające tworzenie gier w pythonie ale nie jest to zbyt popularne rozwiązanie. Ale python może się przydać do automatyzacji różnych procesów albo szybkiego tworzenia prostych programów.

-   i wiele, wiele, wiele innych

Języków programowania jest bardzo dużo. Na studiach informatycznych często jednym z zadań jest stworzenie własnego. Różne silnik i systemy często tworzą też własne języki i formaty przystosowane do zadań które wykonuje dany system czy rodzaju zachowań potrzebnych w danej grze. Zdecydowana większość jest jakąś wariacją na temat rozwiązań spotykanych w C++ i jego pochodnych.

## Biblioteki, frameworki i silniki

Są to kawałki już napisanego przez kogoś kodu którego można użyć we własnych programach czy projektach. Biblioteki to kawałki kodu napisane przez innych programistów. Frameworki oznaczają trochę więcej, są to bardziej rozbudowane rozwiązania tworzące bazę na której umieszcza się swój kod. Silniki są to gotowe rozwiązania których można użyć od razu, można je też rozwijać i modyfikować do swoich potrzeb.

-   Direct X - 1995

Direct X jest podstawową biblioteką na której oparta jest masa gier na systemie Windows. Główna część biblioteki skupia się na wykorzystaniu możliwości kart graficznych. Ale Direct X oprócz części czysto graficznych takich jak Direct3D i Direct2D zawiera też kod ułatwiający obsługę sterowania padem DirectInput czy obsługę Audio. Dając pełen zestaw narzędzi na których mogą budować swój kod twórcy gier.

-   Open GL - 1992

Open GL jest "konkurencyjną" biblioteką. W odróżnieniu od DirectX Open GL jest biblioteką otwartą nie kontrolowaną przez Microsoft. Więc umożliwia wydawanie gier również na Linuxa albo MacOS. Skupia się wyłączeni na grafice. I ma inny model współpracy z kartą graficzną niż rozwiązanie Microsoftu. Jest spotykany rzadziej ale jest troche gier z grafiką opartą wyłącznie na OpenGL albo decydujących się na użycie obu bibliotek i dających wybór czy gracz woli skorzystać z wersji opartej na DirectX czy OpenGL.

-   Web GL - 2011

Web GL jest biblioteką graficzna przeznaczoną do środowisk webowych. Najczęściej będzie odpalony z Javascriptu. Umożliwi on aplikacjom webowym wykorzystanie możliwości nowoczesnych kar graficznych i tworzenie rozbudowanej grafiki w grach przeglądarkowcyh.

- Vulkan - 2016

Nowe biblioteki do komunikacji z kartą graficzną która mają zastąpić OpenGL i DirectX. Vulkan charakteeryzuje się przenośnością i dużą troską o wydajność. Nie przeszkadza mu bycie skomplikowanym dla nowych developerów. Warto śledzić projekt bo ma duży potencjał i zyskuje popularność zwłaszcza w obszarach takich jak gamedev czy VR gdzie wydajnosc mozliwosć wykorzystania potencjału nowinek technnicznych mają duże znaczenie.


## Silniki

-   Unity (3D) - 2005

Unity jest popularnym silnikiem. Z racji relatywnie łatwego startu jest cząsto polecany początkującym. Rozbudowany edytor, duża ilość tutoriali, rozszerzeń i zasobów na wewnętrznym rynku (marketplace) to duże zalety tego rozwiązania. Niestety kod samego silnika nie jest dostępny bez wykupienia drogiej licencji, co może być problemem dla niektórych projektów. Skrypty oparte najczęściej na C# umożliwiają tworzenie rozbudowanej logiki gry, pomimo braku możliwości ingerencji w kod źródłowy, więc sama logika gry moze być bardzo złożona.

[https://en.wikipedia.org/wiki/List_of_Unity_games](https://en.wikipedia.org/wiki/List_of_Unity_games)

-   Unreal Engine 4 - 2014

Firma Epic Games stworzyła silnik do swoich gier Unreal i Unreal Tournament. Silnik tamtych gier pozwalał na duże możliwości modowania i wiele zespołów było zainteresowanych wykorzystaniem silnika we własnych produkcjach. Wersja 3 silnika była bardzo często licencjonowana przez różne firmy do tworzenia własnych tytułów, dla amatorów była dostępna ograniczona wersja UDK w której również mogli pobawić się możliwościami silnika. Jednak prawdziwy przełom nastąpił w silniku w wersji 4 - cały kod silnika jest publicznie dostępny, a amatorzy mają równie dobry dostęp do całości silnika jak duże firmy. Silnik jest napisany w c++, nie posiada języka skryptowego... ale posiada wbudowany w edytor wizualny język Blueprint który umożliwia tworzenie logiki gry bezpośrednio w edytorze. Nie polecam tworzenia tak dużych projektów ale do protypowania jest to idealne, a jak rozwiązanie będzie fajne można je przenieść do c++. Ten c++ w unrealu jest bardzo specyficzny, bo kod musi się integrować z narzędziami przygotowanymi przez firmę epic. Ale duże ilości poradników do tego c++ jak i do masy funkcji oferowanych w samym edytorze ułatwiają naukę tego olbrzymiego narzędzia.

[https://en.wikipedia.org/wiki/List_of_Unreal_Engine_games](https://en.wikipedia.org/wiki/List_of_Unreal_Engine_games)

- inne np Godot, silniki różnych studiów do gier AAA, małe silniki mniejszych studiów dostosowane pod konkretne projekty albo serie, silniki robione przez pasjonatów jako hobby

[Silniki Przyjazne Amatorom Lista](https://gamedev-pl.fandom.com/pl/wiki/Silniki_Przyjazne_Amatorom_Lista "Silniki Przyjazne Amatorom Lista")

## Frameworki

DirectX i OpenGL są dość niskopoziomowe. Istnieje więc wiele rozwiązań, które je opakowują w prostsze do użycia kawałki, dodają obsługę różnych formatów plików itp. itd. Jeśli chodzi o dostępne za darmo silniki Unity i UE zdecycydowanie nie są jedynymi. Są najpopularniejszymi dużymi narzędziami. Sporo firm tworzy też własne rozwiązania. Część z nich jest dostępna dla amatorów w formie samego edytora, czy innych narzędzi umożliwiających korzystanie z silnika w ograniczonym zakresie do własnych projektów albo modów.

Np cocos2d, phaser, ogre

[TODO: dodać jakieś frameworki]

## Algorytmy

Pod spodem każdego systemu informatycznego są jakieś pomysły na to jak coś mogłoby działać. Algorytm oznacza przepis, jest on generalnie niezależny od języka czy biblioteki. Ale oczywiście ten pomysł w innym języku i na innych bibliotekach będzie wymagał trochę innego kawałku kodu.

Na start najczęstszymi algorytmami są sposoby na posortowanie listy/tablicy liczb. Jest to dość mało fascynujący temat, ale pokazuje różnych sposobów na osiągnięcie tego zadania jest całkiem sporo. Różnią się one bardzo mocno. Niektóre wymagają bardzo złożonego kodu. Zachowują się różnie w różnych przypadkach. Mogą drastycznie różnić się wydajnością. A wszystkie dają na końcu ten sam wynik.

O ile samo sortowanie nie jest specjalnie ciekawe to ma zastosowanie w wielu różnych dziedzinach. A uczenie się algorytmów pozwala zrozumieć zagadnienia związane z wydajnością kodu.

Poza tym wszystkie biblioteki i silniki opierają się na algorytmach które ktoś za nas napisał, wiec znajomość tych sposobów pozwala na ocenę, które obiekty w grze jak się zachowają. Pozwala na dopisywanie nowych zachowań, których nie uwzględniono w narzędziu. A raz na jakiś czas taka wiedz może być potrzebna do napisania naszej logiki gry np kodu zagadki logicznej albo zaprojektowania AI przeciwnika.

Przydatna jest też znajomość matematyki, zwłaszcza geometrii obliczeniowej w 3d. Bo często trzeba wydajnie policzyć np jak daleko są obiekty od siebie, czy dany obiekt znajduje się po lewej czy po prawej itp. itd.

Podstawowa wiedza z fizyki, zwłaszcza mechanika newtonowska, pojawia się często przy symulacji ruchu czy to jednostki czy np kamery.

Po poznaniu podstaw umiejętności algorytmiczne można szlifować na serwisach typu [https://www.hackerrank.com/](https://www.hackerrank.com/) które mają duże biblioteki małych zadań o różnym stopniu trudności. Pozwalają wysłać rozwiązania w wielu językach i zweryfikują poprawność i czas działania rozwiązania.

## Narzędzia i sposoby organizacji kodu

Kodu bardzo szybko robi się dużo i robi się w nim straszny bałagan. W pracy z taką ilością tysięcy linii technicznych hieroglifów bardzo przydają się dobre narzędzia. Zwłaszcza że często nie pracujemy sami, tylko z innymi programistami. Kod częściej jest czytany niż pisany. A mimo że każdy ciągle zmienia inny kawałek chcemy żeby całość rozwiązania sprawnie działała.

Pierwszy program który jest niezbędny to kompilator - jest to program który przeczyta kod i wygeneruje z niego program albo bibliotekę. W nowoczesnych narzędziach kompilator pracuje sobie gdzieś pod spodem i często programista nie zwraca na niego bezpośrednio uwagi tylko czyta ew. błędy jeśli proces się nie uda.

Do czytania i modyfikacji tych tysięcy linii kodu potrzebny jest edytor. Niby można pisać kod w notatniku ale jest to bardzo słaby pomysł. Nowoczesne edytory dają dużo więcej wsparcia programiście - pokolorują składnię żeby kod był czytelniejszy. Podświetlą błędy od razu zanim program zostanie wysłany do kompilacji. Umożliwią łatwe przeskakiwanie między powiązanymi częściami kodu. Mają dużo ułatwień przy generowaniu kodu, podpowiedzą jakie są dostępne funkcje i zmienne, ułatwią wygenerowanie standardowych fragmentów. Pomogą też w najczęściej spotykanych przeróbkach. Pozwalają konfigurować i odpalać kompilację. A potem pomagają w szukaniu błędów [debug] czy odpalaniu testów automatycznych (unit test)

Najczęściej instaluje się od razu całe IDE (Integrated desktop Environment) czyli całe środowisko. Kompilator, edytor i masę dodatkowych narzędzi przydatnych przy pracy z kodem. W grach najpopularniejszym IDE będzie visual studio [https://visualstudio.microsoft.com/](https://visualstudio.microsoft.com/) z którego dzięki nowej polityce microsoftu amatorzy mogą korzystać za darmo w wersji Community. VS wspiera wiele popularnych języków w tym C++ i C#.

Furorę robi też inny produkt microsoftu - Visual Studio Code - jest to dużo lżejsza wersja pakietu dla programistów. Ale zawiera bardzo rozbudowany mechanizm wtyczek. Jest dostępna też na systemach linux i MacOS. I wspiera wiele języków w tym takie z którymi "duże" Visual Studio nie współpracuje. Wielu ceni też mniejsze zużycie zasobów i większą możliwość konfiguracji.

Kolejny zestaw narzędzi to systemy kontroli wersji. Te rozwiązania chronią programistów przed sytuacją gdzie zniknie jakiś kluczowy plik. Umożliwiają też podgląd co, kiedy i gdzie się zmieniło w plikach. Pozwalają wielu programistom pracować na tej samej bazie kodu, ułatwiając nakładanie zmian od innych osób i wymienianie się kodem. Najpopularniejszy system kontroli wersji to niewątpliwie git [https://git-scm.com/](https://git-scm.com/). Jest on troche skomplikowany ale warto się go poduczyć. Nawet lokalnie do własnych projektów daje on dużo możliwości. A praca w większym zespole programistów bez tego narzędzia to koszmar. Można z niego korzystać wpisując polecenia z linii komend, ale dużo edytorów integruje się z gitem i pozwala na wykonywanie akcji z samego edytora. Jest bardzo popularny zwłaszcza w połączeniu z usługą typu [https://github.com/](https://github.com/) która pozwala dzielić się kodem z całym światem. Jest ona bardzo oppularna dla wszystkich otwartych projektów w tym większości bibliotek.

W branży gier popularny jest też system kontroli wersji Perforce (P4, P4V). Jednak jest to rozwiązanie komercyjne i ma dużo mniejsze możliwości jeśli chodzi o pracę z kodem niż git. Nawet jeśli w firmie używany jest P4 polecam do kodu i tak używać git'a.

Kiedyś popularne było rozwiązanie SVN, jest to system prostszy od gita. Ma niestety wiele wad dlatego polecam jednak nauczyć się gita, a o SVN zapomnieć. Jeszcze starszym systemem był CVS ale on został kompletnie zastąpiony przez SVN więc nie ma sensu do niego wracać.

Wraz z rozwojem kodu szybko robi się bałagan. Zmiany w jednym miejscu potrafią popsuć zupełnie inny kawałek. A sterowanie przepływa w bardzo trudny w zrozumieniu sposób i nie wiadomo jak zabrać się do modyfikacji. Na takie problemy napotykają wszyscy programiści i przez lata zebrało się dużo poradników i zasad jak pisać kod żeby bałagan był mniejszy, dało się łatwiej użyć danego kawałka kodu w następnym projekcie, a zmiany było łatwiej wprowadzać i żeby nie psuły innych kawałków. Część z tych porad dotyczy konkretnych technologii, część jest ogólna i sprawdza się w dużej gamie technologii i projektów.

Generalnie chodzi o to żeby dobrze dzielić kod na kawałki. Dbać o to żeby kawałki były małe, dobrze określone i nie miały dziwnych niepotrzebnych zależności. Te porady często są ubierane w akronimy takie jak DRY, KISS, YAGNI, SOLID.

DRY - don't repeat yourself - nie powtarzaj się - jeśli ciągle cos kopiujesz to pewnie powinieneś to wrzucić do jakieś wspólnej funkcji

KISS - keep it simple stupid - użyj prostej wersji głupku - programiści mają tendencję do robienia bardziej skomplikowanych rozwiązań niż potrzebne, zasada przypomina że proste działające rozwiązania są najlepsze

YAGNI - you aint gonna need it - nigdy tego nie użyjesz - programiści często dodają obsługę wielu wariantów zanim ktokolwiek ich użyje, takie podejście często niepotrzebnie komplikuje system, zasada przypomina o unikaniu takich niepotrzebnych komplikacji

SOLID - to jest przypominajka o 5 różnych zasadach projektowania obiektów, każda z tych 5 zasad wymaga kilku akapitów komentarza więc tego tu nie opiszę

Na koniec często zaniedbana ale bardzo przydatne narzędzie. Testy automatyczne. Pisanie kodu jest trudne, nawet najlepsi programiści popełniają masę błędów często w najprostszym kodzie. Dlatego programy wymagają intensywnego testowania. Testowanie ręczne zajmuje masę czasu, często jest koszmarnie nudne i łatwo nie sprawdzić nawet głównych istotnych przypadków... a co dopiero warunków brzegowych. Dlatego wszędzie gdzie jest to możliwe warto napisać testy automatyczne. Jest to kawałek kodu który wykona jakiś inny kod i sprawdzi czy wynik jest taki jak oczekiwano. Nowoczesny edytor umożliwia szybkie puszczenie nawet bardzo dużej ilości takich testów. Dzięki temu natychmiast dowiemy się że cos jest nie tak jak chcieliśmy i można poprawić kod (albo test). Dobrze zaprojektowany zestaw testów uchroni programistę przed wieloma głupimi błędami które mogą mieć poważne konsekwencje i pozwoli skupić się na szukaniu bardziej skomplikowanych przypadków ręcznie. Taki zestaw jest też niezastąpiony po wprowadzeniu zmian organizacji kodu i przyspieszaniu algorytmów(refaktor i optymalizacja). Takie miany nie powinny wpływać na wynik obliczenia. Dobrze zrobiony zestaw testów wyłapie pomyłki przy refaktoringu i przy optymalizacji.