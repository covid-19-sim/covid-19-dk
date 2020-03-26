# Prognoser

Her modellerer vi epidemikurven, og undersøger hvordan det kan gå, og hvad der kan ske, og hvad vi kan gøre.
Vi genimplementerer Sundhedsstyrelsens og Statens Seruminstituts modelberegning, kontrollerer
beregningerne og udvider med de manglende scenarier.

## Prognose fra Statens Seruminstitut og Sundhedsstyrelsen

Statens prognose er overordnet beskrevet i notatet *Håndtering af COVID-19: Prognose og kapacitet i Danmark for intensiv
terapi* (findes i kopi her: [ITA_COVID_19_220320.pdf](ITA_COVID_19_220320.pdf), ellers 
henvises til litteraturlisten nedenfor).

### Angrebsraten 
Notatet nævner, at pandemier erfaringsmæssigt rammer 10-30% af befolkningen (*angrebsraten*) i første bølge, men så 
regner de kun efterfølgende på solskinsscenariet 10%. Sundhedsstyrelsen har tidligere meldt ud, at de regner med en 
*worst case* på 20% angrebsrate, men det scenarie behandles ikke, ej heller 30% scenariet, som der åbenbart er 
erfaring for er relevant.

Prognosen er baseret på erfaringer fra Kina (side 3, nederst). De officielle kinesiske tal tages således 
for pålydende.

### Opgaveformulering SIR-model
Vi genimplementerer modellen som kontrol af resultaterne i notatet, tester den mod de empiriske observationer
og beregner de manglende scenarier.

Modellen er i [ssi_prognose_2020_03_22.ipynb](ssi_prognose_2020_03_22.ipynb)
 
## Litteratur

- Sundhedsstyrelsens notat, *Håndtering af COVID-19: Prognose og kapacitet i Danmark for intensiv terapi* 
(22. marts 2020, Sagsnr. 4-0101-33) hentet fra [Statens Seruminstitut](https://www.sst.dk/-/media/Nyheder/2020/ITA_COVID_19_220320.ashx?la=da&hash=633349284353F4D8559B231CDA64169D327F1227)
på adressen https://www.sst.dk/-/media/Nyheder/2020/ITA_COVID_19_220320.ashx?la=da&hash=633349284353F4D8559B231CDA64169D327F1227


