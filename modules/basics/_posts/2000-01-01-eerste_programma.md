---
title: Je Eerste Programma
---

<div class="header1" id="top" markdown = "1"># Je Eerste Programma
</div>

<div class="header2" markdown = "1">## Visual Studio Installeren
</div>

Wanneer je een tekst wil schrijven, dan kan je dat doen met eender welk programma waar je in kan typen. Notepad is al voldoende. Toch zal je werk wellicht vlotter gaan als je een programma gebruikt dat specifiek bedoeld is voor het schrijven van teksten, zoals OpenOffice Writer of Microsoft Word.

Ook programmeren kan simpelweg in Notepad, maar ook hier geldt dat je het jezelf een stuk makkelijker maakt met een programma dat speciaal gemaakt is voor programmeurs en voor de programmeertaal die je gebruikt. In deze cursus gebruiken we C# om te leren programmeren. Daarom gebruiken we ook een editor die zeer geschikt is voor C#: **Microsoft Visual Studio**. Omdat we software ontwikkelen, noemen we dit ook wel een **ontwikkelomgeving** (**Integrated Development Environment** of **IDE**).

<div class="header2" markdown = "1">## Download & Installatie
</div>

Indien Visual Studio nog niet op je computer staat, dan moet je dit programma eerst downloaden. Ga naar de <a href="https://visualstudio.microsoft.com/vs/community/" target="_blank">Visual Studio website</a> en download de meest recente versie van Visual Studio.

Eens gedownload, moet je het installatieprogramma uitvoeren. Je kan akkoord gaan met de standaard opties bij het installeren. Kies zeker voor de **Community** versie: de professional en enterprise versies heb je echt niet nodig, en bovendien zijn die niet gratis. Vermijd de **Community _Insiders_** versie: deze is bedoeld om een omgeving met de allernieuwste snufjes uit te testen, maar is niet stabiel.

Wanneer de installatie gestart is, kan je _Workloads_ kiezen. Voorlopig heb je enkel de _.NET Desktop development_ workload nodig. Bij de _Installation details_ vink je bij _.NET desktop development - Optional_ volgende opties uit: _GitHub Copilot_ en _GitHub Copilot app modernization_. Deze staan het leerproces in de weg.  
Later in de cursus gebruiken we ook andere workloads, maar op dat moment is het eenvoudig om die toe te voegen.

![image](/img/basics/eerste_programma/netWorkload.JPG)

### Launch

Na het installeren kan je Visual Studio starten. De eerste keer zal je moeten inloggen _(je kan dat de eerste maand overslaan, maar daarna niet meer, dus maak je beter dadelijk een account)_. Inloggen moet gebeuren met een Microsoft Account. Gebruik hiervoor je school account gebruiken: `voornaam.familienaam@student.romerocollege.be`.

### Problemen?

Zit je vast met de installatie, bekijk dan <a href="https://www.youtube.com/watch?v=EF5YDkGu5Lk" target="_blank">deze video</a>. De eerste drie minuten tonen je hoe je Visual Studio installeert. _De rest van de video is niet van toepassing op deze cursus._

<div class="header2" markdown = "1">## Een Project Maken
</div>

Om code te kunnen schrijven heb je een project nodig. Afhankelijk van het soort applicatie dat je maakt, kies je een projecttype. In het eerste deel van deze cursus werk je uitsluitend met **Console** projecten.

### Een nieuw Console project

Als je Visual Studio 2026 opstart, krijg je automatisch de vraag om een bestaand project te openen of een nieuw project aan te maken. Je kiest voor _'Create a new project'_.  
![Startscherm](/img/basics/eerste_programma/01.png)

Stond Visual Studio al open, dan kan je een nieuw project aanmaken via het menu (_'File > New > Project/Solution'_).

In beide gevallen heb je nu het scherm waar je het projecttype kan kiezen. Filter eerst alle projecttypes die geschikt zijn voor C# door de taalfilter aan te passen van `All languages` naar `C#`. Kies nu voor `Console App`.  
![Create a new project](/img/basics/eerste_programma/02.png)

In de volgende stap controleer je dat je wel degelijk voor een **Console App** in **C#** gekozen hebt en kies je waar en onder welke naam jouw project opgeslagen wordt:

* **Project name:** `MijnEersteProgramma`  
Tip: voor het gemak is het eerste teken een letter en gebruik je geen spaties of speciale tekens!
* **Location:** Kies de folder van jouw repository  
Dit is iets als `C:\users\account\source\repos\iw-jouwnaam`
* **Solution:** `Create new solution`
* **Solution name:** Hier is het handig om een volgnummer voor de naam te zetten zodat al jouw projecten in _Windows Verkenner_ in volgorde getoond worden

![Configure your new project](/img/basics/eerste_programma/03.png)

In de laatste stap kies je nog enkele opties voor jouw project. Voor deze cursus zijn van belang:

* **Framework:** hier is `.NET 10.0 (Long Term Support)` een goede keuze
* **Do not use top-level statements:** in het begin vink je deze optie **niet** aan, later (bij het maken van functies en classes), doe je dit wel.

Op dit moment houden we dus de standaard opties:
![Additional information](/img/basics/eerste_programma/04.png)

### Je programma starten

Je kan je programma starten door bovenaan **Start** te kiezen. Je nieuwe programma zal de tekst `'Hello World'` op het scherm tonen. Sluit je programma af door op de spatiebalk te duwen.

<div class="note protip">
<p>Je zal dit jaar heel vaak een programma moeten starten. Dat kan via de button <b>Start</b>, maar nog sneller via de functietoets F5.</p>
</div>

### Code Aanpassen

Een programma bestaat uit code. Op dit moment geeft die code je computer de instructie om een console te tonen met daarin een tekst. Je kan deze code ook bekijken.

* Open de Solution Explorer als die nog niet zichtbaar is via _'View > Solution Explorer'_. 
* In de Solution explorer zie je een boomstructuur met bovenaan je _Solution_. In die Solution zie je je programma, met daarin alle bestanden die bij je programma horen. 
* Open het bestand **Program.cs**.
* Je ziet de volgende code. Welke regel zorgt er voor dat je een tekst op het scherm toont?

```csharp
// See https://aka.ms/new-console-template for more information
Console.WriteLine("Hello, World!");
```

<div class="note protip">
<p>Herinner je je de optie <strong>Do not use top-level statements</strong>? Had je die optie aangevinkt, dan had je code er nu als volgt uitgezien:
</p>
</div>
```csharp
namespace MijnEersteProgramma
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
        }
    }
}
```

<div class="note oefening">
<p>Pas de tekst 'Hello, World!' aan en start het programma opnieuw.</p>
</div>

<div class="toTop"><a href="#top">Omhoog</a></div>
