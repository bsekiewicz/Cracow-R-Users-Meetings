**Opowiedz prosz� kr�tko, czym si� na co dzie� zajmujesz?**

W mojej codziennej praktyce zawodowej ��cz� obowi�zki biostatystyka, projektanta oprogramowania i programisty.

Biostatystyk zajmuje si� statystyczn� analiz� danych p�yn�cych z medycznych bada� naukowych w ramach tzw. "medycyny opartej na dowodach". Obecnie poruszam si� w dziedzinie badawczych eksperyment�w medycznych zwanych "badaniami klinicznymi", poszukuj�c odpowiedzi na pytanie czy dana terapia jest skuteczna i bezpieczna. Podpis biostatystyka wie�czy zar�wno statystyczn� cz�� protoko�u ("Biblii") badania jak r�wnie� ko�cowy raport statystyczny, bez kt�rego proces dopuszczenia terapii do stosowania nie mo�e zosta� zako�czony. Biostatystyk wspiera r�wnie� dzia� Zarz�dzania Danymi oraz klinicyst�w w procesie monitorowania poprawno�ci i kompletno�ci wprowadzonych danych. Czasem wciela si� tak�e w rol� detektywa pomagaj�c badaczom zrozumie� przyczyny zaistnia�ych nieprawid�owo�ci.

Opr�cz analizy danych zajmuj� si� tak�e projektowaniem i tworzeniem specjalistycznego oprogramowania "bran�owego". S� to zar�wno proste narz�dzia wspieraj�ce proces monitorowania jako�ci danych jak r�wnie� bardziej z�o�one systemy wst�pnej ich analizy i raportowania. Warto nadmieni�, �e praktycznie ka�dy biostatystyk jest r�wnie� programist�: analizy wymagaj� znacznej bieg�o�ci w j�zykach programowania zwi�zanych z u�ytym oprogramowaniem analitycznym (R, SAS, SPSS, itd.). Kluczowa jest tak�e dobra znajomo�� SQL.

**Co w kontek�cie analizy danych wyr�nia bran��, w kt�rej pracujesz?**

Analiz� danych w ramach bada� klinicznych scharakteryzowa�bym dwoma s�owami: "rygoryzm" i "odpowiedzialno��". Je�li nie ograniczymy si� do bada� eksperymentalnych, doda�bym tak�e "pogo� za moc�".

***Rygoryzm***, poniewa� badania kliniczne charakteryzuj� si� d��eniem do uregulowania wszystkiego, co tylko mo�e zosta� uregulowane. Wszystko odbywa si� wedle wytycznych (np. wytyczne ICH), Standardowych Procedur Operacyjnych (SOP), szablon�w (TFL) z uwzgl�dnieniem tzw. "Dobrej praktyki klinicznej" (GCP). Ka�dy krok jest sprawdzany pod k�tem zgodno�ci z SOP. A wszystko to pod rygorem uniewa�nienia ca�ego badania. Przypominaj� mi si� w tym momencie sceny z film�w katastroficznych, gdzie w obliczu zagro�enia, pilot si�ga najpierw po ksi�g� procedur.

***Odpowiedzialno��***, poniewa� pomy�ka i niefrasobliwo�� mog� kosztowa� czyje� zdrowie - tu za ka�d� analizowan� liczb� stoi �ywy cz�owiek. "Walidacja" - s�owo-klucz, kt�re pojawia si� co chwil�, na ka�dym kroku. Krytyczne fragmenty program�w  sprawdzane s� przez niezale�nego analityka, a nierzadko tak�e zewn�trznych ekspert�w.

***Pogo� za moc�*** - chocia� termin ten nie dotyczy bada� stricte klinicznych (s� dok�adnie zaplanowane "na najgorszy mo�liwy wariant"), to jest on nieod��czn� zmor� wielu bada� dotycz�cych rzadkich chor�b i zjawisk. Nierzadko zdarzaj� si� retrospektywne badania o donios�ym znaczeniu, generuj�ce pr�by o liczebno�ci "nastu" obserwacji, z kt�rych trzeba uzyska� maksymalnie du�o informacji. W sytuacji, gdy �wiat zach�ysn�� si� terminem "Big data", w medycynie nadal kr�luje niepodzielnie "Small data" przez du�e "S".

**Opowiedz kilka zda� o tym o czym b�dziesz opowiada� podczas najbli�szego spotkania**

�ycie pisze najlepsze scenariusze. W firmie, w kt�rej pracuj�, pojawi�o si� zapotrzebowanie na mechanizm generuj�cy bardzo wa�ne raporty. R�czne przygotowanie takiego raportu to droga przez m�k�. Zachodzi�o ryzyko, �e raport b�dzie nieaktualny ju� w momencie jego tworzenia.

