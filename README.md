WIA1002-DataStructure

# Pokémon -

# Kanto Adventure

```
Image 1 - ArtworkoftheKantoRegion
```
## Introduction

WelcometotheworldofPokémon,whereyouwillembarkonanepicjourney
through the Kanto region, capturing, training, and battling Pokémon to
become theultimate PokémonTrainer.If youwereacoolchildgrowingup,
you were definitely a Pokémon fan, from collecting cards, playing the
Nintendogamesandobsessingovertheanimeadaptation.

Inthis game, you willnavigate through various cities,each with its unique
Pokémonencountersandchallenges.AsaTrainer,yourjourneywillbefilled
withbattles againstGymLeaders,trainingyourPokémonandexploringthe


WIA1002-DataStructure

vastKantoregion.Yourprogress,includingyourPokémonteam,badges,and
location,willbesaved, allowingyou tocontinueyouradventurefromwhere
youleftoff.

## ProblemStatement

Theobjectiveof thisprojectisto developatext-basedPokémongamethat
captures the essence of the beloved Pokémon franchise, focusingon the
Kanto region. The game will be designed to run in a Text-based User
Interface(TUI)butifyouarewilling,youcan improveitanduseaGraphical
UserInterface(GUI),utilizingJavaastheprogramminglanguage.Theproject
aims to leverage your probleming solving skills while helping you develop
yourconceptsofDataStructures(DS)andbasicgamelogic.

Thegamewillfeatureavarietyofelements,includingnavigatingthroughthe
Kantoregion,capturingandtrainingPokémon,battlingagainstGymLeaders,
and exploring the game's mechanicssuch as levelingup,savingprogress,
and managing the player's team. The gamewill alsoincorporate dynamic
weather systems, challenging wild Pokémonencounters, and a system for
playerstoevolvetheirPokémon.

## MainFeatures(13Marks)

### 1. Path of Champions - RegionExplorer( 1. 5 mark)

TheKantoMapis theheartofyourjourney.Eachcity ispartofthejourney
and giving the player the ability to move around and do different stuff in
different citiesis crucial.Thejourneystartsintheplayer’shometowncalled
“Pallet Town”. Each city [except Pallet town and Lavender Town] has its
uniqueGymandGymleaders[moreinformation].EachCitywillalsohaveits
own unique set of wild Pokémon the player can fight to train their own
Pokémon, you can select each set as you like, but stick to the Pokémon
found in the Kanto region. Try to keep the level of wild Pokémonslightly
belowbutclosetotheGymTrainer’sPokémontoensuretheplayercantrain
properlyforeachregion.


WIA1002-DataStructure

**ImplementationTips:**
Eachcitycanbeanode,andthepathscanbeedges.Ignorethebluedotson
themapforthesakeofsimplicity.

```
Image 2 - MapofKantofromPokémonFireRed
```
Youcanusetheimageprovidedtoimplementyourmapandunderstandhow
eachcityconnects.

SampleOutput:

```
+----------------------------------------------------------------------+
You are currently in Viridian city:
+----------------------------------------------------------------------+
[1] Move to:
a. Pallet Town b. Pewter city
[2] Challenge Gym leader [Giovanni - Ground type]
[3] Fight Wild Pokemon [Pidgey, Ratata, Spearow are common]
```

WIA1002-DataStructure

```
[4] Player Options
a.Show map b.Show My Pokemon c.Show My badges d.Save and Exit
+----------------------------------------------------------------------+
Your choice: 1b
+----------------------------------------------------------------------+
Moving to Pewter City...
```
```
+----------------------------------------------------------------------+
You are currently in Pewter City:
+----------------------------------------------------------------------+
[1] Move to:
a. Cerulean City b. Viridian City
[2] Challenge Gym leader [Brock - Rock type]
[3] Fight Wild Pokemon [Pidgey, Meowth, Sycther are common]
[4] Player Options
a.Show map b.Show My Pokemon c.Show My badges d.Save and Exit
+----------------------------------------------------------------------+
Your choice: 4a
+----------------------------------------------------------------------+
Map of Kanto
```
```
[**Pewter City**]-------------------[CeruleanCity]-----------------|
| | |
| | |
| | |
| | |
| [Celadon City]----[SaffronCity]-----[Lavender Town]
| | | |
[Viridian City] | | |
| | | |
| | | |
| | [Vermillion City]---------------|
| | |
[Pallet Town] | |
| | |
| [Fuchsia City]---------------------------------|
| |
| |
[Cinnabar Island]-----------|
```
```
+----------------------------------------------------------------------+
```

