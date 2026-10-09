# Reflektion – Skogsäventyret

**Namn:** Murtaza Sultani  
**Kurs:** Grundläggande objektorienterad programmering i C#  
**Projekt:** Skogsäventyret  
**Datum:** 9 oktober 2026  
## Vad var svårast?
Det svåraste var att förstå hur olika klasser samarbetar i spelet, särskilt Player, Monster och BattleSystem.
Jag var inte med från början i grupparbetet, så jag behövde läsa koden noggrant för att förstå strukturen. 
Jag lärde mig också varför Console.ReadLine kan ge null och hur operatorn ?? gör att programmet får en tom text i stället för ett fel.
kan du fixa den att det ska komma rätt och jag ska bara kopiera den och klistera in det i min reflektionen. 
## Hur fungerade samarbetet i gruppen?
 Jag kom inte in i gruppen från början, men jag försökte sätta mig in i projektet och bidra på ett tydligt sätt.
 Jag arbetade med att rätta null-varningar i min egen fork och gjorde separata commits för ändringarna. Samarbetet fungerade genom att jag kunde läsa gruppens kod och förstå hur delarna hängde ihop.
 ## Vad hade du gjort annorlunda?
 Om jag hade varit med från början hade jag deltagit mer i planeringen av klasserna och spelreglerna.
 Jag hade också gjort mindre commits tidigare under arbetet för att lättare kunna följa ändringarna i Git. 
 Nästa gång vill jag testa programmet oftare medan jag skriver kod, i stället för att vänta tills flera ändringar är klara.
 ## Så fungerar spelet? 
 Player är klassen som lagrar spelarens värden, till exempel hälsa, attack, försvar, guld och erfarenhetspoäng.
 Monster är en grundklass för fiender i spelet och innehåller information som namn, hälsa, attack och belöning.
 Goblin, Orc och Ogre ärver från Monster, vilket betyder att de kan använda samma grundfunktioner men ha olika värden.
 BattleSystem styr en strid mellan spelaren och ett monster och visar valen attackera, försvara eller springa. 
 När spelaren attackerar räknas skadan ut från spelarens attack och monstrets försvar. 
 Om monstrets hälsa blir noll eller mindre får spelaren erfarenhetspoäng och guld. 
 I BattleSystem.cs ändrade jag Console.ReadLine() till Console.ReadLine() ?? "",
 vilket betyder att programmet använder tom text om användaren inte skriver något. Det gör att programmet undviker null-varningar och kan hantera inmatning säkrare.
