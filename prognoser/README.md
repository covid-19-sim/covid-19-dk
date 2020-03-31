# Prognoser

Her modellerer vi epidemikurven, og undersøger hvordan det kan gå, og hvad der kan ske, og hvad vi kan gøre.
Vi genimplementerer Sundhedsstyrelsens og Statens Seruminstituts modelberegning, kontrollerer
beregningerne og udvider med de manglende scenarier.

## Prognose fra Statens Seruminstitut og Sundhedsstyrelsen 22. marts 2020

Statens prognose er overordnet beskrevet i notatet *Håndtering af COVID-19: Prognose og kapacitet i Danmark for intensiv
terapi* (findes i kopi her: [ITA_COVID_19_220320.pdf](ITA_COVID_19_220320.pdf), ellers 
henvises til litteraturlisten nedenfor).

### Angrebsraten er pludselig kun best-case
Notatet nævner, at pandemier erfaringsmæssigt rammer 10-30% af befolkningen (*angrebsraten*) i første bølge, men så 
regner de kun efterfølgende på solskinsscenariet 10%. Sundhedsstyrelsen har tidligere meldt ud, at de regner med en 
*worst case* på 20% angrebsrate, men det scenarie behandles ikke, ej heller 30% scenariet, som der åbenbart er 
erfaring for er relevant.

Prognosen regner på erfaringer fra Kina (side 3, nederst), hvor de officielle kinesiske tal tages således for pålydende. 
Desuden regnes på italienske tal, der pakket ind i embedsmandssprog er "mere sammenlignelige" med danske forhold.

Desværre forklarer notatet ikke modellen til fulde, men vi gætter på, at der er tale om en SIR-model.

### Opgaveformulering SIR-model
Vi genimplementerer modellen som kontrol af resultaterne i notatet, tester den mod de empiriske observationer
og beregner de manglende scenarier.

Modellen er i [ssi_prognose_2020_03_22.ipynb](ssi_prognose_2020_03_22.ipynb)
 
 
## Eksponentiel prognose
Dette er en simpel, kortsigtet prognose for antal indlæggelser af forskellig art og dødsfald.
Vi bruger dagsaktulle tal fra Sundhedsstyrelsen og Seruminstituttet. 

Modellen findes i [eksponentiel_prognose.ipynb](eksponentiel_prognose.ipynb).

## Prognose fra Statens Seruminstitut og Sundhedsstyrelsen 30. marts 2020

Statens prognose er overordnet beskrevet i notatet *COVID-19 i Danmark - Status ved indgang til 5. epidemiuge* 
(findes i kopi her: [Status_COVID19_femte_uge.pdf](Status_COVID19_femte_uge.pdf), ellers 
henvises til litteraturlisten nedenfor).

Her modellerer vi epidemikurven.
Vi forsøger at genskabe notatets model, der denne gang er lidt bedre beskrevet; bl.a. nævner de at det *er* en 
SIR-model, hvilket vi i sidste uge var nødt til at antage ud fra de noget vage beskrivelser.

Notatet sætter en ny dato for **epidemistarten** til primo marts, da man har fundet COVID-19 positive de 
de løbende influenzaprøver, der tages i det såkaldte "sentinelprogram".

### Hvor længe skal Danmark være lukket?
Dette svarer de ikke på - faktisk snakker de meget om "røde" og "grønne" kurver (den røde er den hurtige epidemi, hvor
sundhedsvæsenet bryder sammen på grund af overefterspørgsel, den grønne er en lavere, hvor behandlingsbehovet holder 
sig under sundhedsvæsenets kapacitet). 

Notatet nævner, at vi er på den "grønne kurve", men viser ikke prognosen, de nævner blot (p. 26): 

> Det forventes, at der fortsat vil ses en stigning i antal påviste tilfælde, antal indlagte og intensiv patienter 
> i den kommende uge.Uden indgreb vil epidemien toppe først eller midt i april, men nu med indgreb forventes det at 
> blive en senere top, eller et affladet forløb.

SIR-modellen kan nemt beregne prognosen, så det giver ikke mening at udelade den, da den kvantificerer det 
uhåndterbare begreb "den grønne kurve" og  er essensen i beslutningsgrundlaget for de folkevalgte og regeringen, 
og som dokumentation og information til  borgerne, der er frataget deres levebrød, så længe Danmark holder lukket.  

Vi regner efter, og ser, om presseudlægningens og beslutningstagernes optimistiske udmeldinger
om situationen har noget på sig.

Modellen findes i [ssi_prognose_2020_03_30.ipynb](ssi_prognose_2020_03_30.ipynb)


## Litteratur

- Sundhedsstyrelsens notat, *Håndtering af COVID-19: Prognose og kapacitet i Danmark for intensiv terapi* 
(22. marts 2020, Sagsnr. 4-0101-33) hentet fra [Statens Seruminstitut](https://www.sst.dk/-/media/Nyheder/2020/ITA_COVID_19_220320.ashx?la=da&hash=633349284353F4D8559B231CDA64169D327F1227)
på adressen https://www.sst.dk/-/media/Nyheder/2020/ITA_COVID_19_220320.ashx?la=da&hash=633349284353F4D8559B231CDA64169D327F1227


- Sundhedsstyrelsens notat, *COVID-19 i Danmark - Status ved indgang til 5. epidemiuge*  (30. marts 2020, elektronisk ISBN: 978-87-7014-164-2). 
Udgivet på Sundhedsstyrelsens [hjemmeside](https://www.sst.dk/da/Udgivelser/2020/COVID-19-Status-paa-epidemien-uge-5). 
Selve notatet er hentet fra Sundhedsstyrelsens hjemmeside på adressen 
https://www.sst.dk/-/media/Udgivelser/2020/Corona/Status-og-strategi/Status_COVID19_femte-uge.ashx?la=da&hash=2889D7E5580B1450EB896A3A1EB69A1E4ADA93F6