WIA1002-DataStructure

This output showsthe user's current location in Viridian Cityandpresents
options for movement, challenging aGym Leader, catchingwild Pokémon,
and accessing player options. The user's choiceto movetoPewter Cityis
thenexecuted,showcasingthedynamicandinteractivenatureofthegame.

AmongthePlayerOptionstheusercanviewthemapasshownintheoutput,
themapalsohighlightstheuser'scurrentlocationusingtheasterisksymbols
around that city. The other options include viewing the player’s pokemon
informationandshowingthenumberofbadgesearned.

### 2. Memory Cartridge - SavingProgress( 1 marks)

```
Image 3 - AnoldNintendoPokémoncartridge
```
Thecoreobjective ofthe SaveGamefeatureis toenableplayerstopersist
theirprogress acrossgame sessions. Thisfeatureis crucialformaintaining
continuityinthegameplayexperience,allowingplayerstosavetheircurrent
state, including the trainer's name, location within the Kanto Map, the
Pokémon teamthey have collected, and anyGym Leaders defeated along
withthebadgestheyhaveearned.Uponloadingthegame,playersshouldbe


WIA1002-DataStructure

abletoresumefromtheirlastsavedstate,ensuringthattheirprogressisnot
lostandthattheycancontinuetheiradventurefromwheretheyleftoff.They
mayalsostartanewgame.
The progress can easily be saved and loaded by using File I/O and
convenientfiletypes(maybeJSONorxml?).

SampleOutput:

