# Pytania na egzamin v2.5
1. [Mieszanie neutrin](#mieszanie-neutrin)
2. [Detekcja fal grawitacyjnych](#Detekcja-fal-grawitacyjnych)
3. [Rekonstrukcja torów cząstek naładowanych w eksperymentach HEP](#Rekonstrukcja-torów-cząstek-naładowanych-w-eksperymentach-HEP)
4. [Sieci Bayesowskie](#Sieci-bayesowskie)
5. [Technologia informatyczna a fizyka - wpływ informatyki na fizykę, proszę omówić temat na wybranych przykładach](#Technologia-informatyczna-a-fizyka)
6. [Wyzwania stojące przed fizykiem eksperymentatorem, ze szczególnym uwzględnieniem eksperymentów z dużą liczbą naukowców](#Wyzwania-stojące-przed-fizykiem-eksperymentatorem)


# Mieszanie neutrin
(a.k.a. oscylacja neutrin)

## Historia neutrin 

Neutrino zostało początkowo postulowane przez Wolfganga Pauliego, w 1930 w celu wyjaśnienia rozpadu Beta. Z powodu kolizji nazw z neutronem, Enrico Fermi zaproponował neutrino.
W 1942 Wang Ganchang zaproponował użycie wychwytu elektronu (odwrotną przemianę beta) W 1956 Cowan–Reines przeprowadzono [eksperyment][1] w którym wykryto neutrino.

## Neutrina a model standardowy

Neutrino to fermion który wchodzi w interakcje tylko przez grawitacje oraz oddziaływania słabe.
Jedną z nierozstrzygniętych kwestii dotyczących neutrin jest to czy anty-neutrina i neutrina to ta sama cząstka (model majorana) czy też inna cząstka (model fermiego).
Antyneutrina powinny mieć  opposite-signed lepton number and weak isospin, and right-handed instead of left-handed chirality. 

![](https://i.imgur.com/LdTv4vw.png "Skrętnośc neutrin")

Rozróżniamy trzy stany zapachowe neutrin:
Neutrino elektronowe, neutrino mionowe, i neutrino tau.




### Eksperyment w Cowan–Reines 
(źrodło [wiki](https://en.wikipedia.org/wiki/Cowan%E2%80%93Reines_neutrino_experiment#Setup) )

Eksperyment potwierdzający istnienie neutrino bazował na obserwacji tzw wychwytu elektronu ( odwrotnej przemiany beta).

$\bar{\nu}_e + p \to n + e^+$

Gdzie antyneutrino elektronowe oddziałuje z protonem, produkując pozyton i neutron.

![diagram feymana wychwytu elektronu](https://i.imgur.com/kRPXR85.png =240x200)

(Pytanie, jak się zieniają kwarki?)

Jako źródło neutrin zastosowano reaktor jądrowy. Zastosowano dwa kontenery z wodą, przedzielone materiałem scyntylacyjnym. Gdy neutrino uderzało w proton, powstaje neutron i posyton. Pozyton reaguje z elektronem (anihilacja) emitując dwa fotony (gamma), które trafiają do fotopowielacza. Natomiast neutron jest wychwytywany jądrowo (?) i również produkuje foton (trzeci).

Atomy wodoru w molekułach wody są tarczą dla neutrin, więc użyto wody jako materiału detekcyjnego. Protony w wodzie są dość luźno połączone z molekułą. W przypadku jądra atomu tlenu wiązania są silne.

Przekrój czynny na interakce neutrina z wodą jest bardzo mały, ale w eksperymencie zastosowano reaktor jądrowy z dużym strumieniem. Zastosowano detektor składający się z dwóch zbiorników z wodą, "zakanapkowanych" płynnym materiałem scyntylacyjnym, który po wychwyceniu promieni gamma (zjawisko komptona) przewodził błysk do fotopowielacza.

W celu zarejestrowania trzeciego sygnału gamma, do zbiorników dodano chlorek kadmu $\ce{CdCl_2}$. Kadm bardzo dobrze wychwytuje neutrony, i produkuje sygnał gamma (po spowolnieniu neutronu przez wodę):

$n+\ce{^{108}_Cd}\rightarrow\ce{^{109m}_Cd}\rightarrow\ce{^{109}_Cd}+\gamma$

Eksperyment rejestrował najpierw sygnał (dwa fotony) z fotopowielacza pochodzące od anihilacji protonu i pozytonu, a kilka mikrosekund później sygnał (foton) pochodzący od neutronu.

Uzyto około 200 litrów wody i 40 kilo chlorku kadmu.

Autorzy eksperymentu otrzymali nagrodę nobla.

## Skrętność neutrin 

(chyba W eksperymencie Goldhabera, Grodzinsa i Sunyara w 1958 sprawdzono skrętność neutrin, i ) wykryto tylko lewoskrętne neutrina i prawoskrętne antineutrina.

## Masy Neutrin: neutrina Diraca i Majorany

W konwencjonalnym podejściu neutrina traktuje się jako cząstki Diraca. To jest cząstka która posiadające spin 1/2 wystepujące tylko w jednym stanie spinowym. Model majorana zaproponował że neutrino jest swoją własną ant-cząstką i jedną cząstkę o spinie 1/2 z dwoma skrętnościami $\nu_L$, $\nu_R$ (majorana narusza zachowanie leptonowości ?)

## Oscylacje

Na początku uważano że neutrina nie posiadają masy. Ta idea była podważana przez (Bruno) Pontecorvo i innych. Wysunięto hipotezę iż neutrina są produkowane lub anihilowane jako stany własne zapachu, ale propagują się w przestrzeni jako superpozycje stanów własnych operatora masy. Stany własne masy neutrin ($\nu_e$, $\nu_\mu$, $\nu_\tau$) są traktowane jako kombinajca liniowych stanów własnych ($\nu_1$, $\nu_2$, $\nu_3$), które propagują sie w przestrzeni z nieznacznie różnymi częstościami, co wynika z faktu że mają różne masy. Prowadzi to do zmiany względnych faz między stanami w zależności od pokonanej masy, co daje w efekcie oscylacje zapachu neutrin.

### Wywód oscylacji
W uproszczeniu, zakłądając dwa zapachy neutrin:

$\begin{pmatrix} \nu_\mu \\ \nu_e \end{pmatrix} =\begin{pmatrix}\cos\theta & \sin\theta \\
    -\sin\theta & \cos\theta
  \end{pmatrix} \begin{pmatrix} \nu_1 \\ \nu_2 \end{pmatrix}$
  
 (tutaj mnożenie wektorów)
 
 Ponieważ tą macierz można przedstawić jako macierz diagonalną (https://en.wikipedia.org/wiki/Neutrino_oscillation#Classical_analogue_of_neutrino_oscillation) to są to stany ortonormalne. Ich propagacje opisuja równania 
 
 $\nu_1(t)=\nu_1(0)e^{-ie_{1}t}$
 $\nu_2(t)=\nu_2(0)e^{-iE_{2}t}$
 
 Gdzie ($\hbar=c=1$) Stany własne mają ustalony pęd, więch ich masy spełniaja warunek $m_i<<E_i$ (?)(i={1,2}) to
 
 $E_i=p+\frac{m_i^2}{2p}$
 
 Dla neutrina mionowego w stanie początkowym $\nu_\mu(0)=1$ $\nu_e(0)=0$ i zatem $\nu_\mu(t) = \cos\theta\nu_1(t)+\sin\theta\nu_2(t)$
 
 
 Więc amplituda 
 $A_\mu = \frac{\nu_{\mu}(t)}{\nu_{\mu}(0)} = \cos^{2}\theta e^{-iE_{1}t}+\sin^{2}e^{-iE_{2}t}$
 
 I zatem prawdopodobiństoiw:
 
 $\frac{I_{\mu}(t)}{I_{\mu}(0)} = A_{\mu}A_{\mu}^{*} = 1 - \sin^{2}\theta \sin^{2}\frac{(E_2-E_1)t}{2}$ używając masy neutrin i usatalając $\Delta m^2 = m_2^2-m_1^2$:
 
 $P(\nu_\mu \rightarrow \nu_\mu) = 1 -\sin^{2}\theta\sin^2(\frac{1,27 \Delta m^2}{E})$
 
 $P(\nu_\mu \rightarrow \nu_e) = 1 - P(\nu_\mu \rightarrow \nu_\mu)$
 
![](https://i.imgur.com/VGyzJAG.png)

### Macierz PMNS
Macierz PMNS to macierz mieszania neutrin, to analogia do macierzy CKM. Opisuje się mieszanie trzech stanów własnych masy neutrin. 

![](https://i.imgur.com/QkawnGn.png)

Przy czym ostatnia macierz ma znaczenie wtedy jeśli neutrino jest majorana.

[wiki](https://en.wikipedia.org/wiki/Neutrino_oscillation#Pontecorvo%E2%80%93Maki%E2%80%93Nakagawa%E2%80%93Sakata_matrix)

Pontecorvo–Maki–Nakagawa–Sakata matrix

## Oscylacje a eksperymenty i obserwacje

Doświadczalne pszukiwania oscylacji neutrin prowadzone sa od lat. Dotychczas tylko jedno laboratorium wykonujące pomiary na wiązce ogłosiło pozytywny wynik.

### Eksperymenty

Prawdopodobieństwa zachowania zapachu $P(\bar{\nu_\alpha} \rightarrow \bar{\nu_\alpha})$ oraz $P(\nu_\alpha \rightarrow \nu_\alpha)$ (gdzie indeks dolny oznacza dowolny zpach neutrin) są równe, i wynika to z CPT. Jednak przejście $P(\bar{\nu_\alpha} \rightarrow \bar{\nu_\beta})$ jest różne od $P(\nu_\beta \rightarrow \nu_\alpha)$ i $P(\nu_\alpha \rightarrow \nu_\beta)$. Wynika to z niezachowania CP. W doświaczczeniach laboratoryjnych posługiwano się wiązkami $\bar{\nu_e}$ z reaktora i wiązkami $\nu_\mu, \bar{\nu_\mu}$ z akceleratorów.
Wiązki reaktorowe mają niskie energie (10MeV), przy szybkości zdarzeń dla procesu rejestracji neutrin to 5MeV. Wynika stąd że takich wiązek można używać w doświadczeniach mierzących zanikanie początkoweego zapachu, ponieważ nawet w przypadku wystąpienia przejścia (anty-neu ele do anty-neu mio) energia neutrina jest mniejsza niż progowa na produkcje mionu (t.j. mion nie może zostać wyprodukowany bo nie wystarcza na niego energii).

#### Eksperyment CHOOZ

W eksperymencie jako tarczy użyto 5 ton materiału scyntylacyjnego, domieszkowanego gadolinem, otoczonego obudową o masie 17 ton. Tarcza posiadała fotopowielacze. Całość była zamknięta w dodatkowej komorze, o opodobnej kompozycji w celu eliminacji tła mionowego z promieniowania kosmicznego. Detekto zamknięty był w stalowym zbiorniku umieszczonym pod grubą warstwą skał, w odległości 1km od dwóch reaktorów o łącznej mocy 8GW. 
Eksperyment w chooz włożył wkład na element macierzy PMNS $U_{e3}^2<0.03$ (jest tez druga opcja 0.97 wykluczona przez neutrina słoneczne) ([wiki](https://en.wikipedia.org/wiki/Chooz_(experiment))).


### Neutrina słoneczne

W eksperymentach nieakceleratorowych, korzystających z naturalnych źródeł neutrin zaobserwowano eefekty które można zinterpretować jako przejawy oscylacji neutrin.

Najważniejszą reakcja produkujacą neutrina jest reakcja pp (a.k.a Cykl Protonowy [wiki](https://en.wikipedia.org/wiki/Proton%E2%80%93proton_chain) -- fuzja jądrowa)

Jest to łańcuch reakcji , gdzie finalnie na każde 25 MeV energi słoneczej produkowane są dwa neutrina. 

Sygnały neutrin słonecznych zerejestrowały cztery duże eksperymenty. Detektory radiochemiczne SAGE oraz GALLEX zaweirały dziesiatki ton galu, charakteryzująego się niska energią progową dla reakcji $\nu_e + \ce{{}^{37}Ga}  \rightarrow \ce{{}^{37}Ga} + e^-$ Całkowita częstośc zdarzeń zdarzeń jest równa 55 $\pm$ 5% częstości obliczonej na podstawie standardowego modelu słonecznego. (Detektor był kalibrowany sztucznym źródłem neutrin.)

Neutrina słoneczne obseruje takze Kamiokande i SuperKamiokande, w których wodne liczniki Czerenkowa rejestruja elektrony odrzucane w wyniku procesu rozpraszania elastycznegi $\nu_e+e^- \rightarrow \nu_e+e^-$. Eksperyment jest czuły na neutrina pochodzące z rozpadu $\ce{{}^8B}$ (Boron). Obserwowana częstość jest równa około 40%.

Deficyt neutrin moze mieć kilka przycyn, mogą to być niedostatki modelu słonecznego. Możliwe że coś dzieje sie z neutrinami na drodze z jądra Słońca na Ziuemie. Preferowanym wyjaśnieniem jest mieszanie neutrin.

### Neutrina atmosferyczne

Porównując stosunek 

$R = \frac{(N_\mu/N_e)_obs}{(N_\mu/N_e)_oolicz}$ okazuje się że pięć niezlaeżny eksperymentów wszystkie dały R<1. Pryz średniej wartości $R ~ 0.6$. Rezulatat ten interperetowano w kategoriach oscylacji $\nu_\mu \rightarrow \nu_\tau$

Bardziej przekonywujący jest rozpad mionów z energiami wyższyczmi niż 1,3 GeV powstajacych w wniku odzdiaływań $\nu\mu$, w funkcji kąta zenitalnego. Długość drogi neutrina w materi L sinlie zależ od ąta zenitalnego i wynosi 20km dla neutrin giegnących ponowo w dół, 200 km dla neutrin wzdłuż horyzontu i 10 tys km dla neutrin docierających do atmosfery z drugiej strony ziemi.

Te obserwacje można zinterpretować w kategorii oscylacji neutrin.

Aby dowieść istnieneia oscylacji neuytring koniecznie jest zaobserwowaenie pełnego okresu oscylacji, takie doświadczenie można przypuszczalnie dowieść jedynia za pomocą kontrolowanych wiązek z akceleratorów i reaktorów. ponieważ skala odległości w ekspeymentach atmosferycznych i słonecznych to 10^3 - 10^8 km uzyskanie takiego dowodu będzie raczej dosć trudnym zadaniem.
 
 
[1]: https://en.wikipedia.org/wiki/Cowan%E2%80%93Reines_neutrino_experiment#:~:text=Cowan%20and%20Stevens%20Institute%20of,decay%20processes%20in%20the%201930s.
# Fale grawitacyjne

## Historia

Einstein 1915 równania pola
1916 einstein przewiduje fale grawitacyjnne

1970.1980 Hulse-taylor obserwacja pulsara (arecibo) z rozpadem orbity zgadzającym się z przewidywaniami uwzględniającymi stratę energi na fale grawitacyjne

2015 - bezpośrednia obserwacja - LIGO

2017 - Rainer Weiss, Barry Barish and Kip Thorne nagroda nobla za detekcje [artykuł][grawitacja-nobel]

## Równanie einsteina 

Równanie einsteina opisuje ogólną teorię względności, i relacje pomiędzy pędem/energią a czasoprzestrzenią [wiki][3].

$R_{\mu \nu} - \frac{1}{2} R g_{\mu \nu}= \frac{8\pi G}{c^4} T_{\mu \nu}$

Również $G_{\mu \nu} + \Lambda g_{\mu \nu} = \kappa T_{\mu \nu}$, gdzie G to tensor einsteina.
W całości razem ze stałą kosmologiczną:
$R_{\mu \nu} - \tfrac{1}{2} R\, g_{\mu \nu} + \Lambda g_{\mu \nu} = \kappa T_{\mu \nu}$ Jednak stała kosmologiczna jest często pomijana, ponieważ zakładamy że wszechświat się rozszerza (ze stałą prędkością).

Jest to opisowe równanie, potwierdzone przez obserwacje ([video][2]).

## Elementy równiania einsteina

$g_{\mu \nu}$ - tensor metryczny [wiki][4]. Dla pustej przestrzeni jest to tensor minkowskiego $\eta$, dla masy sferycznej masy jest to metryka Schwarzschild'a. Tensor metryczny określa metrykę na rozmaitości, i opisuje jak się rozmaitośc zachowuje.

$\Gamma^\alpha_{\mu \nu}$ - Symbol Christoffel'a [wiki][5] opisują składową zmiany w rozmaitości ($\frac{\overrightarrow{de_1}}{dx^0}$ rzutowane na wektor początkowy). Możemy dzięki temu obliczyć linię geodezyjną. Symbole christofela możemy pozyskać używając tensora metrycznego.

$R^\alpha_{\mu \nu}$ Tensor krzywizny Riemanna [wiki][6]. Opisuje różnicę pomiędzy dwiema pochodnymi wektora basowego w przeciwnej kolejności (e.g. $\overrightarrow{R} = \frac{d}{dx^\mu}\frac{d}{dx^\nu}\overrightarrow{e_\beta}-\frac{d}{dx^\nu}\frac{d}{dx^\mu}\overrightarrow{e_\beta}$). Innymi słowy, opisuje jak poruszając się po różnych osiach rozmaitości zmienia się wektor. Można opisać używają symboluy Christoffel'a

$R_{\mu \nu}$ Tensor Ricciego [wiki][7]. Można utworzyć na podstawie tensora Krzywizny reimanna sumując odpowiednie komponenty ($R_{\mu \nu} = R^\lambda_{\mu\lambda\nu}$). W ujęciu intuicyjnym tensor ricciego opisuje jak zmienia się objętość w przestrzeni przy poruszaniu się po jej krzywiźnie (np dystans pomiędzy południkami), lub jak bardzo geometria różni się od euklidesowej.

$R$ Skalar Ricciego [wiki][8]- charakteryzuje krzywizny we wszystkich kierunkach

$T_{\mu \nu}$ to tensor energii-pędu opisuje materię (pęd i energie)

## Rozwiązywanie równań einsteina (bonus)

1. Wybieramy metrykę czasoprzestrzeni (minkowski - pusta przestrzeń, Schwarschild - sferyczne statyczne masy, morris-thorne - wormhole)
2. Wybieramy typ współrzędnych (kartezjańskie, sferyczne itp)
3. Znajdujemy symetrie (np krążenie księżyca wokół ziemi wystarczy rzut 2d)
4. obliczamy po kolei tensor ricciego

jedno opcja to poszykiwanie prędkości lub linii geodezyjnych, można też przejść tą ścieżke odwrotnie dobierając T i wyliczając ztego metrykę



## Teoria Fal grawitacyjnych

A więc zaczynamy od czasoprzestrzeni ([wykłady][9], [video 1][10], [video 2][11]) która różni sie od minkowskiego tylko nieznacznie:

$g_{\mu\nu} = \eta_{\mu\nu} + h_{\mu\nu}$, gdzie $||h_{\mu\nu}|| <<1$ oraz pochodna $h_{\mu\nu}$ jest bliska zero.

Wyznaczając tensor Einstein'a (po długich obliczeniach, używając powyższego równania na tensor metryczny tworzymy symbole christofela, z symboli tensor riemanna) dochodzimy do formy:

$G_{\mu\nu} = \frac{1}{2} (
\partial^{\alpha}\partial_{\mu}\bar{h_{\alpha\nu}} + \partial^{\alpha}\partial_{\nu}\bar{h_{\mu\alpha}} - \eta_{\mu\nu}\partial^{\alpha}\partial^{\beta}\bar{h_{\alpha\beta}} -\partial^{\alpha}\partial_{\alpha}\bar{h_{\mu\nu}} )$

Możemy dokonać zamiany współrzednych tak że każdy element opródz ostatniego będzie równy zero. Tj z warunkiem cechowania (lorentza) $\partial_{\mu}\bar{h}^{\mu\nu} = 0$:

$G_{\mu\nu} = \frac{1}{2} (
0 + 0 - 0 -\partial^{\alpha}\partial_{\alpha}\bar{h_{\mu\nu}} )$ oraz $\partial^{\alpha}\partial_{\alpha}\bar{h_{\mu\nu}}=\Box\bar{h_{\mu\nu}}$ gdzie $\Box$ to delambertjan

Delambertjan:
$\Box = \partial^\mu \partial_\mu = \eta^{\mu\nu} \partial_\nu \partial_\mu = \frac{1}{c^{2}} \frac{\partial^2}{\partial t^2} - \frac{\partial^2}{\partial x^2} - \frac{\partial^2}{\partial y^2} - \frac{\partial^2}{\partial z^2}$

W związku z tym że patrzymy na pustą przestrzeń $T_{\mu\nu} = 0$

A więc z równania Einsteina

$\Box\bar{h_{\mu\nu}}=0$**
gdzie
$\bar{h}=\eta^{\mu\nu}\bar{h_{\mu\nu}}=-h$
oraz $\bar{h^{\mu\nu}}=h^{\mu\nu}+\frac{1}{2}\eta^{\mu\nu}h$

Co mozna zapisać jako:

$\frac{1}{c^2}\frac{\tilde{h_{\mu\nu}}}{\partial{\tilde{t}^2}}=\nabla^2\tilde{h_{\mu\nu}}$

Co odpowiada równaniu fali.

(@TODO skąd tutaj nad h kreska?)

** warunek cechowania Lorentza - oznacza klasę przestrzeni

## Implikacje

Oznacza to że w czasoprzestrzeni istnieją fale poprzeczne, które "ściskają" i "rozluźniają" przestrzeń. Aby takie zaburzenia w czasoprzestrzeni były wykrywalne, muszą być tworzone przez ogromną masę. Najprosztszym źródłem fal są dwa ciała orbitujące wokół siebie.

## Eksperymenty i obserwacje

Ligo ([video a][12]) to eksperyment w USA, składający się z dwóch detectorów grawitacyjnych. Jeden w livingston, louisiana i drugi w Hanford, washington.
Detektory LIGO - Laser Interferometer Gravitational-Wave Observatory. Są to ogrome interferometry. Interferometr pokazuję róznicę w fazie w wiązkach pochodzących z lasera. W przypadku LIGO jest to różnica destrukcyjna - to znaczy jeżeli nie ma zaburzenia w drodze lasera nie obserwujemy. Były dwa detektory bardzo daleko od siebie żeby potwierdzić wyniki niezależnie w tym samym czasie. 
Od 2015r fale wykryto ponad 50 razy.


## Pytania

- co oznaczają indeksy $\mu\nu$?

## Notatki

Fale grawitacyjne zostały pierwotnie przewidziane przez Einstein'a

![Listing publikacji z jakiejś strony wydziałowej](https://home.agh.edu.pl/~kozlow/fizyka/Fale%20grawitacyjne/)

![]()

[30.10.2022]

Zaczynam czytać wykłady  przybycienia https://home.agh.edu.pl/~mariuszp/wfiis_stw/
https://www.youtube.com/watch?v=Hf-BxbtCg_A grwaitacja tensor
https://home.agh.edu.pl/~mariuszp/wfiis_stw/wyklad_stw_8.pdf

- Transformacja Galileusza https://www.youtube.com/watch?v=BLu99pC05ng

[1.11.2022]

Przerobiłem filmiki z [2][2] i dalej z wykładami.

W zasadzie w tej serii filmików https://www.youtube.com/watch?v=cmqASHpWDi8 oraz w wykładzie przybycienia https://home.agh.edu.pl/~mariuszp/wfiis_stw/wyklad_stw_14.pdf jest wszystko co trzeba żeby pokazać że istnieją fale grawitacyjne

http://fma.if.usp.br/~mlima/teaching/PGF5292_2021/Carroll_SG.pdf

[2]:
https://youtu.be/PCujLVSRuMk?t=107

[3]:
https://en.wikipedia.org/wiki/Einstein_field_equations

[4]:
https://en.wikipedia.org/wiki/Metric_tensor_(general_relativity)

[5]:
https://pl.wikipedia.org/wiki/Symbole_Christoffela

[6]:
https://en.wikipedia.org/wiki/Riemann_curvature_tensor

[7]:
https://en.wikipedia.org/wiki/Ricci_curvature

[8]:
https://en.wikipedia.org/wiki/Scalar_curvature

[9]:
https://home.agh.edu.pl/~mariuszp/wfiis_stw/wyklad_stw_14.pdf

[10]:
https://youtu.be/CZoeBmrtJO0?t=27

[11]:
https://www.youtube.com/watch?v=PDY7snRyjBg

[12]:
https://www.youtube.com/watch?v=ofi9VllCOxI

[grawitacja-nobel]:
https://home.agh.edu.pl/~kozlow/fizyka/Fale%20grawitacyjne/Physics%20Nobel%20awarded%20for%20_Nature%202017.pdf


# Rekonstrukcja torów cząstek naładowanych w eksperymentach HEP

## Oddziaływanie cząstki z materiałem
Są trzy efekty które są najbardziej znaczące dla detekcji czastek naładowanych: jonizacja, Rutherford scattering, bremmstrahhlung.

Do detekcji cząstek naładowanych najczesciej wykorzystuje się krzemowe półprzewodniki.
domieszkowanie n półprzewodnika dodaje elektronolubne atomy
domieszkowanie p dodaje atomy nie lubiące elektronów
Półprzewodniki np mają w sobie warstwe zubożoną, na której występuje potencjał elektryczny. Ten potencjał jest powiększany poprzez dodanie bias voltage.

Cząstka naładowaana przechodząca przez półprzewodnik pozostawia za sobą ładunek. Ten ładunek jest zbierany na okładkach i przekazywany dalej jako impuls elektryczny.

Najpopularniejsze są dwa typy ułożenia elmentów zbierających sugnał z detektra: paskowe i pikselowe. 

Paskowe detektory krzemowe najcześciej wykorzystują dwie płaszczyzny ułozone w sposób pozwalający na rozróżnienie koordynatów w przestrzeni 2D zbieranego sygnału przejścia cząstki przez detektor.

Detektory pikselowe same z siebie z definicji zawierają część tej informacji.

Również popularną opcją jest detekcja czastek naładowanych za pomocą gazu. Przykład: ATLAS TRT - drift tubes. Są to podłużne rury z gazem (Xenon 70%, 27% c02, 3% o2). Ładunek zdeponowany w gazie jest zbierane w anodzie wewnątrz rury (sama rura jest katodą).

## Klastrowanie

W celu odtworzenia toru lotu cząstki, przede wszystkim konieczne jest odtworzenie jej miejsca zderzenia z detektorem (hit'u). Zależnie od architektury detektora jest to realizowane na różne sposoby.

W przypadku paskowego VELO była to procedura bliska obliczaniu średniej ważonej z sąsiednich pasków (może się zdarzyć tak że sygnał zostanie zebrany przez więcej niz dwa paski).

## Tracking 

Sama rekonstrukcja toru lotu cząstki (tracking) jest (zależnosci od detektora) skomplikowaną i delikatna procedurą, gdyż w przypadku detektorów kanapkowych wpływa na całościowy proces zbierania danych i identyfikacje cząstk.

Ponieważ rozdzielczość czasowa, oraz rodzaj rejestrowanych zdarzeń i ilości rejestrowanych hitów wpływa na możliwości rekonstrukcyjne w detektorze, możliwe jest wiele różnych podejść do trackingu.

Jedną z częstszych opcji jest rozdzielenie procesu na kilka etapów.

Track finding polega na znajdowaniu tracków-kandydatów. Może przybrać formę. Można wyróznić sposoby lokalne (podążanie za ścieżką hitów od interaction point) - które pod uwagę biorą pojedyncze części hitów, oraz sposoby globalne (Hough transformation) które przetwarzają wszystkie hity na raz i znajdują kandydatów.

Track fitting polega na dopasowaniu pełnej linii toru lotu do zbioru hitów tworzących track kandydujący. Przykładową metodą może być np. filtr kalmana.

### Filtr kalmana

![](https://i.imgur.com/Jof4mkm.png)



https://nbviewer.org/github/rlabbe/Kalman-and-Bayesian-Filters-in-Python/blob/master/table_of_contents.ipynb

## Notatki

https://en.wikipedia.org/wiki/Tracking_(particle_physics)

https://indico.cern.ch/event/847626/contributions/3585799/attachments/1926286/3192537/PascalLecture.pdf slide 15 slide 38 for atlas kalman

https://cds.cern.ch/record/578151/files/cer-002336630.pdf - strona 98 około

# Siecie Bayesowskie

W najprosztszym rozumieniu sieci bayesowskie to modele reprezentowany w formie probabilistycznego grafu (DAG)

![](https://i.imgur.com/ewCtS7e.png)


## twierdzenie bayesa
 
 Twierdzenie (wzór) Bayesa w swej podstawowej formie mówi, że
: $\mathsf P(A\mid B) = \frac{\mathsf P(B \mid A) \, \mathsf P(A)}{\mathsf P(B)}$

gdzie A i B są zdarzeniami oraz $\mathsf P(B) > 0,$ przy czym
* $\mathsf P(A\mid B)$ oznacza prawdopodobieństwo warunkowe, tj. prawdopodobieństwo zajścia zdarzenia A o ile zajdzie zdarzenie B
* $\mathsf P(B\mid A)$ oznacza prawdopodobieństwo zajścia zdarzenia B, o ile zajdzie zdarzenie A


Z definicji prawdopodobieństwa warunkowego

![](https://i.imgur.com/yLOoZWM.png)


$P(A \mid B) = \frac{P(A\cap B)}{\mathsf P(B)}$
W przypadku, gdy $\mathsf P(A) = 0$ twierdzenie zachodzi, ponieważ wtedy $P(A\cap B) = 0.$ Załóżmy zatem, że $\mathsf P(A) > 0.$ Wtedy
$\mathsf P(B \mid A) = \frac{\mathsf P(A\cap B)}{\mathsf P(A)}$

Stąd
$\mathsf P(A \mid B)\cdot \mathsf P(B) = \mathsf P(A\cap B) = \mathsf P(B \mid A) \cdot \mathsf P(A)$

Dzieląc stronami powyższą równość przez $\mathsf P(B)$ otrzymujemy tezę.

## Markov Chain Monte Carlo

Próbkowanie Monte Carlo łańcuchami Markowa (ang. Markov Chain Monte Carlo, MCMC) – klasa algorytmów próbkowania z rozkładu prawdopodobieństwa. Poprzez budowę łańcucha Markowa, który ma rozkład równowagowy taki jak szukana dystrybucja, można wydajnie próbkować złożone rozkłady prawdopodobieństwa. Im większa liczba kroków w takim algorytmie, tym dokładniej rozkład próbki odpowiada pożądanemu rozkładowi.
Łańcuch markowa to proces w którym zdarzenia są od siebie niezależne.
Monte carlo to metoda modelowania matematycznego używająca próbek losowych z rozkładu zgodnego z charakterystyką procesu.

## Metropolis hastings
Skróvony wywód z doktooratu.

Załóżmy f jako rozkład gestości
$f(d_{i}) = \frac{1}{\sigma \sqrt{2\pi} } e^{-\frac{1}{2}\left(\frac{d_{i}-\mu}{\sigma}\right)^2}$

Z bayesa
$P(\theta|D) = \frac{P(D|\theta)P(\theta)}{P(D)}$

przybliżenie
$f(d_{i} | \theta) \approx P(D|\theta)$

Współczynniki kandydata theta
$R = \frac{P(\theta'|D)}{P(\theta|D)}$
Chain rule (część wspólna zdarzeń to iloczyn)
$R = \frac{P(D|\theta')P(\theta')}{P(D|\theta)P(\theta)} =\frac{ \prod_{i}^{n}f(d_{i}|\theta')P(\theta') }{\prod_{i}^{n}f(d_{i}|\theta)P(\theta)}$

Akceptacja:

$A(R)=
\begin{cases}
 R, & \text{if } R < 1 \\ 1,& \text{otherwise}\end{cases}$
 
 
 ![](https://i.imgur.com/NM2Rh9d.png)

metropolis hastings to w zasadzie random walk

## Notatki

https://en.wikipedia.org/wiki/Bayesian_network
http://www.cs.technion.ac.il/~dang/books/Learning%20Bayesian%20Networks(Neapolitan,%20Richard).pdf



# Technologia informatyczna a fizyka
wpływ informatyki na fizykę, proszę omówić temat na wybranych przykładach

Tematy: 

## Sam kod w LHCb

A więc tak, jesli chodzi o wnioski idące z LHCb, to możemy rozróżnić dwi strefy w których informatyka, a raczej programowanie wpływa na fizykę:

- Eksperyment i jego obsługa
- Analiza fizyczna

A więc w poprzediej wersji LHCb, w zadadzie całość obsługi detektora była napisana w C/C++. Kod był odpowiedzialny za przetwarzanie informacji pochodzących z detektora, w tym tracking i identyfikacje cząstek. 
Sam wniosłem wkład w opiekę nad częścia kodu przetwarzającego dane oraz w monitorowanie detektora.




# Wyzwania stojące przed fizykiem eksperymentatorem
, ze szczególnym uwzględnieniem eksperymentów z dużą liczbą naukowców

Fizyka eksperymentalna jest w zasadzie w obecnych czasach niewykonywalna bez udziału w kolaboracji.
O ile pojedyncze analizy fizyczne są możliwe do zrobienia przez pojedynczych naukowców; kolekcjonowanie tych danych a tym bardziej stworzenie aparatury jest praktycznie niemożliwe do wykonania w pojedynkę (o ile mówimy tu o badaniach takich jak fizyka wysokich energii).

Dzięki połączeniu sił przez wiele różnych grup i naukowców możliwe jest wykonywanie badań "cutting edge science" takich jak te wykonywance w CERN'ie.

W rozumieniu wyzwania stojącego przed fizykiem eksperymentatorem to jednym z nich jest własnie współpraca z dużą ilością osób.
Uzyskanie danych do analizy zazwyczaj nie jest proste i wymaga dyskusji i koordynacji z wieloma osobami.

A jeśli chodzi o problemy eksperymentów z dużą liczbą naukowców to myśle że można rozróżnić 3 najważniejsze


- koordynacja grup, rozdział obowiązków i finansowanie
- rozmycie odpowiedzialności
- sytuacja polityczna wpływa na eksperyment

Tutaj bedę się posiłkowała włąsnymi obserwacjami z pracy z LHCb;

Duże kolaboracje naukowe tak na prawdę tworzą dosyć ciekawy schemat zarządzania. Choć rozmiarami i kształtem przypominają duże korporacje, sposób zarządzania jest praktycznie w 100% zgoła inny. 
Tj. w klasycznych korporacjach model zarządzania przypomina piramidę, a kadra menedżerska z rzadka sama wykonuje podstawową pracę.
Również są sztywno określone pozycje i obowiązki.
Natomiast z moich obserwacji wynika że pozorny chaos panujący w zarządzaniu LHCb jest paradoksalnie dość efektywny.
Tak jak dla niewprawionego ucha jazz może brzmieć jak losowa sekwencja dźwięków.
Osoby odpowiedzialne za koordynacje bardzo często pracują bardzo blisko z efektem końcowym swojej pracy.
Brak ściśle określonych pozycji i obowiązków sprawai że o ile jest taka potrzeba osoby mogą zająć się odpowiednimi elementami układanki jeśli istnieje tak potrzeba. 
Natomiast gdy tworza się odpowiedzialne podgrópy krytyczna jest ich synchronizacja, i z powodu rozdzielonej natury pracy, czesto się zdarza że efekt pracy nie jest dobrze dopasowany do wymagań.

Finansowanie może być kłopotliwe, ponieważ jest to schemat mało że uwzględniający finansowanie państwowe to uwzględnia wiele różncych państw.

Rozmycie odpowiedzialności - problem 800 autorów.

Sytuacja polityczna - to co było z rosją.


