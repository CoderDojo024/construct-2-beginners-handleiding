*somige teksten zijn niet vertaald  om zo betere aansluiting te hebben met het programma*

*Let op: gelieve niet om hulp te vragen in de reacties van deze tutorial! In plaats daarvan, ga naar ons [forum](https://www.scirra.com/forum/) om het best mogelijke antwoord op de eventuele vragen te krijgen.*

#Alternatieve tutorials#

Er is een alternatieve gids voor beginners: [How to make a platform game](https://www.scirra.com/tutorials/253/how-to-make-a-platform-game), gericht op het maken van een jump-and-run platformer in plaats van een top-down shooter. Het maakt niet uit met welke tutorial je begint, maar we raden aan om beide tutorials te volgen om een goede idee te hebben hoe je beide typen games kunt maken!

Er is ook [How to make an Asteroids clone in under 100 events](https://www.scirra.com/tutorials/358/asteroid-clone-in-less-than-100-events) door Kyatric. Die is wat geavanceerder, maar ook zeer gedetailleerd.

##Installeren Construct 2##

Als je het nog niet hebt gedaan, download een exemplaar van de nieuwste release van Construct 2 [here](https://www.scirra.com/construct2/releases/new).  De Construct 2 editor is alleen beschikbaar voor Windows, maar de games die je maakt kunnen overal op draaien, zoals Mac, Linux of iPad. Construct 2 kan ook op beperkte gebruikersaccounts worden geïnstalleerd. Het is ook draagbaar, zodat u ook kunt installeren op een USB-stick bijvoorbeeld, zodat je het kunt meenemen! 

##Aan de slag##

Nu je alles hebt ingesteld, start Construct 2 Klik op de *File*-toets, en kies *New*.

![The File menu 'New' button.](https://www.scirra.com/images/articles/filenew.png)

In het *New Project* dialoogvenster, hoef je niets te veranderen. Klik op *Create project*. Construct 2 zal het gehele project voor ons in een enkele *.capx* file bewaren. Je zou nu naar een lege *lay-out* moeten kijken - de lay-out is een ontwerpweergave waarin je objecten kunt maken en plaatsen. Denk aan een lay-out als een level of menuscherm. Met andere software, kan dit ook wel een *room*, *scene* of *frame* worden genoemd.

#Invoegen van objecten#
##Betegelde achtergrond##

Het eerste wat we willen is een herhalende achtergrond tegel. De *Genoemd Background* object kan dit voor ons doen. Allereerst, is hier je achtergrondtextuur - klik erop met de rechtermuisknop en sla het ergens op je computer op ( wel onthouden, je hebt deze straks weer nodig):

![The Tiled Background texture](https://www.scirra.com/images/articles/bg.png)

Nu, **dubbel klik**  in de lay-out om een nieuw object in te voegen. (Later, als het vol is, kunt u ook met de rechtermuisknop openen en kies *Insert new object*.) Zodra de *Insert new object* dialoogvenster verschijnt, ** dubbelklik op de titel Background object** om deze te plaatsen.

[The Insert New Object dialog.][4]

Er verschijnt een vizier voor u om aan te geven waar je het object wilt plaatsen. Klik ergens in de buurt van het midden van de lay-out. De *textuur editor* opent, voor u om de textuur van de tegels in te voeren. Laten we de foto importeren die we eerder hebben opgeslagen. Klik op het map pictogram om een textuur te laden, U kunt het vinden waar u het bestand had neergezet bij het downloaden en selecteer de textuur.

[Load texture from file][5]

Sluit de textuur editor door te klikken op de X in de rechterbovenhoek. Als er om wordt gevraagd, zorg ervoor dat u eerst save`t! Nu moet u uw betegelde achtergrond object zien in de lay-out. Laten we het formaat wijzigen om de gehele lay-out te dekken. Zorg ervoor dat het is geselecteerd, dan is de *Properties Bar* links moeten alle instellingen voor het object zien, waaronder de grootte en positie. Stel de positie in op 0, 0 (linksboven in de lay-out), en de grootte 1280, 1024 (de grootte van de lay-out).

[Tiled Background properties][6]

Een overzicht maken van ons werk. Houd ** controle ** en scroll het ** muiswiel naar beneden ** om uit te zoomen. Of klik * uitzicht - uitzoomt * een paar keer. U kunt ook de middelste muisknop, of space bar ingedrukt houden, om rond te kijken. Netjes, Uw betegelde achtergrond bedekt de gehele lay-out nu:

[The inserted tiled background.][7]

Hit control + 0 of klik * view - zoom tot 100% * om terug te keren naar 1: 1 view.

* (Als je ongeduldig bent zoals ik, op het pictogram kleine 'run' in de titelbalk van het venster -! Een browser  pop-up en zal  lay-out tonen    Woo) *==========
#Een laag toevoegen#

Oké, nu willen we wat meer objecten toevoegen. Echter, gaan we steeds per ongeluk de betegelde achtergrond selecteren, tenzij we achtergrond * op slot * doen, waardoor het niet meer selecteerbaar is. Laten we gebruik maken van de gelaagdheid systeem om dit te doen.

Lay-outs kan bestaan uit meerdere *lagen *, die u kunt gebruiken voor een groep objecten. Stel lagen is zoals glasplaten gestapeld bovenop elkaar met voorwerpen geschilderd op elk glasplaat. Hiermee kunt u eenvoudig regelen welke voorwerpen op anderen lijken, en lagen kunnen worden verborgen, vergrendeld, hebben parallax effecten toegepast, en nog veel meer. Bijvoorbeeld, in dit spel, we willen alles boven de betegelde achtergrond hebben, doordat wij een nieuwe laag bovenop te maken voor onze andere objecten.

Om lagen te beheren, klikt u op het ** tabblad Lagen **, die meestal naast de * Project bar * is:

[Layers bar tab][8]

Je moet zien * Layer 0 * in de lijst (Construct 2 tellen vanaf nul, omdat het beter als dat werkt in de programmering). Klik op het pictogram potlood en ** hernoemen ** naar * Achtergrond *, want het is onze achtergrondlaag. Klik nu op de groene 'toevoegen' icoon om een nieuwe laag toe te voegen voor onze andere objecten. Laten we deze *Main* noemen. Tot slot, als je de sloticon klikt naast * Achtergrond *, wordt het * gesloten *. Dat betekent dat je niet in staat bent om iets te selecteren op die layer. Dat is heel handig voor onze betegelde achtergrond, omdat het gemakkelijk per ongeluk te selecteren is en zal nu niet opnieuw kunnen worden geselecteerd. Echter, als je nodig hebt om wijzigingen aan te brengen, kunt u gewoon op het hangslot te klikken om hem weer te ontgrendelen.

De selectievakjes kunt u ook de lagen in de editor verbergen, maar wij hebben dat niet nodig op dit moment. Uw lagen bar ziet er nu als volgt uit:

[The layers bar, all set up.][9]

Nu, ** zorg ervoor dat de 'Main' laag is geselecteerd in de lagen bar **. Dit is belangrijk - de geselecteerde laag is de actieve laag *. Alle nieuwe ingevoegde objecten worden ingevoegd in de actieve * laag, dus als het niet is geselecteerd, zullen we per ongeluk het invoegen in de verkeerde laag. De actieve laag wordt weergegeven in de statusbalk, en verschijnt ook in een tooltip bij het plaatsen van een nieuw object - het is de moeite waard om dat in de gaten te houden.
# Voeg de input to aan objecten #
** Richt je weer op de lay-out. ** Dubbelklik om een nieuw object in te voegen. Dit keer selecteert u de ** Mouse ** object, aangezien we de muis-ingang nodig hebben.  Doet hetzelfde voor de ** Keyboard ** object.
* Opmerking: * deze objecten hoeven niet te plaatsen in een lay-out. Ze zijn verborgen, en werken automatisch door uw gehele project heen. Nu zijn alle lay-outs in ons project voorzien van muis en toetsenbord acceptatie.
#The game objects#
Het is tijd om ons spel objecten in te voegen! Hier zijn je textures - sla ze allemaal op de harde schijf, zoals eerder.

Player:
[Player texture][10]

Monster:
[Monster texture][11]

Bullet:
[Bullet texture][12]

and Explosion:
[Explosion texture][13]

Voor elk van deze voorwerpen, zullen we met behulp van een * Sprite * object. Het is gewoon een textuur, die je kunt bewegen, draaien en vergroten of verkleinen. Games zijn over het algemeen meestal samengesteld uit sprite objecten. Laten elk van de vier bovengenoemde objecten toe voegen als sprite objecten. Het proces is vergelijkbaar met het plaatsen van de Tegels Achtergrond:

1. ** Dubbelklik ** om een nieuw object in te voegen
2. ** Dubbelklik ** de 'Sprite' object.
3. Wanneer de muis verandert in een crosshair, klikt u ergens in de lay-out. De tooltip moet 'Main' zijn. (Onthouw dat dit de actieve opmaak.)
4 De textuur editor verschijnt. Klik op het pictogram Openen en ** load een van de vier patronen. **)
5. ** Sluiten** de textuur editor, wijzigingen op te slaan. U ziet nu het object in de lay-out!
* Let op: * een andere snelle manier om sprite objecten te voeren is met slepen en neerzetten van het image-bestand van Windows in de lay-out gebied. Construct 2 zal een Sprite met die textuur voor u maken. Zorg er voor dat je een voor een naar de lay-out scherm sleept als je alle vier in een keer slepen, Construct 2 zal een Sprite maken met vier animatie frames.
Beweeg de * kogel * en * explosie * sprites om ergens buiten de rand van de lay-out – we willen ze nog niet zien als het spel begint.
Deze objecten zullen worden opgeroepen * Sprite *, * Sprite2 *, * Sprite3 * en * Sprite4 *. Dat is niet erg handig - dingen zullen snel verwarrend zijn. Hernoemen ze naar * Speler *, * Monster *, * Bullet * en * Explosie * naargelang het geval. U kunt dit doen door het selecteren van het object, dan is het veranderen van de ** naam **  in de eigenschappen bar:

[Renaming an object.][14]
==========
## Het toevoegen van gedrag ##
Gedragingen zijn voorverpakte functionaliteit in Construct 2 Bijvoorbeeld, kunt u een * Platform * gedrag toe voegen aan een object, en de * Solid * gedrag op de grond, en kunt u direct rond te springen als in een platformer. U kunt het zelfde in de gebeurtenissen te doen, maar het duurt langer, En dat is niet echt nodig, het gedrag is al goed genoeg! Dus laten we eens kijken naar welk gedrag we kunnen gebruiken. Oa Construct 2 heeft deze gedragingen;

** 8 Richting beweging **. Hiermee kunt u een object bewegen met het pijltjestoetsen. Het zal goed zijn voor de beweging van de speler.
** Bullet beweging **. Deze eenvoudig beweegt een object vooruit vanuit zijn huidige hoek. Het zal geweldig zijn voor de kogels van de speler. Ondanks de naam, zal het ook mooi werk om de monsters te bewegen - omdat de Objecten verplaatsen naar voren met een bepaald snelheid.
** Scroll naar **. Dit zorgt dat het beeldscherm rond een object beweegt (ook bekend als * scrollen *). Dit zal nuttig zijn voor de speler.
 ** Gebonden aan de lay-out **. Dit zal een object stoppen bij het verlaten van de lay-out gebied. Dit zal ook nuttig zijn op de speler, zodat ze niet kunnen af dwalen buiten het speelveld!
** Destroy buiten layout **. In plaats van het stoppen van een object bij verlaten van de lay-out gebied, wordt het object vernietigd. Het is nuttig voor onze kogels. Zonder dat, zou de kogels steeds op het scherm blijven vliegen, met een beetje geheugen en rekenkracht. In plaats daarvan moeten we de kogels vernietigen zodra ze de lay-out heeft verlaten.
** Fade **. Dit maakt geleidelijk een object fade out, die we zullen gebruiken voor de explosies.
Voeg deze gedragingen toe aan de objecten die ze nodig hebben.
# Hoe pas je een gedrag aan #
We voegen de ** 8 richting beweging ** gedrag aan de speler. Klik op de speler om deze te selecteren. In de eigenschappen bar, let op de * Gedrag * categorie. Klik * Add / Edit * er. Het gedrag dialoogvenster voor de speler zal openen.

[Opening the Behaviors dialog.][16]


Klik op de groene icoon 'toevoegen gedrag' in het dialoogvenster gedrag. Dubbelklik op de ** 8 richting beweging ** dan toevoegen.
[Adding the 8-direction movement.][17]

Gebruik weer hetzelfde en ditmaal voeg het ** Scroll To ** gedrag om het beeldscherm op de speler en ook ** Bound to layout ** gedrag om ze in de layout te houden. Het dialoogvenster gedragingen ziet er nu als volgt uit:

[The Player with all three behaviors added.][20]

Sluit het dialoogvenster gedrag. Hit Run om het spel te proberen! *Save eerst het programma*
[The Run button.][19]

Hopelijk heb je een HTML5 compatibele browser geïnstalleerd. Anders moet u de laatste versie van Firefox of Chrome of Internet Explorer 9 krijgen als je op Vista en hoger. Zodra u het spel loopt, merk je dat je rond kunt bewegen met de pijltjestoetsen, en het scherm volgt de speler! Je kunt ook niet buiten de lay-out ruimte, dankzij de Bound to lay-gedrag. Dit is waar het gedrag goed voor is.Het snel toevoegen van stukjes gedrags functionaliteit. We zullen het evenement systeem binnenkort gebruikt om aangepaste functionaliteit toe te voegen.
# Het toevoegen van de andere gedragingen #
We kunnen het gedrag toe voegen aan de andere objecten op dezelfde manier - te selecteren, klikt * Add / Edit * om het dialoogvenster gedrag te openen, en voeg het gedrag toe. Laten we die andere gedragingen toevoegen:

Voeg de ** Bullet beweging ** en ** Destroy buiten layout ** aan de ** Bullet ** object (geen verrassingen hier)
 Voeg de ** Bullet beweging ** aan de ** Monster ** object (omdat het monster een kant op beweegt net als de bullet)
Voeg de ** Fade ** gedrag aan de ** Explosion ** object (dus het verdwijnt geleidelijk na het verschijnen). Standaard wordt de Fade gedrag vernietigd ook het object na het vervaagd, dat bespaart ons om zorgen te hoeven maken over onzichtbare Explosion voorwerpen waardoor het spel verstopt raakt.
Als je het spel start, kunt u merken het enige wat anders is elke monsters die je kunt zien plotseling vrij snel schieten. Laten we het vertragen naar een rustiger tempo. Selecteer de ** Monster ** object.  Omdat we een gedrag toegevoegd, krijgen we extra eigenschappen die zijn verschenen in de eigenschappen bar:

[Bullet behavior properties][21]

Dit stelt ons in staat om te kijken hoe gedragingen werken. Verander de snelheid van ** 400 ** naar ** 80 ** (dit is in pixels reisde per seconde).
Ook veranderen de ** ** snelheid Bullet object tot 600, en de ** Explosion ** * Fade out tijd Fade gedrag van object * tot ** 0.5 ** (dat is een halve seconde).
# Maak wat meer monsters #
How en controle samen, klik en sleep de ** Monster ** object. U zult merken dat andere monster object bij komen * bijvoorbeeld *. Dit is gewoon een ander object van het Monster * soort object *.
Objecttypen zijn in wezen 'klassen' van objecten. In het geval het event systeem, je vooral bezighouden met objecttypen. Bijvoorbeeld, kunt u een event dat zegt: "Bullet botst met Monster" te maken. Dit betekent eigenlijk "* Elke instantie van de * Bullet * soort object * botst met * een instance van de * Monster * soort object *" - in tegenstelling tot het hebben van een apart event voor elk monster. Met Sprites, alle exemplaren van een objecttype delen ook dezelfde textuur. Dit is geweldig voor de efficiëntie - als spelers je spel online, in plaats van te downloaden 8 monster texturen voor 8 monsters, moeten ze enkel een monster textuur downloaden en Construct 2 herhalingen het 8 keer. We kijken later naar * objecttypen * VS * instances *. Voor nu, een goed voorbeeld om na te denken over is verschillende soorten vijanden zijn verschillende soorten objecten, is de werkelijke vijanden zelf (waarvan er meerdere van kunnen zijn) zijn voorbeelden van deze soorten objecten.
Met behulp van control + slepen, ** creëren 7 of 8 nieuwe monsters **. Plaats geen te dicht bij de speler, of ze kunnen meteen sterven! U kunt uitzoomen met control + muiswiel naar beneden als het helpt, en verdeel ze over de hele lay-out. Je moet eindigen met iets wat een beetje lijkt als dit.
[Several monsters in the layout.][22]

Nu is de tijd om onze aangepaste functionaliteit via visuele manier van programmeren Construct 2 toe te voegen - het * event systeem *.
==========
##Events##
Klik eerst op de * Event sheet 1 * tab aan de bovenkant om over te schakelen naar de * Event sheet editor *. Een overzicht van de gebeurtenissen wordt genoemd een * Event vel *, en je kunt verschillende event voor de verschillende onderdelen van uw spel, of voor de organisatie hebben. Event vellen kunnen ook "onder" andere gebeurtenis vellen vallen, zodat u gebeurtenissen op meerdere niveaus voor bijvoorbeeld hergebruik, maar we zullen dat niet nodig hebben op dit moment.
[The Event Sheet tab.][23]

#Over events#
Als de tekst in het lege blad aangeeft, Construct 2 loopt alles in het event vel eenmaal per tick. De meeste monitors werken hun scherm 60 keer per seconde, zodat Construct 2 zal proberen aan te passen dat voor de meest vloeiende weergave. Dit betekent dat de event vel loopt meestal 60 keer per seconde, telkens gevolgd door opnieuw te tekenen op het scherm. Dat is wat een tick is - een eenheid van "run de event dan tekent op het scherm".
Events loopt van boven naar beneden, zodat gebeurtenissen bovenaan de event pagina eerst worden uitgevoerd.
# Voorwaarden, acties en sub-events #
Gebeurtenissen uit ** voorwaarden **, die test of er wordt voldaan aan bepaalde criteria, bijvoorbeeld "Is spatiebalk naar beneden?". Als aan al deze voorwaarden is voldaan, het evenement ** acties ** gaan allemaal draaien, bijvoorbeeld "Maak een kogel object". Na de acties hebt uitgevoerd, elke ** sub-events ** zijn ook aan het draaien - deze kunnen dan testen meer voorwaarden, dan lopen meer acties, dan is meer sub-events, en ga zo maar door. Met behulp van dit systeem kunnen we de geavanceerde functionaliteit op te bouwen voor onze games en apps. We hebben de sub-events niet nodig in deze tutorial.
Laten we nog een keertje kijken. Kortom, een evenement loopt in principe net als dit:

* Zijn alle voorwaarden voldaan? * 
---> ** Ja **: alle acties van het evenement lopen. 
---> ** Nee **: ga naar de volgende event (met uitzondering van alle sub-events).

Dat is een beetje een oversimplificatie. Construct 2 biedt veel evenement functies om veel verschillende dingen die je zou moeten doen. Maar voor nu, is dit een goede manier om over na te denken.
#Mijn eerste event#
We willen een speler maken die altijd naar de muis kijken. Het ziet er zo uit als we klaar zijn:
[The completed event.][25]

Onthoud een tick draait elke keer wanneer er op het scherm wordt getekend, dus als we de speler gezicht de muis is zullen altijd proberen te kijken richting de muis
Laten we beginnen met het maken van dit evenement. Dubbelklik op een ruimte in het event vel. Dit zal ons gevraagd een ** voorwaarde toe te voegen ** voor de nieuwe event.
[The New Event dialog.][24]

Verschillende objecten hebben verschillende voorwaarden en acties, afhankelijk van wat ze kunnen doen. Er is ook het ** object Systeem **, wat op neerkomt Construct 2 ingebouwde functionaliteit. ** Dubbelklik op ** het object Systeem zoals afgebeeld. Het dialoogvenster zal dan een lijst van alle omstandigheden van het systeem object:
[Choosing 'Every tick'.][26]

** Dubbelklik op ** de * event tick * voorwaarde om deze in te voegen. Het dialoogvenster wordt gesloten en de gebeurtenis wordt gemaakt, zonder acties. Het ziet er nu als volgt uit:
[The empty 'Every tick' event.][27]

Nu willen we een actie toe voegen aan de speler kijkt naar de muis te maken. Klik op de * Actie toevoegen * link aan de rechterkant van het evenement. (Zorg ervoor dat je de Add * actie * koppeling, ** niet ** Add * evenement * koppeling eronder die een heel ander evenement weer zal toevoegen.) Het dialoogvenster Actie toevoegen zal verschijnen:
[The Add Action dialog.][28]

Net als bij het toevoegen van een event, we hebben onze dezelfde lijst van objecten om uit te kiezen, maar dit keer voor het toevoegen van een * actie *. Probeer niet in de war raken tussen het toevoegen van voorwaarden en het toevoegen van acties! Zoals afgebeeld, ** dubbelklikken ** de *-speler * object, want het is de speler die we willen kijken naar de muis. De lijst met acties die beschikbaar zijn in de Player-object verschijnt:

[Player 'Set angle towards position' action.][29]

Merk op hoe 8-richting beweging het gedrag van de speler heeft zijn eigen actie. We hoeven geen zorgen te maken over dat het voor nu.
In plaats van vast te stellen de hoek van de speler in graden, is het handig om de ** Set hoek gebruiken richting van het standpunt ** actie. Deze berekent automatisch de hoek van de speler naar de opgegeven X en Y-coördinaat en stel de hoek van het object in. ** Dubbelklik op ** de * Stel hoek naar positie * actie.
Construct 2 moet nu de X-en Y-coördinaat weten om de speler te wijzen op:
[Set angle towards position parameters.][30]

Dit zijn de zogenaamde de ** parameters**  van de actie.  Voorwaarden kunnen ook parameters hebben, maar * event tick * heeft er geen nodig.
We willen de hoek naar de muis in stellen. De muis object kan hiervan. Voer ** Mouse.X ** voor * X * en ** Mouse.Y ** voor * Y *. Dit zijn de zogenaamde * uitdrukkingen *. Ze zijn als de bedragen die worden berekend. Bijvoorbeeld, kon u ook invoeren * Mouse.X + 100 * of * sin (Mouse.Y) * (hoewel deze specifieke voorbeelden niet erg nuttig zou kunnen zijn!). Op deze manier kunt u alle gegevens gebruiken van een voorwerp, of een berekening, uit te werken parameters in acties en voorwaarden. Het is zeer krachtig, en een soort van verborgen bron van veel van Construct 2's flexibiliteit.
* Hebt u een fout melding  dat zegt  : "mouse is not an object name "  Zorg ervoor dat je de muis object toegevoegd! Ga terug naar pagina 2 en controleren onder " Add the input objects". *
U vraagt zich misschien af hoe je zou herinneren alle mogelijke uitdrukkingen die u zou kunnen gaan gebruiken. Gelukkig is er het "object panel" die je moet zien zweven erboven. Standaard, het is vervaagd, zodat het u niet afleiden.
[The object panel.][31]

Wijs met de muis overheen, of klik op het, en het zal volledig zichtbaar worden. Dit dient als een soort woordenboek van alle uitdrukkingen die u kunt gebruiken, met beschrijvingen, en om u te helpen herinneren. Als u dubbelklikt op een object, zie je al haar uitingen vermeld. Als u dubbelklikt op een uitdrukking, zal het ook automatisch voor u invoert, bespaart u het uittypen van de uitdrukkingen.
Hoe dan ook, klik ** Gereed ** in het dialoogvenster parameters. De actie wordt toegevoegd! Zoals je al eerder zag, zou het er zo uitzien:
[The completed event.][25]

Daar heb je je eerste event! Probeer het spel * wel eerst even saven*, de speler moet nu in staat zijn om te bewegen zoals voorheen, maar nu het gezicht altijd gericht naar de muis. Dit is onze eerste stukje functionaliteit op maat.
==========
##toevoegen game functionaliteit##
Als elke gebeurtenis wordt beschreven in een zo gedetailleerd als voorheen, het gaat om een heel lange tutorial. Laten we de beschrijving een beetje korter voor de volgende gebeurtenissen. Vergeet niet, de stappen om een voorwaarde of actie toe te voegen zijn: y.
1. Double-click to insert a new event, or click an *Add action* link to add an action.
2. Double-click the object the condition/action is in.
3. Double-click the condition/action you want.
4. Enter parameters, if any are needed.

Van nu af aan, zullen gebeurtenissen worden beschreven als het object, gevolgd door de toestand / actie, gevolgd door de parameters. Zo zou de gebeurtenis die we zojuist hebben ingevoerd worden geschreven:
Add condition *System* -> *Every tick*
Add action *Player* -> *Set angle towards position* -> X: *Mouse.X*, Y: *Mouse.Y*

# Krijg de speler om te schieten #
Wanneer de speler klikt, moeten ze een kogel schieten. Dit kan gedaan worden met de * Spawn een object * actie Player, die een nieuwe instantie van een object op dezelfde positie en de hoek creëert. De * Bullet beweging * we eerder toegevoegd dan maakt het vliegen naar voren. Maak het volgende evenement:
Condition: *Mouse* -> *On click* -> Left clicked (the default)
Action: *Player* -> *Spawn another object* -> For *Object*, choose the *Bullet* object.  For *Layer*, put **1** (the "Main" layer is layer 1 - remember Construct 2 counts from zero).  Leave *Image point* as 0.

Uw evenement ziet er nu als volgt uit:

[Ghost shooter event 2.][49]

Als je het spel te draaien, zult u merken de kogels schieten vanuit het midden van de speler, in plaats van het einde van het pistool. Laten we vast dat door het plaatsen van een ** beeldpunt ** aan het eind van het pistool. (Een beeld punt is gewoon een standpunt over een beeld dat je objecten kunt spawnen uit.)
** Klik met de rechtermuisknop ** de speler in het project of object bar en kies Bewerken ** animaties **.
[Editing the player's animations.][50]

De foto-editor voor de speler weer. Klik op de oorsprong en de beeldpunten tool:
[The origin and image points tool.][51]

... en het dialoogvenster beeldpunten opent:

[The image points dialog.][52]

Let op het object oorsprong verschijnt als een rode vlek. Dat is de "hotspot" of "scharnierpunt" van het object. Als u het object te roteren, het draait rond de oorsprong. Wij willen een ander beeld punt toe te voegen aan het pistool te presenteer, dus klik op de groene * toevoegen * knop. Een blauwe punt verschijnt - dat is onze nieuwe beeldpunt. Klik met de linkermuisknop op het einde van het pistool van de speler om het beeld punt daar te plaatsen:

[Placing the image point at the end of the player's gun.][53]

Sluit het beeldbewerkingprogramma. Dubbelklik op het * Spawn een object * actie die we eerder toegevoegd, en verander de * Afbeelding punt * tot ** 1 **. (De oorsprong is altijd het eerste beeldpunt, en onthoud Construct 2 telt van nul.) Het evenement ziet er nu als hieronder - let op het zegt * Afbeelding punt 1 * nu:
[The edited event.][54]

Start het spel. * Eerst even saven* De kogels schieten nu uit het einde van je wapen! De kogels doen nog niets hoewel hopelijk, je zult nu te beginnen te beseffen dat als je eenmaal te pakken met het event-systeem, kunt u zeer snel de functionaliteit elkaar zetten.
Laten we de kogels maken die monsters doden. Voeg de volgende event:

Condition: *Bullet* -> *On collision with another object* -> pick *Monster*.
Action: *Monster* -> *Destroy*
Action: *Bullet* -> *Spawn another object* -> *Explosion*, layer **1**
Action: *Bullet* -> *Destroy*

# The explosion effect #
Start het spel en probeer het opnemen tegen een van het monster. Oeps, de explosie heeft dat grote zwarte rand!
[Explosion with no effect][33]

Je zou kunnen hebben voorspeld dat het zo zou lijken vanaf het begin, en vraagt zich af of ons spel echt zo zou gaan eindigen als dat! Maak je geen zorgen, het zal niet-gebeuren. ** Klik op de Explosie object ** in het object balk in de rechteronderkant, of de Project bar (die met tabbladen met de lagen bar). De eigenschappen worden weergegeven in de eigenschappen balk aan de linkerkant. Aan de onderkant, zet haar ** Blendmode ** onderdeel naar ** Additive **. Nu probeer het spel opnieuw.
[Explosion with additive effect.][34]

Waarom werkt dit? Zonder in te gaan op om de moeren en bouten, zijn gewone beelden * geplakt op de top * van het scherm. Met het additief effect, wordt elke pixel in plaats * toegevoegd * (als in, samengevat) met de achtergrond pixel erachter. Black is een zero pixel waarde, zodat er niets wordt toegevoegd - zie je niet de zwarte achtergrond. Door meer Helderdere kleuren toe te voegen, lijkt het sterker. Het is geweldig voor ontploffingen en lichteffecten.
# Maak de monsters een beetje slimmer #
Nu de monsters dwalen net buiten de lay-out aan de rechterkant. Laten we ze een beetje interessanter maken. Allereerst, laten we beginnen ze op een willekeurige hoek.

Condition: *System* -> *On start of Layout*
Action: *Monster* -> *Set angle* -> random(360)

[Event 4 of the tutorial.][35]

Ze zullen nog steeds afdwalen ze verlaten de lay-out , om nooit meer terug te zien. Laten we ze naar binnen houden. Wat we doen is wijzen ze terug naar de speler als ze de lay-out te verlaten. Dit zorgt voor twee dingen: ze blijven altijd binnen de lay-out, en als de speler stilstaat, monsters komen recht voor hem!

Condition: *Monster* -> *Is outside layout*
Action: *Monster* -> *Set angle toward position* -> For X, **Player.X** - for Y, **Player.Y**.

Start het spel. Als u rond blijft hangen voor een tijdje, zult u merken dat de monsters blijven ook rond de lay-out , en ze gaan in allerlei richtingen. Het is nauwelijks AI, maar dit zal het doen!
Nu, stel dat we vijf keer moeten schieten voor dat het monster sterft, in plaats van onmiddellijke dood als het wordt geraakt. Hoe gaan we dat doen? Als we alleen maar een save "Gezondheid" teller hebben dan wanneer we eenmaal een monster vijf keer hebben geraakt, * alle * monsters zullen dan sterven. In plaats daarvan moeten we * elk * monster moet zijn * eigen * gezondheid onthouden. We kunnen dat doen met ** instantie variabelen **
.==========
##Instance variables##
Instantie variabelen kan elke monster zijn eigen gezondheid waarde op slaan. Een variabele is gewoon een waarde die kan veranderen (of * variëren *), en ze afzonderlijk opgeslagen voor elk exemplaar, vandaar de naam * instantievariabele *.
Laten we een * gezondheid * instantie variabele maken voor onze monster. Klik op het monster in het project of het bar object. U kunt terug naar de lay-out schakelen en selecteer een monster object. Dit zal eigenschappen van het monster in de eigenschappen bar tonen. Klik ** Toevoegen / bewerken ** van ** Bewerken variabelen **.
[Adding a new instance variable.][36]

Het dialoogvenster instance Variabelen verschijnt. Het lijkt op het gedrag dialoogvenster we eerder zagen, maar in plaats daarvan kun je bijvoorbeeld variabelen toe te voegen en te wijzigen voor het object. **Klik op de groene toevoegen knop** om een nieuwe toe te voegen.
[Adding the 'health' instance variable.][37]

In het dialoogvenster dat verschijnt, typt ** gezondheid ** voor de naam, laat * Type * als ** Aantal **, en voor * Initiële waarde * vul ** 5 ** (zoals afgebeeld). Dat begint elke monster op 5 gezondheid. Wanneer ze geraakt worden zullen we 1 aftrekken van de gezondheid, en dan wanneer de gezondheid van nul is zullen we het object vernietigen.
Als je klaar bent klik op OK. Let op de variabele wordt nu weergegeven in het dialoogvenster instantie variabelen en ook in de eigenschappen van het monster ook. (Je kunt snel veranderen beginwaarden in de eigenschappen bar, maar om toe te voegen of te verwijderen van variabelen moet je klikken op * Add / Edit * link.)
[The health instance variable now added to the monster.][38]

#Verander de events#
Ga terug naar het evenement vel. Op dit moment zijn we het vernietigen van monsters, zodra de kogel hen raakt. Laten we dat veranderen van 1 aftrekken van zijn gezondheid.
Vind de gebeurtenis die leest: * Bullet - botsing met Monster *.  We hebben een "te vernietigen monster" actie gemaakt. Laten we dat vervangen met "1 aftrekken van de gezondheid". Klik rechts op het "vernietigen monster" actie en klik ** Vervang **.
[Replacing an action.][39]

Hetzelfde dialoogvenster verschijnt alsof we het invoegen van een nieuwe actie, maar deze keer zal de actie die we geklikt te vervangen. Kies * Monster -> Trek van * (in de * Aanleg variabelen * categorie) * -> * aanleg variabele "gezondheid", en voer ** 1 ** voor * waarde *. Klik ** Gedaan **. De actie moet nu worden weergegeven als volgt:
[Subtracting 1 from monster's health.][40]

Nu we schieten op de monsters verliezen ze 1 gezondheid en de kogel explodeert, maar we hebben geen gebeurtenis gemaakt om monsters te doden als hun gezondheid op nul staat. Voeg een event toe:
Condition: *Monster -> Compare instance variable ->* Health, *Less or equal*, 0
Action: *Monster -> Spawn another object ->* Explosion, layer **1**
Action: *Monster -> Destroy*

[The completed event.][41]

Waarom "minder of gelijk 0" in plaats van "gelijk is aan 0"? Stel dat we een krachtiger wapen dat ** 2 ** afgetrokken van gezondheid. Als je een monster neergeschiet, zou zijn gezondheid gaan ** 5 **, ** 3 **, ** 1 **, ** - 1 **, ** - 3 ** ... mededeling op geen enkel moment was haar gezondheid direct * nul *, dus het zou nooit sterven! Daarom is het een goede gewoonte om te gebruiken "minder of gelijk is" om te testen of de gezondheid op is. 

Start het spel. Je moet nu de monsters vijf keer raken om ze te doden!
## Bijhouden van de uitslag ##
Laten we een score maken, zodat de speler weet hoe goed ze het hebben gedaan. We zullen een andere variabele voor nodig. Je zou kunnen denken "laten ons de uitslag als een van de instantie variabelen van de speler". Dat is geen slechte eerste idee, maar vergeet niet de waarde is opgeslagen "in" het object. Als er geen gevallen zijn er geen variabelen ofwel! Dus als we vernietigen de speler, kunnen we niet meer te vertellen wat hun uitslag was, want het werd vernietigd bij de speler.
In plaats daarvan kunnen we een ** globale variabele gebruiken **. Als een instantie variabele, een globale variabele (of gewoon "global") tekst of opslaan. Elke variabele kan een getal of een enkel stuk tekst opslaan. Globale variabelen zijn ook beschikbaar voor het hele spel in alle layouts - handig als we naar andere niveaus toe voegen.

**Right-click** the space at the bottom of the event sheet, and select *Add global variable*.

[Add a global variable.][42]

Voer ** Score ** zoals de naam. Het andere veld standaardinstellingen zijn OK, het zal beginnend bij 0.
[Adding the Score global.][43]

Nu wordt de globale variabele als regel bij blad. Het is een event vel, maar het is toegankelijk vanaf elk event blad in elke lay-out.
[The Score global variable.][44]

* Opmerking: * er zijn ook * lokaal * variabelen die alleen kan worden geopend door een kleinere "scope" van de gebeurtenissen, maar we hoeven geen zorgen over dat te maken.
Laten we de speler een punt voor het doden van een monster geven. In onze "Monster: gezondheid minder of gelijk 0" event (wanneer een monster sterft), klik ** actie ** toevoegen, en selecteer * Systeem * -> * In * (onder Global en lokale variabelen) -> ** Score **, waarde ** 1 **. Nu zou de event er zo uitzien:
[The event giving the player some score.][45]

Nu heeft de speler een score, die toeneemt met 1 voor elk monster dat ze te doden - maar ze kunnen hun score niet zien! Dat Laten we zien het aan de speler met een tekstobject.
==========
## Het creëren van een heads-up display (HUD)##
Een heads-up display (aka HUD) is de interface die de speler de gezondheid, de score en andere informatie in het spel laat zien. Laten we een heel eenvoudige HUD maken met een tekstobject.
De HUD blijft altijd op dezelfde plaats op het scherm. Als we een aantal interface-objecten, we willen niet dat ze weg schuiven als de speler rond loopt - ze moeten blijven op het scherm. Standaard lagen bladeren. Om ze op het scherm te houden, kunnen we de laag ** Parallax ** instelling gebruiken. Parallax kunnen verschillende lagen om met verschillende snelheden voor een soort van semi-3D-effect te scrollen. Als we de parallax op nul, maar de laag niet helemaal scroll - ideaal voor een HUD.
Ga terug naar de bar lagen we al eerder gebruikt. Voeg een nieuwe laag genaamd * HUD *. Zorg ervoor dat het op de top, en geselecteerd (onthoud dit maakt het de actieve laag). De bar Eigenschappen moet nu tonen van zijn eigenschappen. Stel de ** Parallax ** property aan ** 0, 0 ** (dat is nul op zowel de X-en Y-as).
** Dubbelklik ** een ruimte om een ander object te plaatsen. Deze keer kiest de ** Tekst ** object. Plaats het in de linkerbovenhoek van de layout. Het zal moeilijk te zien zijn als het maar zwart is, dus in de eigenschappen bar, maken het vet, cursief, geel, en kies een iets groter lettertype. Verklein hem breed genoeg om een redelijke hoeveelheid tekst in te past. Het moet er ongeveer zo uitzien:
[The inserted Text object.][46]

Ga terug naar het event vel. Laten we de tekst bijgewerkt met de score van de speler. In de ** Iedere tick ** evenement die wij eerder toegevoegd, voeg de actie * Tekst * -> * Stel tekst *.
Met behulp van de ** & ** operator, kunnen we een aantal converteren naar tekst en met andere tekenreeks. Dus voor de tekst, in te voeren:
**"Score: " & Score**

Het eerste deel (* "Score:" *) betekent dat de tekst zal altijd beginnen met de zin: * Score: *. Het tweede deel (* Score *) is de werkelijke waarde van de Score globale variabele. De ** & ** voegt ze samen in een stuk tekst.
Start het spel, en schiet een aantal monsters. Je score wordt weergegeven, en het blijft op dezelfde plaats op het scherm! T.
## Afwerking ##
We zijn bijna klaar. Laten we nog wat puntjes bijwerken.
Ten eerste, laten we eens wat monsters regelmatig te voorschijn komen, anders als je eenmaal alle monsters dood zijn is er niets meer te doen. We zullen een nieuw monster elke 3 seconden te creëren. Voeg een nieuw evenement:
Condition: *System* -> *Every X seconds* -> **3**
Action: *System* -> *Create object* -> **Monster**, layer **1**, **1400** (for X), **random(1024)** (for Y)

* 1400 * is een X-coördinaat vlak bij de rechterrand van de lay-out, en * random (1024) * is een willekeurige y-coördinaat van de hoogte van de lay-out.
Tot slot, laten we eens spoken maken die de speler kunnen doden.
Condition: *Monster* -> *On collision with another object* -> **Player**
Action: *Player* -> *Destroy*

## Conclusie ##
Gefeliciteerd, je hebt je eerste HTML5 spel gemaakt in Construct 2! Als je een server hebt en je wilt pronken met je werk, klik ** Export** in het menu Bestand. Construct kunnen alle project bestanden naar een map zetten en deze op slaan op uw computer, die u kunt uploaden of te integreren naar een webpagina. Als u niet beschikt over een eigen server, kunt u [share your games on Dropbox][48].

Invoegen van objecten, het gebruik van lagen, gedragingen, events en nog veel meer: je hebt een aantal belangrijke grondbeginselen over Construct2 geleerd. Hopelijk zal dit u motiveren om meer over Construct 2 leren! Probeer het verkennen van de mogelijkheden en zie wat het voor u kunt doen.
# Het afgewerkte ding en#
Probeer het downloaden van het afgewerkte [tutorial project][47].  Ik heb een aantal dingen toegevoegd een aantal extra functies, zoals sommige "Game over" tekst, en monsters die geleidelijk versnellen. Met wat je nu weet, zou het niet moeilijk zijn om erachter te komen hoe het werkt. Er zijn ook tal van reacties te beschrijven hoe het werkt.

Goed gedaan! Als je problemen hebt of u denkt dat een deel van deze tutorial kan worden verbeterd, laat een reactie of stuur ons een bericht op het forum. We zullen zien wat we kunnen doen!
Tenslotte, als je deze tutorial goed vond en je kent iemand die ook graag Construct 2 zou willen, waarom dan geen link van deze tutorial sturen? Het kan toch geen kwaad:)
# Verder lezen #
Wil je muziek en geluidseffecten toe te voegen? Zie [Sounds & Music][57]kijk  in de handleiding voor een snel overzicht.

Je bent misschien geïnteresseerd in leerprogramma onze alternatieve-platformer gebaseerd voor beginners, [How to make a platform game][60].

Indien u meer wilt weten over hoe gebeurtenissen werken in Construct 2 , zie de paragraaf over [How Events Work][55] in de handleiding. Het is sterk aanbevolen, zodat u snel de slag te gaan met uw eigen projecten! Vervolgens voor nog meer informatie, vergeet niet er is [complete documentation in the manual][56]

[1][https://www.scirra.com/construct2/releases/new]
[2][https://www.scirra.com/images/articles/filenew.png]
[3][https://www.scirra.com/images/articles/bg.png]
[4][https://www.scirra.com/images/articles/insertobject.png]
[5][https://www.scirra.com/images/articles/loadtexturefromfile.png]
[6][https://www.scirra.com/images/articles/tiledproperties.png]
[7][https://www.scirra.com/images/articles/tiledui.jpg]
[8][https://www.scirra.com/images/articles/layerstab.png]
[9][https://www.scirra.com/images/articles/layersbar.png]
[10][https://www.scirra.com/images/articles/player.png]
[11][https://www.scirra.com/images/articles/monster.png]
[12][https://www.scirra.com/images/articles/Bullet.png]
[13][https://www.scirra.com/images/articles/explode.png]
[14][https://www.scirra.com/images/articles/objectname.png]
[15][https://www.scirra.com/demos/ghosttutorial/]
[16][https://www.scirra.com/images/articles/openbehaviors.png]
[17][https://www.scirra.com/images/articles/add8dir.png]
[19][https://www.scirra.com/images/articles/runbutton.png]
[20][https://www.scirra.com/images/articles/playerbehaviors_2.png]
[21][https://www.scirra.com/images/articles/bulletproperties.png]
[22][https://www.scirra.com/images/articles/severalghosts.png]
[23][https://www.scirra.com/images/articles/eventsheettab.png]
[24][https://www.scirra.com/images/articles/newevent_2.png]
[25][https://www.scirra.com/images/articles/alwayslookatmouse.png]
[26][https://www.scirra.com/images/articles/everytickcnd.png]
[27][https://www.scirra.com/images/articles/everytickempty.png]
[28][https://www.scirra.com/images/articles/addactiondlg.png]
[29][https://www.scirra.com/images/articles/playersetanglepos.png]
[30][https://www.scirra.com/images/articles/setangleposparams.png]
[31][https://www.scirra.com/images/articles/objectpanel.png]
[32][https://www.scirra.com/images/articles/ghostshooterevent2.png]
[33][https://www.scirra.com/images/articles/explosionnoadditive.png]
[34][https://www.scirra.com/images/articles/explosionadditive.png]
[35][https://www.scirra.com/images/articles/ghostshooterevent4.png]
[36][https://www.scirra.com/images/articles/instvars.png]
[37][https://www.scirra.com/images/articles/healthinstvar.png]
[38][https://www.scirra.com/images/articles/healthadded.png]
[39][https://www.scirra.com/images/articles/replaceaction.png]
[40][https://www.scirra.com/images/articles/sub1fromhealth.png]
[41][https://www.scirra.com/images/articles/monsternohealth.png]
[42][https://www.scirra.com/images/articles/addglobal.png]
[43][https://www.scirra.com/images/articles/addglobalscore.png]
[44][https://www.scirra.com/images/articles/globalscorevar.png]
[45][https://www.scirra.com/images/articles/scoreeevent.png]
[46][https://www.scirra.com/images/articles/textinlayout.png]
[47][https://www.scirra.com/downloads/ghostshooter-tutorial.capx]
[48][https://www.scirra.com/tutorials/42/upload-your-game-to-dropbox]
[49][https://www.scirra.com/images/articles/spawnbullet1.png]
[50][https://www.scirra.com/images/articles/editanimations.png]
[51][https://www.scirra.com/images/articles/imagepointstool.png]
[52][https://www.scirra.com/images/articles/imagepointsdlg.png]
[53][https://www.scirra.com/images/articles/placingimagepoint.png]
[54][https://www.scirra.com/images/articles/spawnbullet2.png]
[55][https://www.scirra.com/manual/75/how-events-work]
[56][https://www.scirra.com/manual/1/construct-2]
[57][https://www.scirra.com/manual/84/sounds-music]
[58][https://www.scirra.com/forum/]
[59][https://www.scirra.com/forum/]
[60][https://www.scirra.com/tutorials/253/how-to-make-a-platform-game]
[61][https://www.scirra.com/tutorials/358/asteroid-clone-in-less-than-100-events]
