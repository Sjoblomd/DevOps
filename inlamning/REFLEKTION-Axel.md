# Individuell reflektion – Axel Rosenlew

När kursen började hade jag inte så bra koll på vad DevOps egentligen betyder. Jag hade använt Git, Docker och andra verktyg tidigare, men mest var för sig. Under kursen blev det mycket tydligare hur allt hör ihop från att man ändrar koden tills appen faktiskt körs i molnet.

Det jag lärde mig mest av var GitHub Actions, Docker, cPouta och Terraform. Jag tyckte speciellt att skillnaden mellan M7 och M8 var bra. I M7 gjorde vi allt manuellt i cPouta. Vi skapade VM, security groups, floating IP, SSH-access och installerade Docker själva. I M8 gjorde Terraform nästan samma sak automatiskt. Eftersom vi redan hade gjort allt för hand var det lättare att förstå vad Terraform faktiskt gjorde.

Git-delen blev också mycket tydligare för mig. Jag hade använt GitHub tidigare, men inte lika mycket med branch protection, pull requests och reviews. I M5 gjorde vi medvetet ett fel så att CI skulle faila. Då såg man tydligt hur GitHub kunde stoppa en dålig ändring innan den kom in på main.

Den svåraste delen var molnet. Det var ganska många saker att hålla koll på samtidigt, till exempel SSH-nycklar, IP-adresser, Docker, OpenStack och Terraform. När något inte fungerade var det inte alltid lätt att direkt se var felet var. Jag tycker ändå att det var nyttigt eftersom man lärde sig att felsöka steg för steg.

Att jobba i par fungerade bra. Vi kunde dela upp arbetet mellan oss, men eftersom vi använde samma repo och granskade varandras pull requests behövde båda ändå förstå vad som hände. Det gjorde att man inte bara kunde göra sin egen del och strunta i resten.

Det viktigaste jag tar med mig från kursen är att jag nu förstår hela kedjan mycket bättre. Jag ser tydligare hur en kodändring kan gå genom Git, tester, CI, Docker images och sedan ut till en server.

Om jag skulle göra kursen igen hade jag tagit screenshots och skrivit inlämningarna direkt efter varje milstolpe. Vi fick ofta tekniken att fungera först och tänkte på dokumentationen senare. Det gjorde vissa delar onödigt jobbiga i efterhand.

Överlag tycker jag att kursen gav mig en mycket bättre förståelse för DevOps. Jag känner mig nu mycket säkrare på GitHub Actions, Docker, moln och Terraform än före kursen.