```
,'\
_.----. ____ ,' _\ ___ ___ ____
_,-' `. | | /`. \,-' | \ / | | \ |`.
\ __ \ '-. | / `. ___ | \/ | '-. \ | |
\. \ \ | __ | |/ ,','_ `. | | __ | \| |
\ \/ /,' _`.| ,' / / / / | ,' _`.| | |
\ ,-'/ / \ ,' | \/ / ,`.| / / \ | |
\ \ | \_/ | `-. \ `' /| | || \_/ | |\ |
\ \ \ / `-.`.___,-' | |\ /| \ / | | |
\ \ `.__,'| |`-._ `| |__| \/ | `.__,'| | | |
\_.-' |__| `-._ | '-.| '-.| | |
```
```
+----------------------------------------------------------------------+
Welcome to Pokemon - Kanto Adventures
+----------------------------------------------------------------------+
[1] Load Game:
a. Save 1 - Amaan b. Save 2 - empty c. Save 3 - empty
[2] Start a new Adventure:
a. Save 1 - Override b. Save 2 - new c. Save 3 - new
[3] Exit
+----------------------------------------------------------------------+
Your choice: 2b
+----------------------------------------------------------------------+
OAK: Hello there! Welcome to the world of Pokémon! My name is Oak!
People call me the Pokémon Prof! This world is inhabited by creatures
called Pokémon! For some people, Pokémon are pets. Others use them for
fights. Myself... I study Pokémon as a profession.
```
```
OAK: First, what is your name?
+----------------------------------------------------------------------+
Enter your name: Amaan
+----------------------------------------------------------------------+
OAK: Right! So your name is Amaan! Welcome to the world of Pokemon.
It's time to choose your starting pokemon.
+----------------------------------------------------------------------+
[1] Bulbasaur [Grass - Level 5]
[2] Squirtle [Water - Level 5]
```

WIA1002-DataStructure

```
[3] Charmander [Fire - Level 5]
+----------------------------------------------------------------------+
Your choice: 1
+----------------------------------------------------------------------+
OAK: You chose Bulbasaur, an amazing choice. Best of luck!
+----------------------------------------------------------------------+
You are currently in Pallet Town:
+----------------------------------------------------------------------+
[1] Move to:
a. Viridian City b. Cinnabar Island
[2] Talk to Mom [Your hometown has no Gym]
[3] Fight Wild Pokemon [Pidgey, Meowth, Sycther are common]
[4] Player Options
a.Show map b.Show My Pokemon c.Show My badges d.Save and Exit
+----------------------------------------------------------------------+
Your choice: 2
+----------------------------------------------------------------------+
MOM: "Oh, Amaan! You're leaving on your adventure with Pokémon? How
exciting! I know you've always dreamed of this day. Remember, the bond
you share with your Pokémon is the most important thing. Take care of
them, and they'll take care of you. Don't worry about me; I'll be just
fine here. I can't wait to hear all about your adventures and the new
friends you're going to make. Remember, no matter how far you go, I'm
always here for you. Be brave, be kind, and everything will turn out
just fine. I'm so proud of you already! Now, go on, your adventure
awaits! Oh, and don’t forget to change your underwear every day! Safe
travels, my dear!"
+----------------------------------------------------------------------+
```
Yes, that is actual dialoguefrom the game. Youcan search through other
original dialogue on the internet and maybe cycle some of the things the
momsayshere.

Try to keep the starting Pokémon close to the original (don’t start with
Moltres,ZapdosandArticunolol).


WIA1002-DataStructure

### 3. Pokémon Journeyer - Trainer/Player( 1. 5 mark)

```
Image 4 - AshKetchumandPikachufromtheAnimeseries
```
The Trainer class in your Pokémon game is a pivotal component that
encapsulatestheplayer'sdataandfunctionalities.Itisdesignedtorepresent
theplayer'scharacter,includingtheirname,currentlocation,Pokémonteam,
badges,andprogress.

```
+----------------------------------------------------------------------+
You are currently in Pallet Town:
+----------------------------------------------------------------------+
[1] Move to:
a. Viridian City b. Cinnabar Island
[2] Talk to Mom
[3] Fight Wild Pokemon [Pidgey, Meowth, Sycther are common]
[4] Player Options
a.Show map b.Show My Pokemon c.Show My badges d.Save and Exit
+----------------------------------------------------------------------+
Your choice: 4c
+----------------------------------------------------------------------+
Your Badges:
```
- None
+----------------------------------------------------------------------+


WIA1002-DataStructure

Asyoucansee,sincetheplayerjuststartedthegame.Theyhavenobadges.

```
+----------------------------------------------------------------------+
You are currently in Pallet Town:
+----------------------------------------------------------------------+
[1] Move to:
a. Viridian City b. Cinnabar Island
[2] Talk to Mom [Your hometown has no Gym]
[3] Fight Wild Pokemon [Pidgey, Meowth, Sycther are common]
[4] Player Options
a.Show map b.Show My Pokemon c.Show My badges d.Save and Exit
+----------------------------------------------------------------------+
Your choice: 4b
+----------------------------------------------------------------------+
Your Pokémon:
```
- Bulbasaur - Level: 6
+----------------------------------------------------------------------+

Thetraditionalpathofdifficultyforgymsis:
● PewterCityGym
● CeruleanGym
● VermilionGym
● CeladonGym
● FuchsiaCityGym
● SaffronCityGym
● CinnabarIslandGym
● ViridianCityGym

You need to vary the level of the Leaders’ Pokémon and the area wild
Pokémonaccordingtothe ordergiven above.Aftertheplayerhascollected
all 8 badges,congratulatethemandplaycredits.


WIA1002-DataStructure

### 4. Elemental Creatures - ThePokémon

### ( 1. 5 marks)

```
Image 5 - AshKetchumwithhisKantoPokémon
```
The coreof the Pokémon gamerevolvesaroundthePokémonthemselves,
each with unique attributes and capabilities. The goal is to design and
implement a Pokemon class in Java that encapsulates the essential
characteristics and behaviors of a Pokémon, allowing playersto train,and
battlewiththem.

**Requirements:**

- **Pokémon Attributes:** Each Pokémon must have the following
    attributes:
       - **Name:** ListofPokémoninKanto-Noneedtoincludeall.
       - **Type:** Fire/Grass/Wateretc.
       - **Level:** DeterminestheattackpowerandHPofthePokémon.
       - **Moves:** Each Pokemon has 2 Fixedmoves,useamaptomap
          eachmovetoitsdamage.
       **- Strengthand Weakness:** EachPokemonisweakagainstsome
          typesandstrongagainstothertypes,theyreceivea20%attack
          bonusforbeingstrongand20%reductionforbeingweak.


WIA1002-DataStructure

```
+----------------------------------------------------------------------+
You are currently in Pewter City:
+----------------------------------------------------------------------+
[1] Move to:
a. Cerulean City b. Viridian City
[2] Challenge Gym leader [Brock - Rock type]
[3] Fight Wild Pokemon [Pidgey, Meowth, Sycther are common]
[4] Player Options
a.Show map b.Show My Pokemon c.Show My badges d.Save and Exit
+----------------------------------------------------------------------+
Your choice: 4b
+----------------------------------------------------------------------+
Your Pokémon:
Bulbasaur - Level: 5
Type: Grass/Poison
HP: 18
XP: 35/
Moves:
```
- Vine Whip [30 damage]
- Tackle [20 damage]
Strong Against:
- Water
- Ground
- Rock
Weak Against:
- Fire
- Flying
- Psychic


WIA1002-DataStructure

### 5. Pokémon Battle - FightingotherPokémon

### ( 1. 5 Marks)

```
Image 6 - TwoPokémontrainersbattlingitout
```
Theprimaryobjectiveof thisfeatureistoimplementacomprehensivebattle
system within the Pokémon game. This system will facilitate encounters
betweentheplayer andgymleadersorwildPokémon,allowingfordynamic
and strategic battles. The battle system will be designed to simulate the
turn-based combat mechanics found in the Pokémon series, where each
Pokémon can attackand defend ina sequencedeterminedbytheirspeed
stat.

```
+----------------------------------------------------------------------+
You are currently in Pewter City:
+----------------------------------------------------------------------+
[1] Move to:
a. Cerulean City b. Viridian City
[2] Challenge Gym leader [Brock - Rock type]
[3] Fight Wild Pokemon [Pidgey, Meowth, Sycther are common]
[4] Player Options
a.Show map b.Show My Pokemon c.Show My badges d.Save and Exit
+----------------------------------------------------------------------+
Your choice: 2
+----------------------------------------------------------------------+
You are about to challenge Gym Leader Brock!
Prepare yourself for an intense battle!
Your Pokémon:
```

WIA1002-DataStructure

```
Bulbasaur - Level: 5
+----------------------------------------------------------------------+
Battle Start: Trainer Amaan vs. Gym Leader Brock!
Brock sends out Geodude [Level 8]!
```
```
Bulbasaur is sent out! Its grass type is strong against the opponent’s
geodude.
```
```
Round 1:
Bulbasaur's Moves:
```
1. Tackle
2. Vine Whip

```
Which move will Bulbasaur use?
Your choice: 2
+----------------------------------------------------------------------+
Bulbasaur used Vine Whip!
It's super effective!
Geodude's HP drops significantly. [Geodude HP: 20/60]
```
```
Geodude uses Tackle!
Bulbasaur takes some damage. [Bulbasaur HP: 35/45]
```
```
Round 2:
Bulbasaur's Moves:
```
1. Tackle
2. Vine Whip

```
Which move will Bulbasaur use?
Your choice: 1
+----------------------------------------------------------------------+
Bulbasaur uses Tackle!
Geodude's HP drops slightly. [Geodude HP: 10/60]
```
```
Geodude uses Rock Throw!
Bulbasaur takes some damage. [Bulbasaur HP: 25/45]
```
```
Round 3:
Bulbasaur's Moves:
```
1. Tackle
2. Vine Whip

```
Which move will Bulbasaur use?
Your choice: 2
+----------------------------------------------------------------------+
Bulbasaur uses Vine Whip!
```

WIA1002-DataStructure

```
It's super effective!
Geodude faints!
```
```
Bulbasaur gained 40xp.
Bulbasaur [XP: 70/100]
```
```
Brock sent out Onix. You have to defeat all his Pokemon.
+----------------------------------------------------------------------+
```
### 6. Pokémon Mastery - Levelingup( 1 mark)

```
Image 7 - APokémonlevelingup
```
What is the point of playing the gameif you can level up and makeyour
Pokémonstronger?ThefeatureofPokémonlevelingupbasedonexperience
points (XP) and reaching certain XP thresholds is a critical aspect of
gameplay that significantly impacts the progression and development of
Pokémonwithinthegame.Thisfeatureisdesignedtosimulatethereal-world
mechanics of Pokémon games,where Pokémon gainXP from battles and


WIA1002-DataStructure

encounters,andleveluptoincreasetheirstats,learnnewmoves,andevolve
intomorepowerfulforms.
Levels1-10take100xpeach.
Levels10-30take200xpeach.
And30+take300xpeach.
Everytime the pokemondefeats another pokemon, its xp increases by the
(5*levelofopponent)pokemon.

WhenthethresholdoftheXPisreachedthepokemon’slevelincreases.

```
Bulbasaur uses Tackle!
It's super effective!
Ratata faints!
```
```
Bulbasaur gained 40xp.
Bulbasaur [XP: 100/100]
```
```
Bulbasaur leveled up.
Bulbasaur[Level 4 --> Level 5]
```
EverytimeaPokémonlevelsup,itsdamageforallmovesincreasesby2.Soif
Bulbasaur'sTackledid 30 damage,nowitdoes32.

### 7. PokéMaze - Figureyourwayout( 1. 5 marks)

```
Image 8 - InsidethePokémontower
```
YouweretravelingthroughtheghostinhabitingtowncalledLavenderTown,
whenyou decidedtoenterthehauntedPokémontowerandgotstuck.Now
youhavetofigureyourwayoutwhileavoidingGhastlieswhoarehuntingyou.


WIA1002-DataStructure

Requirements:
● Theprogramshoulddisplaytheinitialmaze withthestartingpoint'S'
marked.
● Theprogramshouldprompttheusertoinputdirections(up,down,left,
right)tonavigatethroughthemaze.
● The program should validate the user's input and only accept valid
directions.
● The program should update the position of the player in the maze
accordingtotheuser'sinput.
● The program should usea stack data structureto keep track of the
pathtakenbytheplayer.
● IftheplayertouchestheGhastlytheygetcaught.
● Theprogramshouldcontinuepromptingtheuserfordirectionsuntilthe
playerreachestheendpoint'E'.
● Upon reaching the end point 'E', the program should display a
congratulatorymessage.

Sampleoutputs:
[Note:Lavendertownhasnogym]

```
+----------------------------------------------------------------------+
You are currently in Lavender Town:
+----------------------------------------------------------------------+
[1] Move to:
a.Cerulean City b.Saffron City c.VermillionCity d.Fuchsia city
[2] Fight Wild Pokemon
[3] Player Options
a.Show map b.Show My Pokemon c.Show My badges d.Save and Exit
[4] PokeMaze
+----------------------------------------------------------------------+
Your choice: 5
+----------------------------------------------------------------------+
Welcome to the PokeMaze Challenge!
Find your way through the maze using stacks.
Legend: # - Wall,. - Path, S - Start, E - End, G - Ghastly
# # # # # # # # # # # # # # # # #
# S.... #......... #
# # # # #. #. # # # # # # #. #
#... #. #. #..... #. #
# # #. #. # # # G #. #. # # #
```

WIA1002-DataStructure

```
#... #... #... #... #
# # # # # G #. #. #. # # #. #
#......... #..... #
# # # # # # # # # # # # # # # E #
Enter direction (up, down, left, right): right
# # # # # # # # # # # # # # # # #
# S Y... #......... #
# # # # #. #. # # # # # # #. #
#... #. #. #..... #. #
# # #. #. # # # G #. #. # # #
#... #... #... #... #
# # # # # G #. #. #. # # #. #
#......... #..... #
# # # # # # # # # # # # # # # E #
```
```
# # # # # # # # # # # # # # # # #
# S... Y #......... #
# # # # #. #. # # # # # # #. #
#... #. #. #..... #. #
# # #. #. # # # G #. #. # # #
#... #... #... #... #
# # # # # G #. #. #. # # #. #
#......... #..... #
# # # # # # # # # # # # # # # E #
Enter direction (up, down, left, right): right
Invalid move. Try again.
```
```
# # # # # # # # # # # # # # # # #
# S.... #......... #
# # # # #. #. # # # # # # #. #
#... #. #. #..... #. #
# # #. #. # # # G #. #. # # #
#... #... #... #... #
# # # # # Y #. #. #. # # #. #
#......... #..... #
# # # # # # # # # # # # # # # E #
Oh no! You encountered a Ghastly and got caught.
Game Over.
```
```
Enter direction (up, down, left, right): down
# # # # # # # # # # # # # # # # #
# S.... #......... #
# # # # #. #. # # # # # # #. #
```

WIA1002-DataStructure

```
#... #. #. #..... #. #
# # #. #. # # # G #. #. # # #
#... #... #... #... #
# # # # # G #. #. #. # # #. #
#......... #..... #
# # # # # # # # # # # # # # # Y #
Congratulations! You've reached the end of the maze.
```
### 8. Rival’s Race - Beatyourrival( 2 marks)

```
Image 9 - Gary(Left)andAshKetchum(Right)
```
IntheheartofSaffronCity,anepicrivalryunfoldsasGary,yourlifelongrival,
challengesyoutoarace.Thestakesarehigh,andvictoryiswithinreach,but
toemergetriumphant,youmustnavigatethroughtheintricatestreetsand
pathwaysofthecitytoreachthedestinationthatGaryhaschosen.Yourtask


WIA1002-DataStructure

istouncovertheshortestpathtothecitythatGaryselects,outsmartinghim
andsecuringyourplaceastheultimatePokemontrainer.

**Requirements:**
● TheprogramshouldrandomlyselectadestinationforGarytoraceto.
ThisdestinationshouldnotbedirectlyadjacenttoSaffronCity.
● Utilizeanefficientpathfindingalgorithmtodeterminetheshortestpath
fromSaffronCitytotherandomlychosendestination.Thisalgorithm
shouldcalculatetheoptimalroute,consideringthelayoutofthemap
andanyobstaclesintheway.
● OutputShorterPath:DisplaytheshorterpathfromSaffronCitytothe
selecteddestination,providingcleardirectionsorcoordinatesforeach
stepalongtheway.

```
Image 10 - MapofKantowithinter-citydistances
```
Sampleoutput:

```
+----------------------------------------------------------------------+
You are currently in Saffron City:
+----------------------------------------------------------------------+
[1] Move to:
a.Cerulean City b.Lavender Town c.VermillionCity d.Celadon City
```

WIA1002-DataStructure

```
[2] Challenge Gym leader [Sabrina - Psychic type]
[3] Fight Wild Pokemon
[4] Player Options
a.Show map b.Show My Pokemon c.Show My badges d.Save and Exit
[5] Rival’s Race
+----------------------------------------------------------------------+
Your choice: 5
+----------------------------------------------------------------------+
```
```
The battle has begun! Your rival Gary has challenged you to a race to
Cinnabar Island.
```
```
Shortest Path:
Saffron City -> Vermillion City -> Fuchsia City -> Cinnabar Island
```
```
Goodluck on your race!
+----------------------------------------------------------------------+
```
### 9. Safari Zone - QueueingupthePokémon( 1. 5 mark)

```
Image 10 - PokémonGOSafariZone
```
Welcome to the Safari zone, where chaos reigns and organizationis key!
LininguptoentertheSafariZoneareahordeofpokemon,buttheyneedto
enterinaparticularordertoavoidchaos.Youdecidetohelpoutandarrange


WIA1002-DataStructure

the Pokémon; but it's notas simpleasarrangingthem alphabeticallyorby
type.EachPokemonhasits ownpreferencesandquirksthatmustbetaken
intoaccount.

Yourtask isto arrangeagroupofrandomlyselectedPokemoninaspecific
orderwhileadheringtotheiruniqueconditionsandpreferences.Whichare:
● **Bulbasaur** refusestobeplacednexttoCharmander,hisfireburnstoo
hot.
● **Pikachu** demands to be placed at the center of the arrangement
because,well,it'sPikachu!
● **Snorlax** insistsonbeingpositionedatthe endofthelineuptoensure
maximumrelaxation.
● **Jigglypuff** prefers to be surrounded by other "cute" Pokémon for
moralepurposes.[ShefindsPikachucute]
● **Eevee** insistsonbeingpositionedeitheratthebeginningofthelineup
toshowcaseitsadaptability.
● **Machop** demands to be placednextto theheaviestPokemonin the
lineuptoshowoffitsstrength.[It'sprobablysnorlax]

**Requirements:**
● LettheusersenterthePokémoninorder.
● MakealistofthePokémonandsortit.
● Displayeachstepofthesorting.
● Displaythesortedlist.

SampleOutput:

```
+----------------------------------------------------------------------+
You are currently in Fuchsia City:
+----------------------------------------------------------------------+
[1] Move to:
a.Cinnabar Island b.Lavender Town c.Vermillion City d.Celadon City
[2] Challenge Gym leader [Koga - Poison type]
[3] Fight Wild Pokemon
[4] Player Options
a.Show map b.Show My Pokemon c.Show My badges d.Save and Exit
[5] Safari Zone
+----------------------------------------------------------------------+
```

WIA1002-DataStructure

```
Your choice: 5
+----------------------------------------------------------------------+
Welcome to the Safari Zone! Today's challenge: Sort the Pokémon!
+----------------------------------------------------------------------+
Enter the Pokémon in your party (separated by a comma): Pikachu,
Bulbasaur, Charmander, Snorlax, Jigglypuff, Eevee, Machop
```
```
You entered: Pikachu, Bulbasaur, Charmander, Snorlax, Jigglypuff, Eevee,
Machop
```
```
Sorting your Pokémon according to their unique preferences...
```
```
Step 1: Eevee insists on being positioned either at the beginning of the
lineup to showcase its adaptability.
Sorted List: Eevee, Pikachu, Bulbasaur, Charmander, Snorlax, Jigglypuff,
Machop
```
```
Step 2: Pikachu demands to be placed at the center of the arrangement.
Partial Sort: Eevee, Bulbasaur, Jigglypuff, Pikachu, Charmander,
Snorlax, Machop
```
```
Step 3: Snorlax insists on being positioned at the end of the lineup to
ensure maximum relaxation.
Partial Sort: Eevee, Bulbasaur, Jigglypuff, Pikachu, Charmander, Machop,
Snorlax
```
```
Step 4: Jigglypuff prefers to be surrounded by other "cute" Pokémon for
morale purposes.
Partial Sort: Eevee, Bulbasaur, Jigglypuff, Pikachu, Charmander, Machop,
Snorlax
```
```
Step 5: Bulbasaur refuses to be placed next to Charmander.
Partial Sort: Eevee, Bulbasaur, Jigglypuff, Pikachu, Machop, Charmander,
Snorlax
```
```
Step 6: Machop demands to be placed next to the heaviest Pokemon in the
lineup to show off its strength.
Final Sorted List: Eevee, Bulbasaur, Jigglypuff, Pikachu, Charmander,
Machop, Snorlax
```
```
+----------------------------------------------------------------------+
Your Pokémon are now sorted! Enjoy your adventure in the Safari Zone!
+----------------------------------------------------------------------+
```

WIA1002-DataStructure

## ExtraFeatures(2Marks)

### 1. Graphical User Interface

```
Image 11 - AGameBoyAdvance(GBA)Pokémongame
```
TheGraphicalUser Interface(GUI) featureenhancesthe gamingexperience
by providing a visually appealing interface for players to interact with.
Throughintuitivemenus,buttons,andgraphicalrepresentations,playerscan
seamlesslynavigatethroughtheKantoregion,engageinbattles,andaccess
various game features. The GUI adds a layer of immersion, bringing the
Pokémon world to life with vibrant visuals and animations, making the
gameplayexperiencemoreengagingandenjoyable.


WIA1002-DataStructure

### 2. Pokémon Evolution and Items

```
Image 12 - PokémonevolutioninPokémonFireRed
```
Pokémonevolutionisonethemostimportantaspectsoftheoriginalgames,
although it is a bit complex. Some Pokémon just evolve after reaching a
certainlevel,butsomehavemorecomplexsystemslikeweatherconditions,
itemsheld,etc.Ifyouarewilling,youcanimplementthosefeatures.
Alongwiththatyoucanalsoimplementstatusailmentsandhealingitemslike
Poisoned, Paralyze,etc. counteredwith Antidotes, Paralyze Heals, Potions,
etc.

### 3. Account Creation

Ensuring the ability to save game progress is paramount in any gaming
experience. Moreover, incorporating the functionality for multiple users to
engage with the game through individual accounts presents a significant
enhancement.Thisfeatureenablesplayerstocreateandaccesstheirunique
accounts,facilitatingpersonalizedgameplayexperiences.Eachusercanlog
in totheirrespectiveaccountandseamlesslycontinuetheiradventurefrom
the exact point where they last left off. By implementing user account
management,thegamenotonlyoffersconveniencebutalsofostersasense


WIA1002-DataStructure

of ownership and continuity for players, making their journey through the
PokémonKantoregionmoreimmersiveandenjoyable.

### 4. Database Implementation

Forthoseseekingtoelevatetheirgamedevelopmentskills,transitioninginto
the realmof databasesoffersacompellingopportunity.Whetherforstoring
game progress or managing user accounts, implementing a database
provides a structured approach to data management. By leveraging a
database system, such as MySQL or SQLite, developers can establish a
robust foundation for storing and retrieving game-related information. This
notonlyenhancesthereliabilityofdatastoragebutalsominimizestheriskof
data loss or inconsistencies within the application. Integrating a database
empowersdeveloperstoorganizeandaccessgamedataefficiently,ensuring
asmootherandmoreseamlessgamingexperienceforplayerstraversingthe
PokémonKantoregion.

## Marksdistribution

```
MainFeatures Codingandcorrectoutputs 13 marks
ExtraFeatures 2 marks
Report Properexplanationsofcode 5 marks
Documentation(JavaDoc
commentformat)
Collaboration(GitCommits
andContributionspage)
```
Doingjustoneoftheextrafeaturesshouldgetyouthe 2 marks,butifyoufeel
like your main featuresare not fully functional, you can try tomakeupfor
those marks by doing more extra features or improving the game in any
significantwayyoucanthinkof.


WIA1002-DataStructure

## TipsandRecommendations

### FromAmaanGeelani

```
● Thisassignmentwascreatedthroughmytotallyhealthyobsessionwith
thePokémonfranchise,boththegamesandtheshow.
● Trytounderstandhoweachclassandobjectinthesysteminteracts.
● Divideworkonthebasisofequaldifficulty,usegitandgithubtoensure
easycollaboration.
● If you are not as obsessed with Pokémon, you should consider
researching on the Bulbagarden Website about Pokémon, Gyms,
Areas,Trainers,etc.
```
### FromNavid

```
● Commencethe assignmentwellin advanceto avoidrushingnearthe
deadline,asprocrastinationcouldjeopardizetimelycompletion.
● Ensurethoroughincorporationandrigoroustestingofallmainfeatures
within your program to validate their functionality through repeated
trials.
● Above all, immerse yourself in the Pokémon universeand relishthe
journey!
```
```
Image 13 - AshandPikachu
```

WIA1002-DataStructure

## ContactInformation

Tostayupdatedaboutchangesandupdatestotheassignment:

- https://github.com/isyedamaan/DS-Project-Pokemon

If you're seeking to address the individual responsible for the Pokémon
assignment,orsimplywishtodiscussPokémon-relatedtopics,we'vegotyou
covered.

Forthose whowanna ask questions relatedto theassignment,feelfreeto
contactus:

- AmaanGeelaniSyed (s2191704@siswa.um.edu.my)
- NavidRazavi(s2110706@siswa.um.edu.my)

Whether you prefer onlineor in-personinteractions,Amaanisdown totalk
aboutallaspectsofthePokémonworld.

Foranyquestionsorfeedbackregardingtheassignment,feelfreetocontact
either of us. We're here to assist you andensureyou'reequippedforyour
Pokémonadventure!

```
Image 14 - Ash,Pikachu,BrockandMistyfromthePokémonanime
```

