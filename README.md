# Vaja 6 – Več kanalna (scan mode) ADC pretvorba z Nucleo-L476RG

## Cilj naloge

S pomočjo programskega okolja STM32CubeIDE in HAL knjižnicami sprogramirajte mikroprocesor tako, da bo izvajal ADC pretvorbe na več kanalnih sočasno v scan mode način. Vrednosti treh zunanjih potenciometrov boste zajemali preko Nuclea-L476RG in jih prikazovali na STM Studio.

## Postopek inicializacije periferije

- pini za vhode so **PC0** , **PC1** , **PC2**.  
- Poleg pinov se izpiše **ADC1_IN1,2,3**.  
- Izbrana Vrednost parametra je **4**.  
- Privzeta vrednost *Number of Conversio* je **1**.  
- **tvz** = 6,35μs 
- **DMA** = Direct memory access (Direkten dostop spomina).
  



## Pinout
[Pinout](media/Screenshot_20221025_105007.png)

## Slika Vezja
[SlikaVezja]
