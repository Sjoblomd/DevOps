# M8 – Infrastructure as Code

## Vad vi gjorde utanför repot

Vi använde OpenStack CLI för att identifiera projektets interna nätverk och konfigurerade Terraform med rätt nätverk, GHCR owner, instansnamn och SSH-nyckel.
Vi körde sedan Terraform och skapade infrastrukturen i cPouta.
Den första deploymenten skapade åtta resurser och gav oss appens URL, nip.io-adress, floating IP och SSH-kommando.
För att verifiera att infrastrukturen kunde återskapas förstörde vi endast VM-resursen med en targeted destroy och körde sedan Terraform igen.
VM:n återskapades och samma floating IP behölls.

## Skärmdumpar

### Internal project network

![OpenStack network list](ScreenShots/m8/NetworkList.png)

### Terraform variables

![Terraform variables](ScreenShots/m8/TerraformVars.png)

### Initial Terraform deployment

![Initial Terraform apply](ScreenShots/m8/InitialApply.png)

### Targeted VM destroy

![Targeted destroy](ScreenShots/m8/TargetedDestroy.png)

### VM recreated

![Terraform rebuild apply](ScreenShots/m8/RebuildApply.png)