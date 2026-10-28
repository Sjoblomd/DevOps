# Individuell reflektion – Daniel Sjöblom

Under kursen har jag fått en mycket bättre bild av hur en tjänst kan gå från kod till att faktiskt köras i produktion. I början jobbade vi mest med Git och hur man ska hantera kod på ett bättre sätt. I M1 och M2 jobbade vi med commits, branches, pull requests och reviews. Det gjorde att projektet blev mer strukturerat och att man inte bara gjorde ändringar direkt på main.

När vi kom till M5 började kedjan bli mer automatiserad. CI gjorde att tester och lint kunde köras automatiskt varje gång vi gjorde en ändring. Vi testade också att skapa ett fel med flit och såg att GitHub stoppade pull requesten. Det gjorde det ganska tydligt varför automatiska checks är viktiga.

Docker-delen var också viktig eftersom den fortsatte användas genom resten av kursen. Vi byggde images för backend och frontend och publicerade dem till GHCR. Då kunde samma images senare köras i cPouta. Det gjorde att man inte behövde bygga upp hela miljön från början på varje server.

I M7 gjorde vi mycket manuellt i molnet. Vi skapade VM, security group, floating IP och SSH-access och installerade Docker själva. Det var lärorikt, men samtidigt ganska lätt att missa någon liten inställning. I M8 använde vi Terraform för att bygga upp samma typ av miljö med kod. Då blev det tydligt hur mycket enklare det är att kunna skapa infrastrukturen på samma sätt varje gång.

I M9 blev hela flödet mer komplett när deployment också automatiserades. Då kunde man se hela kedjan från en ändring i GitHub till att appen kördes på servern. Det gjorde att DevOps kändes mer som ett helt arbetssätt än bara olika verktyg var för sig.

Om man tar bort automation från den här kedjan skulle mycket bli långsammare och mer osäkert. Ett tydligt exempel är deployment. Om vi skulle logga in på servern manuellt varje gång, hämta nya images och starta om tjänsterna själva, skulle det vara lätt att glömma något steg eller använda fel version. Det skulle också vara svårare att veta exakt vad som körs på servern.

Samma sak gäller infrastrukturen. När vi gjorde allt manuellt i M7 behövde vi själva hålla koll på många små inställningar. Om man hade flera miljöer skulle det vara väldigt lätt att de blev olika. Med Terraform finns inställningarna i kod och kan användas igen, vilket gör processen mycket tydligare.

Det viktigaste jag tar med mig från kursen är att automation inte bara finns för att spara tid. Den gör också arbetet mer stabilt och minskar risken för att människor gör olika eller glömmer steg. Efter kursen förstår jag mycket bättre hur Git, CI, Docker, moln, Terraform och deployment hör ihop i samma kedja.
