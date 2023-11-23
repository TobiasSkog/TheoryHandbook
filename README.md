# TheoryHandbook
My solution to the Theory Handbook assignment by Tobias Skog of class .NET23

# 1. Vad är skillnaden på .NET och C#?
## .NET
**.NET** är ett verktyg för utvecklare, ett så kallat [framework](https://github.com/TobiasSkog/TheoryHandbook/blob/main/Framework.md), som Microsoft utvecklade. 
**.NET** har ett många verktyg och en uppsjö av [libraries](https://github.com/TobiasSkog/TheoryHandbook/blob/main/Libraries.md) som underlättar utvecklandet av applikationer riktade mot webben, mobiler och datorer.

**.NET Core** är ett så kallat [cross-platform](https://github.com/TobiasSkog/TheoryHandbook/blob/main/Cross-Platform.md) [framework](https://github.com/TobiasSkog/TheoryHandbook/blob/main/Framework.md) som tillåter utvecklaren att lätt skapa produkter för olika typer av operativsystem (Windows, Linux, macOS, iOS, Android).

**.NET Core** 1.0 släpptes i juni 2016 och sedan dess har .NET vart open-source!

**.NET** använder sig av **CLR (Common Language Runtime)** vilket är en implementation av **[CLI](https://github.com/TobiasSkog/TheoryHandbook/blob/main/CLI.md)** som är en internationell standard. Detta innebär att att **.NET** kan köra kod och libraries som är skrivna i olika programmeringsspråk men är kompatibel med **.NET's** [CLR](https://github.com/TobiasSkog/TheoryHandbook/blob/main/CLR.md) och [CLI](https://github.com/TobiasSkog/TheoryHandbook/blob/main/CLI.md).
**.NET's** [CLR](https://github.com/TobiasSkog/TheoryHandbook/blob/main/CLR.md) använder sig av **[JIT](https://github.com/TobiasSkog/TheoryHandbook/blob/main/JIT.md)** kompilering som konverterar [IL](https://github.com/TobiasSkog/TheoryHandbook/blob/main/IL.md) koden till instruktioner som datorn förstår [Binär kod](https://github.com/TobiasSkog/TheoryHandbook/blob/main/Bin%C3%A4rKod.md). Språkinteroperabilitet är en nyckelfunktionen i **NET** [IL](https://github.com/TobiasSkog/TheoryHandbook/blob/main/IL.md) koden producerad av C# kompilatorn överensstämmer med **[CTS (Common Type Specification)](https://github.com/TobiasSkog/TheoryHandbook/blob/main/CTS.md)**.
Vilket innebär att IL kod som är genererad i C# kan interagera med annan kod som har är kompatibel med samma CTS som **.NET** kan tyda, dvs Du är inte begränsad till att enbart använda dig av programmeringsspråket C# då du som utvecklare använder dig av **.NET** och så länge språket är kompatibelt med **.NET** [CTS](https://github.com/TobiasSkog/TheoryHandbook/blob/main/CTS.md) så kan kod i olika programmeringsspråk kommunicera med varandra utan avbrott eller kostnad av hastighet eller prestanda.

**.NET** är inte begränsat till att bara använda sig av programmeringsspråket **C#** utan stödjer **C#**, **F#**, **Visual Basics**, **C++**, **ClojureCLR**, **IronPython**, **PowerBuilder**, **Swift**, **PowerShell** och mer!
## C\#
**C#** är ett programmeringsspråk, också skapat av Microsoft, specifikt avsätt för att arbeta med deras **.NET** plattform! Det släpptes i februari 2002.

**C#** är ett objekt-orienterad programmeringsspråk och dess syntax har tagit mycket av C++ och Java. 

**C#** har en automatisk skräp insamling funktionalitet, "garbage collection", som skiljer C# från t.ex. C++ där utvecklaren själv måste se till att frigöra minne i sin kod.

-------------------
# 2. Vad är skillnaden på en IDE och en kod editor?
## IDE
En **IDE (Integrated Development Environment)** är en mjukvara som är till för att hjälpa utvecklare att utveckla projekt mer effektivt och erbjuda mer funktionalitet än att bara kunna skriva sin kod.
Funktionaliteter så som att bygga koden till ett program, skapa och använda unit tests, smart kod avslut där utvecklaren kan få förslag på kod stycket eller metoden de vill skriva och till och med utskriven åt en, verktyg för att omstrukturera sin kod, kompilerar koden till ett språk som ditt operativsystem kan förstå och en riktigt stark funktionalitet är debugging verktygen som många IDE's har som tillåter utvecklare att debugga och hitta problem i sin kod.
## Kod Editor
En **kod editor** är enbart en mjukvara som låter utvecklare skriva sin kod i. Den behöver inte ha någon funktionalitet för att underlätta eller hjälpa utvecklaren i sitt skrivande av koden, utan bara finnas där för att skriva koden. 

Du kan skriva din kod i Microsofts program "Notepad". Den kommer inte hjälpa dig med något av skrivandet av koden, men tillåter dig att öppna en fil och spara den till olika typer av format där du som utvecklare själv är ansvarig för att skriva din kod.

-------------------
# 3. Vilka varianter/versioner av .NET är aktuella i dagsläget?
I dagsläget så har vi följande .NET versioner att förlita oss på vid skapande av nya projekt.

LTS  = Long Term Support. Får aktivt uppdateringar i 36 månader.
STS = Standard Term Support. Får aktivt uppdateringar i 18 månader.

.NET 6 som är LTS fram tills Nov 2024.
.NET 7 som STS fram tills Maj 2024.
.NET 8 Som är den senaste LTS fram tills 2026

-------------------
# 4. Lista de datatyper och datastrukturer som du känner till i .NET/C\#
### Datatyper
| Datatyp i .NET | Värde                                                                                              | Datatyp i C# | 
| -------------- | -------------------------------------------------------------------------------------------------- | ------------ |
| System.Int64   | Signerat heltal som tillåter värden från -9,223,372,036,854,775,808 till 9,223,372,036,854,775,807 | long         |
| System.UInt64  | Osignerat heltal som tillåter värden från 0 till 18,446,744,073,709,551,615                        | ulong        |
| System.Int32   | Signerat heltal som tillåter värden från -2,147,483,648 till 2,147,483,647                         | int          |
| System.UInt32  | Osignerat heltal som tillåter värden från 0 till 4,294,967,295                                     | uint         |
| System.Int16   | Signerat heltal som tillåter värden från -32,768 till 32,767                                       | short        |
| System.UInt16  | Osignerat heltal som tillåter värden från 0 till 65,535                                            | ushort       |
| System.String  | Text med max storlek på 2GB minne vilket representerar ca 1 Miljard karaktärer                     | string       |
| System.Boolean | Byte värde på 0 eller 1 som vi läser som "True" eller "False"                                      | bool         |
| System.Byte    | Osignerat heltal som tillåter värden från 0 till 255                                               | byte         |
| System.SByte   | Signerat heltal som tillåter värden från -128 till 127                                             | sbyte        |
| System.Char    | Karaktär                                                                                           | char         |
| System.Single  | Decimaltal som tillåter värden från ±1.5 x 10−45 till ±3.4 x 1038                                  | float        |
| System.Double  | Decimaltal som tillåter värden från ±5.0 × 10−324 till ±1.7 × 10308                                | double       |
| System.Decimal | Decimaltal som tillåter värden från ±1.0 x 10-28 till ±7.9228 x 1028                               | decimal      |

#### Heltal och decimaltal
Beroende på vad du behöver använda en siffra till i ditt program så kan du optimera mängden minne du ger din variabel genom att ge den rätt datatyp.
T.ex. ska vi representera en människas ålder i våran kod, så räcker en `byte` då en människa inte har en livstid som går över max värdet på en byte av `255`. 
Ska vi räkna med pengar så ska vi alltid använda oss av datatypen `decimal` för att kunna få så exakt värde som möjligt i våra kalkylationer så behöver vi tillgång till så många decimaler som vi möjligtvis kan tillåta.
#### Text och karaktärer
en string är en en array av karaktärer string text = "Hej allihopa!";  är samma sak som en char[] karaktarsArray = {'H', 'e', 'j', ' ', 'a', 'l', 'l','i','h',o','p','a','!'}; 
### Datastrukturer
**Array** 
En behållare som kan innehålla olika typer av data med en specifik storlek som sparar data på en exakt plats i minnet vilket gör det lätt att veta en specifik plats på specifik data för att lätt få tillgång till den. Statisk storlek, när en array är skapad med en storlek så krävs det att man skapar en ny array om man vill ha större storlek på arrayen. Indexen i en array börjar på 0

**List**
En behållare som kan innehålla olika typer av data med en DYNAMISK storlek, dvs den ändrar storleken på listan allt eftersom data läggs till eller tas bort. Varje element i listan har ingen aning om vad som kommer före eller efter den och tar en mindre plats i minnet än en array som alltid behöver vara en specifik storlek, även innan den är full

**Linked List**
Samma som en array fast skillnaden är att varje element har en reference till nästa element i listan, bortsett från sista elementet i listan som inte kan ha en referens till nästa element då det inte finns något (null)

**Sorted List**
En lista som är sorterad efter sitt värde, default så sorteras listan stigande (lägst på index 0 och högst på sista platsen)

**Stack** 
En behållare som kan innehålla olika typer av data som styrs av ett "LIFO (Last In First Out)" system

**Queue**
En behållare som kan innehålla olika typer av data som styrs av ett "FIFO (First In First Out)" system

**Dictionary**
En behållare som kan innehålla olika typer av data t.ex. Dictionary<string, int> innehåller en `key` av typen `string` och har ett `value` av typen `int` 
```Csharp
Dictionary<string, int> myDictionary = new()
{
    {"Tobias", 31 }
};
```
Illustrerar ett dictionary där `key` `"Tobias"` har värdet `31`. I detta fall ett `namn` och `ålder`.

-------------------
# 5. Beskriv i korthet med egna ord objektorientering och vad det handlar om
Objekt Orienterad Programming (OOP) är ett sätt att bryta ner din kod till klasser, en typ av beskrivning av ett objekt.

Vi ska ta och illustrera det här med ett exempel, vi ska skapa en ny klass och vi kan då beskriva vad ett objekt är i verkliga livet. 
Vi skapar en klass Bok!
```c#
public class Bok
{

}
```
Här har vi en klass som vi kallar för `Bok` som vi vill använda oss av för att hantera data som är relaterat till en Bok. Klassen beskriver objektet, och den innehåller datan för våran bok.

Så vi kan lägga till i våran beskrivning / ritning av en bok att den ska ha en titel och en författare
```c#
public class Bok
{
	string Title;
	string Författare;
}
```

Vi kan nu skapa en bok i vårat program så här
```c#
Bok programmeringsBok = new()
{
	Title = "Programming";
	Författare = "Bjarne Stroustrup";
};
```

Vi har nu tillgång till våran `programmeringsBok` och kan använda datan i vårt program framöver eller till med låta den interagera med andra klasser.


```c#
Console.WriteLine(programmeringsBok.Title);
```
Här skriver vi ut datan i attributen Title i våran instans av klassen Bok.

Output:
```
Programming
```


Du kan även skapa klasser som innehåller en viss funktionalitet, du kanske vill hantera validering av konvertering från text till siffror i ett program från en användare. Men det vore in logiskt att behöva ha en ny instans av din klass varje gång du skulle behöva göra den här kontrollen, så då kan vi göra den statisk. En statisk klass får inte ha några attributer men som vi ser i fallet nedan så finns inget behov för det. Fördelen är att vi direkt kan skriva i vårat program:
`IntValidationHelper.GetIntegerNoMinOrMaxRange("Ange ett heltal: ");`
```c#
 public class IntValidationHelper
 {

     public static int GetIntegerNoMinOrMaxRange(string prompt)
     {
         while (true)
         {
             Console.WriteLine(prompt);
             if (int.TryParse(Console.ReadLine(), out int validInt))
             {
                 return validInt;
             }
         }
     }
 }
```

Nu har vi skapat en klass som har en metod, denna kan vi kalla i vårat program istället för att behöva repetera och skriva om koden om och om igen.

### Fördelar med OOP
1. Återanvändbar kod, ibland en stor majoritet av ditt projekt kan återanvändas i ett nytt projekt!
2. Ökar produktiviteten.
3. Minskar chansen för fel då vi inte behöver skriva om koden ett flertal gånger och kanske vara lite uttråkad att göra samma sak för 39e gången och göra ett litet fel.
4. Ökar markant lättnaden att debugga kod och hitta fel. Då våran kod för att hantera konvertering är på ett och samma ställe är den lätt att hitta och ändra, vi behöver bara göra ändringen på ett ställe, inte på alla andra ställen.
5. Vi ökar säkerheten då vi oftast har alla attributer / fält märkta som privata och har metoder som ger användaren tillåtelse att se värdet men för att ändra dem så måste man kalla på en funktion i klassen och enbart kod inne i klassen kan ändra på värderna.


### Nackdelar med OOP
1. I ett litet program som t.ex ska skriva ut vad använder skriver blir onödigt och implementationen av klasser blir istället en långsammare och tyngre process än att bara köra ditt lilla program direkt i main:
```c
public class Program
{
	static void Main(string[] args)
	{
		while(true)
		{
			var userInput = Console.ReadLine();
			Console.WriteLine($"User: {userInput}");
		}
	}
}   
```
vs
```c
public class Program
{
	static void Main(string[] args)
	{
		Echo echo = new();
		while(true)
		{
		echo.UserInput();
		UserInteraction.WriteToConsole(echo.GetUserInputString());
		}
	}
}   
```
```c
public class Echo
{
	private string UserInputString { get; set; }
	public static void UserInput()
	{
		UserInputstring = Console.ReadLine();
	}
	public string GetUserInputString()
	{
		return userInputString;
	}
}
```
```c
public static class UserInteraction
{
	public static void WriteToConsole(string prompt)
	{
		Console.WriteLine(prompt);
	}
}
```
Som du kan se går det lätt att göra en väldigt simpel process överkomplicerat och ta mer resurser från utvecklare att skapa och prestanda från din maskin för att köra än vad som behövs för ändamålet av detta program.

2. OOP har förkärleken att vara lite av en "fri tolkning" och kan leda till problem om inte en struktur anges om vad just projektet du arbetar med räknar som OOP. I verkligheten är det en stor majoritet av företag som säger att det jobbar med just OOP fast vad dem egentligen gör är att arbeta "OOP inriktat" och inte fullt ut med OOP i fokus.


# 6. Lista de mekaniker och andra begrepp inom OOP som du lärt dig i kursen så som exempelvis klasser, arv och polymorfism (det finns dock fler). Till varje punkt du listar ska du skriva en kort beskrivning av vad det innebär med egna ord. Skriv ca 50-100 ord om varje.
## Klasser
En klass kan man förklara som en beskrivning av ett fysiskt objekt, t.ex. en `Bok`. Våran klass innehåller metoder och / eller attributer relaterat till vad vi ser att en `Bok` ska ha. Den kan attributer som `Titel`, `Författare`, `Genre`, `Beskrivning` osv. En klass är ett sätt att samla data på och metoder relaterade till det objektet där vi kapsylerar datan och skyddar den från yttre störningar. Vi kan sätta våra attributer till `private` och därmed blockerar våran kod att komma åt bokens titel utanför klassen. Det enda sättet vi kan komma åt den är att ha kod inne i vår klass som t.ex. returnerar eller ändrar värdet på attributen. 
Att fördela koden i objekt är också användbart för att skapa en mer lättläst och förståelig kod som inte behöver repeteras, om vi ville skapa ett bibliotek med 1 miljoner böcker, så skulle det ta otroligt mycket kod att skriva ut koden för varje bok 1 miljoner gånger när vi istället kan skapa en ny instans av en bok med datan vi vill ha i den i t.ex en for loop som loopar 1 miljon gånger. Vi har nu bara några få rader kod istället för en fil stor nog att skapa problem för användaren. Tänk dig att göra en ändring på din boks kod om du behöver repetera den så många gånger vs att ha den som en klass där du enkelt ändrar din kod på ett ställe och alla böcker får tillgång till ändringen, eller tillägget av kod utan några bekymmer.
## Arv
Arv tillåter en klass "ärva" propterties och metoder från en annan klass för att kunna vidareanvända dem för sig själv. Detta gör koden väldigt återanvändbar och är en det största anledningarna vi programmerar med OOP. Arv är inte begränsat till en generations arv, utan du kan ha flertal klasser som ärver från en bas klass eller klasser som ärver efter varandra. 
T.ex.
```c
public class Error
{
	public string Message { get; set; }
}
public class FatalError : Error
{
	public string Message { get; set; }
	public string CodeThatKilledTheProgram { get; set; }
}
public class MinorError : Error
{
	public string Message { get; set; }
	public string 
}
```
## Polymorfism
### Statisk Polymorfism
Statisk polymorfism kan man också kalla för en "statisk bindning" eller "tidig bindning" det är en så kallad metod överlagring.
En statisk bindning används när en subklass har samma metod som sin basklass men utan att använda nyckelordet `virtual` eller `abstract` i basklassen och `override` i subklassen. T.ex. 
```c
public class Animal
{
	public void MakeSound()
	{
		Console.WriteLine("Animal makes a sound");
	}
}

public class Dog : Animal
{
	public void MakeSound()
	{
		Console.WriteLine("Dog barks");
	}
}
```
Om vi skapar en ny instance av klassen Dog och kallar på dens metod `MakeSound()`så kommer vi skriva ut `Dog barks`. Men skulle vi referera våran instans av Dog som Animal så kommer vi skriva ut `Animal makes a sound`.
```c
Dog dog = new Dog();
dog.MakeSound()
```
> Output: Dog barks
```c
Dog dog = new Dog();
Animal animal = dog;
animal.MakeSound();
```
> Output: Animal makes a sound

Så i detta fallet ser vi skulle vi skapa en lista av typen `Animal` för att sortera alla våra subklasser i vårat zoo och sedan loopa igenom den med en foreach loop och inte ha en override då vi gör referensen så skulle vi aldrig få våra specifika djurs `MakeSound()`metoder.
### Dynamisk Polymorfism
Dynamisk polymorfism kan man också kalla för en "dynamisk bindning" eller "sen bindning", detta är det man vanligtvis talar om när man talar om "polymorfism".
En dynamisk bindning används när en subklass har samma metod som sin basklass och använder sig av nyckelordet `virtual` eller `abstract` i basklassen och `override` i subklassen. T.ex. 
```c
public class Animal
{
	public virtual void MakeSound()
	{
		Console.WriteLine("Animal makes a sound");
	}
}

public class Dog : Animal
{
	public override void MakeSound()
	{
		Console.WriteLine("Dog barks");
	}
}
```
Om vi skapar en ny instance av klassen Dog och kallar på dens metod `MakeSound()`så kommer vi skriva ut `Dog barks`. Refererar vi våran instans av Dog som Animal så kommer vi skriva ut `Dog barks`.
```c
Dog dog = new Dog();
dog.MakeSound()
```
> Output: Dog barks
```c
Dog dog = new Dog();
Animal animal = dog;
animal.MakeSound();
```
> Output: Dog barks

Om vi denna gången skapar en lista av typen `Animal` som vi loopar med en foreach loop och kallar metoden `MakeSound()` så kommer vi få våran subklass implementation av den istället för basklassen `Animal.MakeSound()`.

Vi kan sätta upp våran basklass som en `abstract`klass istället, på så sätt hindrar vi att basklassen kan skapas i vårat program och den kommer användas som en ritning för utvecklaren om vad som måste finnas med då vi skapar ett arv av våran basklass. En abstract metod får inte ha någon "kropp" dvs ingen kod mellan `{` och `}` och metoden avslutas direkt med `;`.
T.ex.
```c
public abstract class Animal
{
	public abstract void MakeSound();
}

public class Dog : Animal
{
	public override void MakeSound()
	{
		Console.WriteLine("Dog barks");
	}
}
```
Om vi inte skulle ha metoden `MakeSound()` i våran subklass så kommer vi få ett error, då våran abstracta basklass, våran instruktion om hur subklassen ska se ut, inte har allt som våran basklass säger att vi måste ha.
## Properties
En klass kan ha `Properties` som är specifika variabler för den klassen och som man kan tilldela i konstruktorn för att skapa en specifik instans av den klassen med dem specifika värderna.
Om vi tänker på vårat Bok exempel från tidigare: 
```c
public class Bok
{
	string Title;
	string Författare;
}
```
Så ser vi att Bok har 2 variablar Title och Författare, dessa är fält, men vi kan ändra dem till en Propertie t.ex så här:
```c
public class Bok
{
	string Title {get;set;}
	string Författare {get;set;}

	public Bok(string title, string författare)
	{
		Title = title;
		Författare = författare;
	}
}
```
Här la vi till `{get;set;}` som är getters och setters och gör vårat fält till en proterty istället. Dessa säger att om vi i vårat programm försöker komma åt en speicifk instans av objektet Bok så kan vi tack vare `get` få tillgång att se värdet på den variabeln och tack vare `set` ändra värdet på den variabeln.
```c
Bok minBok = new Bok("Harry Potter och de vises sten", "J. K. Rowling")
// Skapar en ny instans av våran Bok som vi kallar för minBok
// Vi använder oss av klassens konstruktor för att tilldela en titel och en författare
// Vi kan nu få tillgång till dessa properties från våran specifika bok

Console.WriteLine(minBok.Title);
// Output: Harry Potter och de vises sten
Console.WriteLine(minBok.Författare);
// Output: J. K. Rowling
```
Detta är väldigt användbart för om vi skulle skapa ett bibliotek med flera tusen böcker så har vi faktiskt sätt att kunna sortera dem, kunna hitta en specifik bok som vi vill ha t.ex
```c
List<Bok> bibliotek = new();
// Låtsas att vi har lagt till 10'000 böcker i våran lista
// Då kan vi loopa och leta efter en bok med en specifik författare, eller titel
foreach(var bok in bibliotek)
{
	if(bok.Titel == "Harry Potter och de vises sten")
	{
		Console.WriteLine("Hittade boken vi skapade i förra exmplet!")
	}
}
```

alternativt kan vi göra så här också:
```csharp
List<Bok> bibliotek = new();
// Låtsas att vi har lagt till 10'000 böcker i våran lista
string hittaBokMedDennaTitel = "Harry Potter och de vises sten";
bool hittadeBoken = false;
foreach(var bok in bibliotek)
{
	if(bok.Titel == hittaBokMedDennaTitel)
	{
		hittadeBoken = true;
	}
}

if(hittadeBoken)
{
	Console.WriteLine("Vi hittade din bok!");
}
else
{
	Console.WriteLine("Vi hittade tyvärr inte din bok i biblioteket!")
}
```
## Enkapsylering
Är ett sätt att skydda och gömma data om din klass och limitera att kod utanför kan ändra på värderna i dina properties eller fält utan istället måste kalla en metod i klassen som sköter ändringen av värdena.
```csharp
public class Bok
{
	public string Title {get; private set;}
	public string Författare {get; private set;}
	public string Ägare {get; private set;}
	public Bok(string titel, string författare, string ägare)
	{
		Författare = författare;
		Titel = titel;
		Ägare = ägare;
	}

	public void ÄndraÄgare(string nyÄgare)
	{
		if(string.IsEmptyOrNull(nyÄgare))
		{
			Console.WriteLine("Ägaren uppdaterades INTE! Du angav en tom string som input.")
			return;
		}
		Ägare = nyÄgare;
	}
}
```
I detta exemplet så har vi lagt till property Ägare, vi har även gjort dem public, men med en `private set` vilket betyder att det är bara kod inuti denna klass som får ändra värden på variabler och det går inte att nås utanför
```csharp
Bok minBok = new Bok("Harry Potter och de vises sten", "J. K. Rowling". "Tobias Skog")
Console.WriteLine(minBok.Ägare)
// Output: Tobias Skog
minBok.Ägare = "Reidar";
// Detta ger oss ett fel, då vi har `private set` så får vi inte ändra värdet på vår variabel utanför klassen och måste istället då använda oss av våran metod ´ÄndraÄgare()´
minBok.ÄndraÄgare("");
// Output: Ägaren uppdaterades INTE! Du angav en tom string som input.
minBok.ÄndraÄgare("Reidar");
// Output: Reidar
```
Vi kan även göra våra properties:
	private = Enbart den specifika klassen kan ändra värdet på dem
	protected = Enbart den specifika klassen OCH de klasser som ÄRVER från den kan ändra värdet på dem
	internal = Enbart klasser och kod inom samma PROJEKT kan ändra på värdena
	public = ALLA som har tillgång till koden kan ändra på den
## Data Abstraktion
Ett sätt att fokusera på VAD som ska göras och inte HUR.
Vi kan göra en klass eller en metod abstrakt där vi säger att metoden SKA finnas, men HUR den fungerar det får varje klass implementera själv.
```csharp
public abstract class LivingThing
{
	public abstract void Breathing();
}
```
Vi skapar en klass av ett levande ting och vill att den ska ha funktionalitet att kunna andas. HUR varje klass som ärver detta väljer att implementera funktionalitet att andas är oviktigt, det viktiga är att den KAN göra det.
```csharp
public class Human : LivingThing
{
	public override void Breathing()
	{
		Console.WriteLine("Air is pulled into your nose or mouth, and into your windpipe. This divides into airways supplying the left and right lungs. The air passes down the airways, which divide another 15 to 25 times, and finally into thousands of smaller airways until the air reaches the air sacs.");
	}
}

public class Fish : LivingThing
{
	public override void Breathing()
	{
		Console.WriteLine("Fish take water into their mouth, passing the gills just behind its head on each side. Dissolved oxygen is absorbed from—and carbon dioxide released to—the water, which is then dispelled. The gills are fairly large, with thousands of small blood vessels, which maximizes the amount of oxygen extracted.");
	}
}
```

Här ovan ser vi att HUR det fungerar är väldigt olika, men funktionaliteten finns med i båda oavsett HUR.
# 7. Beskriv översiktligt vad UML är och ta med en bild som visar en UML du har skapat själv.

**UML** Står för **U**nified **M**odeling **L**anguage och är ett visuellt modelerings språk som finns till för att hjälpa utvecklare att visualisera och strukturera kod / projekt.

Det är inte någon form av programmering språk utan mer ett regelvärk för att göra diagram om hur din kod körs, hur klasser interagerar med andra klasser m.m.

I detta exempel så har vi 2 UML diagram på klassen `Bok` och klassen `Bibliotek`
![image](https://github.com/TobiasSkog/TheoryHandbook/assets/11568812/3d29d755-8124-4b88-abe6-9b98a3384366)


Här ser vi att `Bibliotek` har en private property av typen `List<Bok>` som heter Böcker, vi har också 3 publika metoder
1. publika konstruktorn `Bibliotek` som inte tar någon input och används för att skapa en ny instans av klassen
2. publika metoden `LäggTillEnBokIBiblioteket` som tar en input `bok` av typen `Bok` 
3. publika metoden `TaBortEnBokUrBiblioteket` som inte tar någon input

Klassen `Bok` har 3 public properties `Titel`, `Författare` och `Ägare` alla av typen `string`, vi har också 2 publika metoder
1. publika konstruktorn `Bok` som tar en input på `titel`, `författare`, `ägare` alla av typen `string`
2. publika metoden `ÄndraÄgare` som tar en input på `nyÄgare` av typen `string`

# 8. Beskriv övergripande vad OOAD är. Förklara också varför man kan vilja använda OOAD när man utvecklar.
**OOAD** står för **O**bject **O**riented **A**nalysis and **D**esign och används som ett verktyg för att planera och strukturera projekt skriven med OOP i åtanke.
OOAD inkluderar OOP, design mönster, UML diagram och en beskrivning på hur progammet ska användas.

Fördelen med att använda sig av OOAD är precis som med kod skriven i OOP så kan du återanvända många komponenter för nya projekt och kan spendera mer tid på att optimera din kod istället för att ta fram ny kod.
Att använda sig av OOAD gör så projekten som följer denna strukturen är lättare att utöka och gör det lättare att hantera förändringar längre fram om t.ex användarbasen växer större och nya behov framdagas.
En viktigt del med OOAD är att det ska vara en modulär design som gör det lättare att skapa kod som ska vara underhållbar.




----------------

# **VG-fråga:** Resonera kring OOP-mekaniker

## 1. Välj ut tre mekaniker inom OOP. För varje mekanik du valt ska du resonera kring för- och nackdelar med den. Vad kan bli bättre respektive sämre i koden när dessa mekaniker används?

### Arv
#### Fördelar
Arv tillåter en klass att ärva egenskaper och metoder från en annan klassen, vilket ger möjligheten till återanvändning av kod. Detta i sin tur jobbar efter principen **DRY** (**D**on't **R**epeat **Y**ourself).

Arv gör också så att du skapar en hierarki av klasser, som leder till att koden blir mer strukturerad och lättförståelig (för det mesta).
#### Nackdelar
Ett problem som kan uppstå är  en dålig design vilket leder till tätt kopplade klasser, detta innebär att koden blir mindre flexibel, svårare att underhålla och onödigt komplex.

Ett anna problem kan vara **Diamond Problemet** när basklassen ärvs av två klassen som sedan ärvs av en klass så blir det otydligt och svårt att avgöra vilken metod som ska användas av vilken klass.
Referens: https://www.geeksforgeeks.org/multiple-inheritance-in-c/
### Inkapsling
#### Fördelar
 En klar fördel med inkapsling är säkerhet. Då inkapsling skyddar data genom att gömma det bakom metoder och förhindrar direkt åtkomst och manipulation av datan.
En annan fördel är att om man gör ändringar i implementationen av en metod kan man undvika att orsaka problem i andra delar i koden då dem inte är beroende på hur datan skapas utan bara returnen av datan.
#### Nackdelar
Det är möjligt att överanvända getter och setter metoder som ökar komplixiteten av koden och även minskar prestandan.

Det kan vara svårare att felsöka kod om man inte har tillgång till datan vid debugging och försöker avgöra orsaken från den indirekta åtkomsten av datan.
### Polymorfism
#### Fördelar
Tillåter utvecklaren att skriva mer flexibel och återanvändbar kod.
Du kan skapa ett generellt klass system som bygger på varandra för att bygga din slutprodukt.
T.ex. så kan du ha en klass för ett fordon, en klass för att starta en motor, en klass för att köra framåt, en klass för att köra framåt på vatten, en klass för att stanna osv...
Detta gör att vi kan återanvända många modulera i framtida projekt där vi enbart behöver små ändringar i våran kod istället för att måsta börja varje projekt med att bygga från grunden då vi redan gjort det. 
#### Nackdelar
Ett problem som kan uppstå är att vi ökar komplexiteten av koden när en och samma metod kan bete sig olika i olika sammanhang, detta kan också leda till kod som är svårare att underhålla.

I vissa situationen kan även polymorfism skapa prestanda problem, speciellt vid användning av dynamisk bindning.
# VG-fråga: Historiken för .NET
#### **.NET Framework historik**      **.NET Core historik**
| Version | CLR Version | Utgivningsdatum |     | Version | Utgivningsdatum |
| ------- | ----------- | --------------- | --- | ------- | --------------- |
| 1.0     | 1.0         | 2002-01-15      |     | 1.0     | 2016-06-27      |
| 2.0     | 2.0         | 2005-10-27      |     | 1.1     | 2016-11-16      |
| 3.0     | 2.0         | 2006-11-06      |     | 2.0     | 2017-08-14      |
| 4.0     | 4           | 2010-04-12      |     | 2.1     | 2018-05-30      |
| 4.5     | 4           | 2012-08-15      |     | 2.2     | 2018-12-04      |
| 4.5.1   | 4           | 2013-10-17      |     | 3.0     | 2019-09-23      |
| 4.5.2   | 4           | 2014-05-05      |     | 3.1     | 2019-12-03      |
| 4.6     | 4           | 2015-07-20      |     | 5       | 2020-11-20      |
| 4.6.1   | 4           | 2015-11-30      |     | 6       | 2021-11-08      |
| 4.6.2   | 4           | 2016-08-02      |     | 7       | 2022-11-08      |
| 4.7     | 4           | 2017-04-05      |     | 8       | 2023-11-14      |
| 4.7.1   | 4           | 2017-10-17      |     | 9       | 2024-11         |
| 4.7.2   | 4           | 2018-04-30      |     |         |                 |
| 4.8     | 4           | 2019-04-18      |     |         |                 |
| 4.8.1   | 4           | 2022-08-09      |     |         |                 |

Ovan ser vi en liten tabell som innehåller de flesta utgivningsdatum för både **.NET Framework** och **.NET Core**.  Notera att från version **.Net Core 5** så ändrades namnet på **.NET Core** till **.NET 5** > **.NET 6** >**.NET 7** osv.

Idag så stödjs **.NET Framework** version 4.6.2-4.8.1 och **.NET 6** - **NET 7** (och **NET 8** som släpps i november 2023).
##### .NET Framework
Används framförallt för att utveckla ASP.NET applikationer för windows.
##### .NET CORE
Är en open-source, cross-platform version av **NET Framework** som används för att utveckla majoriteten av moderna applikationer för ett flertal operativsystem
## Historiken för .NET
**.NET Framework 1.0** släpptes 2002-01-15. 

2016 började Microsoft med **.NET Core**, ett sätt att återskapa **.NET Framework's** funktionalitet men förbättra hastigheten. Dem ändrade så att **.NET Frameworks** [CLI](https://github.com/TobiasSkog/TheoryHandbook/blob/main/CLI.md) är nu **.NET Cores** **[CLR (Core Language Runtime)](https://github.com/TobiasSkog/TheoryHandbook/blob/main/CLR.md)**, de ändrade hur [IL](https://github.com/TobiasSkog/TheoryHandbook/blob/main/IL.md) skulle köras, vad som exekvera och när det skulle exekveras, vad som skulle stödjas och inte stödjas och släppte en del bakåt kompatibilitet. Detta ledde till en massiv ökning i hastighet. 
Det övergick också till helt Open-Source när det började med **.NET Core**!
De släppte även Visual Studio Code som Open-Source!
Detta ändrade deras strategi från att tjäna pengar på **.NET Framework** genom att folk installerade Windows på deras datorer eller serverar till att sälja cloud services.

De böt ut det abstrakta lagret av **.NET Framework** med **.NET Core** men stödjer fortfarande samma språk.

I början av **.NET Core 1** så stödes väldigt lite då de fortfarande jobbade febrilt med det. Först i version 3 så började man se en markant mängd av **.NET Framework** stödjas i **.NET Core** 

När **.NET 5 Core** släpptes så slutade de använda ordet `Core` för att det inte längre var en skillnad från **.NET Framework** utan att hade gått ifrån det och nu heter dem bara **.NET 5**, **.NET 6** osv..

När **.Net 6** släpptes så var målet att bara ha ett abstrakt lager kvar - **.NET 6** 
**.NET Framework** får inte längre nya uppdateringar med nytt innehåll sedan version 4.8, men kommer fortfarande att stödjas långt framöver. Medans **.NET 6, 7, 8...** Fortsätter att utvecklas och få ny funktionalitet och nya versioner.
Nya versioner av C# kommer att fungera med nyare versioner av **.NET** för att **.NET** kommer stödja nya versioner [IL](https://github.com/TobiasSkog/TheoryHandbook/blob/main/IL.md) som kommer vara aktuellt då den versionen släpps.
