# COVID-19-situationen i Danmark

**COVID-19 situationen i Danmark. Dagsaktuelle data og prognoser uden *spin* og skønmaleri.,**

Vi modellerer og visualiserer scenarier omkring COVID-19 i Danmark for at formidle 
og synliggøre situationen og afvejelserne ved forskellige mulige løsninger.

# De essentielle spørgsmål
En leders opgave er at stille de rigtige spørgsmål.

De centrale spørgsmål i situationen er:

1) Hvor er vi nu? (**situationen**: data)
2) Hvor stort bliver **behovet** for behandling (prognose)
3) Hvor stor **overskudskapacitet** har vi til at behandle COVID-19 patienterne og samtidig behandle de "normale" 
patienter? (virkemidler under samfundets kontrol)
4) Hvor hurtigt og hvordan kan vi **øge kapaciteten**? 
5) Hvor meget kan vi **reducere behandlingsbehovet** (udgangsforbud mv.)
6) Hvilke **scenarier** er der (ud over "solskinsscenariet"), og hvilke tiltag skal vi sætte i værk i dag for at være 
beredt hvis noget går galt?

Og endelig:

- Hvordan kommer vi foran bolden, så vi kan handle oplyst ud fra en overordnet plan og vision 
for alle relevante scenarier?

Når man reflekterer over denne ramme, er der rig inspiration til at formulere og teste hypoteser og scenarier.

Må det blive til inspiration og nytte!

# Indhold

## Forbedrede COVID-19 prognoser

Her modellerer vi epidemikurven, og undersøger hvordan det kan gå, og hvad der kan ske, og hvad vi kan gøre.

Vi genimplementerer Sundhedsstyrelsens og Statens Seruminstituts modelberegning som frit tilgængelig 
kode til *peer review*.

Se [prognoser](prognoser/README.md) mappen.

# Vi har brug for din hjælp
Du kan hjælpe med. For eksempel ved:
- *kontrol* og *kritik* af modellen
- *replikering* af modelberegningerne for at sikre, at de er korrekt og fyldestgørende   
- *opstille nye spørgsmål og hypoteser* 
- bedre *visualisering af data* 

# Hvorfor?

Alle må hjælpe hvor de kan. 

Fordelene ved dette konkrete projekt er:

- Det giver **bedre information** da vi modsat Sundhedsstyrelsen kan levere **dagsaktuelle prognoser**.  
- Det skaber **transparens** omkring situationen og beslutningsgrundlaget for den nærmeste fremtid.
- Det skaber **tryghed**, når myndighedernes beslutningsgrundlag er åbent og udsat for _peer review_.
- Det er **rettidig omhu** at vi som borgere er beredte og hjælper til i tide, inden situationen rammer os og vi stadig 
har manøvrerum.
- Det kan hjælpe med bedre at **formidle situationen og løsningsmulighederne** til befolkningen.
- Det er **interessant** matematisk modellering.

# Hvem står bag

Projektet er startet af Martin Jul, inspireret af Morten Gram Pedersen og Matteo Meneghinis gode arbejde 
med at kvantificere COVID-19 i Italien. 
Se deres preprint, 
[*Quantifying undetected COVID-19 cases and effects of containment measures in Italy*](https://www.researchgate.net/publication/339915690_Quantifying_undetected_COVID-19_cases_and_effects_of_containment_measures_in_Italy).

## Bidragydere:

TODO

# Hjælp os

## Udvikling
Kom i gang med at arbejde med dine egne modeller

### Brug af Anaconda (anbefales til Windows)
Installer 
* [Anaconda Scientific Python](https://anaconda.org/)
* [Jupyter notebooks](https://jupyter.org/). 

se [`environment.yml`](environment.yml) for det præcise miljø.

Miljøet kan etableres således:

    conda env create -f environment.yml


### Standard Python
Opsætning af milnjø:
```shell script
python3 -mvenv venv
. venv/bin/activate
pip install -r requirements.txt
``` 

Udvikling med Jupyter:
```shell script
jupyter notebook
```

# Kontaktinformationer

Martin Jul, se [www.mjul.com](http://www.mjul.com)

# Teknisk information

Modellerne er bygget med Python 3 med de gængse databehandlingsværktøjer 
NumPy, Pandas, SciPy, Matplotlib, Seaborn, Jupyter osv.

 
