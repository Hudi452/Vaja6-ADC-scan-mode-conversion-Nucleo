# Vaja6-ADC-scan-mode-conversion-Nucleo

PINOUT MIKROPROCESORJA:\
[pinout](https://github.com/Hudi452/Vaja6-ADC-scan-mode-conversion-Nucleo/blob/main/Pinout_mikroprocesorja.PNG)

ODGOVORI NA VPRAŠANJA:\
2.)\
c) Analogni vhodi:\
   IN1 - PC0,\
   IN2 - PC1,\
   IN3 - PC2\
Spadajo v skupino ADC1.\
e) Poleg pinov se izpiše ADC1_IN1, ADC1_IN2, ADC1_IN3.\
g) Clock prescaler nastavimo na 4.\
i) Privzeta nastavitev Number of Conversion je 1.\
j)  tvz = (tvz_cik + 12) / ftakta_pretvorbe = (92,5 + 12) / 1 MHz = 104,5 us\
k) Data Width: 1 bajt.\
3.)\
e) Kratica DMA pomeni Direct Memory Access. DMA nam omogoča neposreden dostop do pomnilnika, brez vmesnega posredovanja CPU-ja.

Komentar:\
Program deluje po pričakovanjih. S pomočjo programa STM Studio lahko hkrati opazujemo stanja vseh treh potenciometrov. ADC pretvorbe za vse 3 potenciometre se izvajajo ena za drugo na enem ADC-ju. To nam omogoča nastavitev Scan mode, ki spremlja stanja vseh treh potenciometrov in nastavitev Contionus Conversion, ki poskrbi, da se ADC pretvorbe izvajajo nemoteno.