Zasugerowa�em wykonanie systemu dostarczaj�cego takie raporty w ci�gu sekund. Musia�em podj�� decyzj� z jakiej technologii skorzysta�. Jako programista .NET pocz�tkowo my�la�em nad webserwisem pod��czonym konektorem do R. W efekcie analizy moich do�wiadcze� stwierdzi�em, �e wprowadzanie dodatkowych warstw po�rednicz�cych i ci�kiego b�d� co b�d� frameworka to stosowanie armaty na much�. Za du�o konfiguracji, za du�o zachodu, konieczno�� zatrudnienia dodatkowego programisty C#. Praca serwerowa R pod Windows te� nie napawa�a optymizmem. Zdecydowa�em si� �p�j�� na ca�o�� i wykona�em taki system ca�kowicie w R.

Na spotkaniu chcia�bym om�wi� r�ne aspekty wykorzystania R i platformy OpenCPU do zbudowania niewielkiego (50-100 u�ytkownik�w) systemu raportuj�cego dla firmy. Do osi�gni�cia prostych cel�w wystarcz� proste rozwi�zania. Niestety, jest to okupione pewnymi niedogodno�ciami i haczykami, o kt�rych chcia�bym opowiedzie�.

**Dlaczego w�a�nie taki temat?**

Troch� z przewrotno�ci - "patrzcie, oto kolejna rzecz, jak� mo�na zrobi� w R". Troch� z zadowolenia, �e to naprawd� dobrze dzia�a i chcia�bym podzieli� si� tym z innymi. A wreszcie - poniewa� to moja ma�a cegie�ka w promowanie zastosowa� R w firmach.

**Jakie s� wed�ug Ciebie najwi�ksze zalety R?**

Takie pytanie grozi wielogodzinnym wyk�adem :)

A powa�nie - pot�g� R jest to:

- jakie posiada mo�liwo�ci - dost�pne s� biblioteki praktycznie do wszystkiego, tak w zakresie statystyki (praktycznie ka�dy rodzaj modelu) jak i regularnego programowania
- �e jest darmowy, jednak�e w razie potrzeby mamy do dyspozycji tak�e komercyjne wersje firm trzecich (np. RStudio, TIBCO)
- �e jego u�yteczno�� zosta�a dostrze�ona i doceniona przez tak wielkich graczy, jak Oracle czy Microsoft. MS R Server, MS Power BI, Oracle Enterprise - to brzmi dumnie!
- �e ma otwarty kod, kt�ry mo�na przejrze�, nauczy� si� czego� i �atwiej wy�apa� potencjalne b��dy
- �e nad jego rozwojem pracuj� t�gie profesorskie g�owy z solidnym do�wiadczeniem w zakresie (bio) statystyki
- �e mo�na go uruchomi� na Raspberry PI, Androidzie, a by� mo�e i jakiej� lod�wce... Otwiera to szerokie mo�liwo�ci w zakresie tworzenia dedykowanych rozwi�za� analityczno-kontrolno-pomiarowych
- �e "rozmawia" z SAS pozwalaj�c zaoszcz�dzi� sporo pieni�dzy!
- �e ma pot�n�, aktywn� spo�eczno�� gotow� do pomocy cz�sto szybciej i sprawniej ni� najlepszy komercyjny helpdesk
- �e pozwala tworzy� zar�wno z�o�one oprogramowanie analityczne, jak r�wnie� sprytne "kieszonkowe" narz�dzia
- �e wiele rzeczy mog� wykona� na N sposob�w, niemal ka�dy programista R ma swoje ulubione konstrukcje
- �e potrafi odczyta� i zapisa� dane w tak wielu formatach
- �e posiada bibliotek� do operowania SQLa na poziomie ramek danych. I �e mog� korzysta� z R w PostgreSQL lub MS SQL
- �e nawet jego najwi�ksi konkurenci (SAS, SPSS, Statistica) dostarczaj� konektory do R
- �e stanowi mix paradygmat�w: tablicowy, obiektowy, imperatywny, funkcjonalny, proceduralny, refleksyjny. W efekcie dostajemy do r�k pot�ne narz�dzie programistyczne
- �e posiada najwi�cej bibliotek do tworzenia profesjonalnych tabel i grafik do publikacji "klinicznych"

Po wi�cej (znacznie!) zapraszam do prezentacji www.r-clinical-research.com

**Z drugiej strony, jakie s� najwi�ksze wady tego j�zyka?**

