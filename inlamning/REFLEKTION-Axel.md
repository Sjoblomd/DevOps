# Individuell reflektion – Axel Rosenlew

Under kursen har vår tjänst gått från en enkel första commit till att kunna köras i molnet genom en nästan helt automatiserad kedja. I början, i M1 och M2, handlade mycket om Git och hur man jobbar bättre med branches, commits, pull requests och reviews. Jag hade använt GitHub tidigare, men under kursen blev det tydligare varför man inte bara ska pusha allt direkt till main. Branch protection och reviews gjorde att ändringar behövde granskas innan de blev en del av projektet.

Senare började vi lägga till mer automation. I M5 kom CI in i bilden. Där kördes tester och lint automatiskt när vi gjorde ändringar. Vi gjorde också medvetet ett fel och såg att pull requesten blockerades. Det var ett bra exempel på hur automation kan stoppa problem innan de kommer längre i kedjan.

Efter det jobbade vi mer med Docker och GitHub Actions. Vi byggde images för backend och frontend och publicerade dem till GHCR. Det gjorde att samma version av appen kunde köras på olika ställen utan att vi behövde installera allt manuellt varje gång.

M7 var den mest manuella delen av molnarbetet. Där skapade vi en VM i cPouta, security group, floating IP och SSH-access för hand. Vi installerade Docker själva och startade applikationen på servern. Det fungerade, men det var många steg där man kunde göra fel. I M8 blev skillnaden väldigt tydlig när vi gjorde samma typ av miljö med Terraform. Då kunde infrastrukturen byggas från kod istället för att vi behövde komma ihåg alla steg själva.

Till sist i M9 blev kedjan mer komplett genom automatiserad deployment. Då blev det tydligt hur hela kursen hänger ihop. En ändring i koden kan gå genom Git, testas automatiskt, byggas till Docker images och sedan användas i en miljö i molnet. I början gjorde vi mycket för hand, men mot slutet var mycket av processen automatiserad.

En konkret del som skulle bli mycket sämre utan automation är CI. I M5 såg vi att ett enkelt fel kunde blockeras automatiskt innan det mergades. Om vi istället skulle behöva komma ihåg att köra tester och lint själva varje gång, skulle det vara mycket lättare att glömma det. Då skulle fel kod kunna hamna på main.

Terraform är ett annat bra exempel. I M7 gjorde vi infrastrukturen manuellt, och det var ganska många steg som behövde bli rätt. Om man skulle göra samma sak varje gång för hand finns det stor risk att man glömmer någon inställning eller skapar miljöerna lite olika. Med Terraform kan samma miljö byggas på samma sätt igen.

Det viktigaste jag tar med mig från kursen är därför inte bara hur man använder verktygen, utan varför automation behövs. Den gör arbetet snabbare, men framför allt mer säkert och mer repeterbart. Jag förstår nu mycket bättre hur hela kedjan från commit till en fungerande tjänst i molnet hänger ihop.och sedan ut till en server.

Om jag skulle göra kursen igen hade jag tagit screenshots och skrivit inlämningarna direkt efter varje milstolpe. Vi fick ofta tekniken att fungera först och tänkte på dokumentationen senare. Det gjorde vissa delar onödigt jobbiga i efterhand.

Överlag tycker jag att kursen gav mig en mycket bättre förståelse för DevOps. Jag känner mig nu mycket säkrare på GitHub Actions, Docker, moln och Terraform än före kursen.