- R zosta� stworzony przez statystyk�w dla statystyk�w, a nie przez zawodowych projektant�w i programist�w. Nie k�adziono specjalnego nacisku na dopracowanie, ujednolicenie j�zyka, optymalizacj�. Konstrukcje w rodzaju try-catch, obiektowo�� - wygl�daj� tam nieco sztucznie, jakby "doczepione" troch� na si��.
- Brak centralnego "zarz�dzania jako�ci�". Pakiety s� tworzone w bardzo dowolny spos�b, ich zachowanie nie podlega standardom. Istniej� oczywi�cie "zalecenia" i "dobre praktyki", ale trzeba si� do nich jeszcze stosowa�. Brak centralnej walidacji pakiet�w (cho� autorzy cz�sto dostarczaj� testy jednostkowe) sprawia, �e u�ywamy ich na w�asne ryzyko. W przypadku popularnych pakiet�w rekompensuje to silna, aktywna i �wiadoma spo�eczno��, kt�ra b�yskawicznie wy�apuje i raportuje b��dy. Jest to bardzo powa�ny zarzut w bran�y bada� klinicznych!
- Wspomniany mix paradygmat�w sprawia, �e programy w R mog� by� pisane w spos�b bardzo zr�nicowany. Z moich do�wiadcze� trenera wynika, �e sprawia to powa�ny problem pocz�tkuj�cym, kt�rzy dopiero poszukuj� swojego stylu i cz�sto nie potrafi� sprawnie odczyta� program�w napisanych przez innych. Problem ten jest w R widoczny daleko bardziej ni� w innych j�zykach programowania
- Typowa dokumentacja przeci�tnego pakietu jest zaledwie spisem funkcji wraz z pobie�nym opisem ich u�ycia. Daleko jej do dokumentacji znanej np. z SAS. Na szcz�cie dla naju�yteczniejszych pakiet�w istniej� rozbudowane strony instrukta�owe (dplyr, ggplot2, ReporteRs, sqldf)
- R wymaga pewnych zdolno�ci programistycznych - bo to po prostu j�zyk programowania. Odstr�cza to wielu pocz�tkuj�cych. To nie Statistica, w kt�rej wszystko mo�na "wyklika�". Sytuacj� ratuje odrobin� np. RCommander lub Rattle

**Bior�c pod uwag� twoje do�wiadczenie, jakie s� najwi�ksze trudno�ci z wdra�aniem j�zyka R (lub og�lnie oprogramowania open-source) w medycynie i farmacji?**

S� tutaj dwa zasadnicze problemy, bardzo istotne i trudne do �przeskoczenia�.

Wspomniany brak centralnej instytucji kontroli i zapewnienia jako�ci. Najcz�stszy i najpowa�niejszy zarzut w mojej bran�y to "R nie podlega walidacji". Kto jest odpowiedzialny za ca�okszta�t R (= core + biblioteki)? Cz�ciowo The R Core Team, cz�ciowo autorzy bibliotek. SAS posiada oficjalny dzia� test�w, helpdesk, bierze odpowiedzialno�� za sw�j produkt. Do kogo zwr�ci� si� z pro�b� o pomoc albo... odszkodowanie? Licencja m�wi jasno - "na twoje w�asne ryzyko". W tak sformalizowanym �rodowisku jak Clinical Research jest to argument najci�szego mo�liwego kalibru. I dotyczy to ka�dego niekomercyjnego oprogramowania.

Dobrze zorganizowany, �wiadomy problemu dzia� biostatystyki rozwi�zuje te zagadnienia wprowadzaj�c wieloetapow� walidacj� wynik�w analiz przeprowadzanych w danym narz�dziu, zamra�aj�c wersj� u�ytych bibliotek i wprowadzaj�c repozytorium przetestowanych blok�w kodu (makr, procedur). Jest to bardzo szerokie i trudne zagadnienie. Ma�o kto chce je podj��, dlatego wygodniej wyda� kilkaset tysi�cy z�otych na SAS i spa� spokojnie.

Drugi problem to brak informacji. "Wszyscy u�ywaj� SAS, bo nie ma nic lepszego, wi�c my te� go u�yjemy". Informacja, �e istnieje darmowe oprogramowanie o nie tylko por�wnywalnych, ale miejscami du�o wi�kszych mo�liwo�ciach powoduje niek�amane zdziwienie mened�er�w. Najlepiej przemawiaj� do nich liczby. Koszt licencji SAS potrzebnych do stworzenia trzech solidnych stanowisk to wydatek rz�du kilkuset tysi�cy z�otych na rok. W tej bran�y "darmowy = niebezpieczny".

**Co robisz, kiedy nie analizujesz danych?**

W wolnych chwilach ratuj� od zapomnienia zabytkow� elektronik�, bez kt�rej nie by�oby tej dzisiejszej. Odkrywam na nowo rozwi�zania pionier�w elektrotechniki sprzed niemal wieku, przywracam do �ycia star� aparatur� kontrolno-pomiarow�, kolekcjonuj� zabytkowe i rzadkie podzespo�y i eksperymentuj� z lampami elektronowymi.

**I na zako�czenie, dla kogo jest to spotkanie i dlaczego warto przyj��?**

Spotkanie adresowane jest do os�b wdra�aj�cych rozwi�zania OpenSource w firmach, pracownik�w i mened�er�w dzia��w analitycznych pragn�cych poszerzy� horyzonty i wreszcie - dla pasjonat�w R.