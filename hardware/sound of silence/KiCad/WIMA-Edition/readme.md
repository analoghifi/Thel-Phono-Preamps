### This special edition exclusively uses the highly valued WIMA polypropylene capacitors throughout  
(FKP = highest quality film/foil types for the passive RIAA filter and the input (load-) Capacitors)  
* C101,C102,C201..C214 = WIMA FKP2 33nF 63V 1% (tanδ = 0.0005)  
* C3,C4,C6 = WIMA FKP2 100V 1% (tanδ = 0.0005)
* C5,C7 = WIMA FKP2 47pF 1000V 2.5% (tanδ = 0.0005)
* C8,C9,C12,C13,C14,C15 = WIMA MKP2 63V 5% (tanδ = 0.0005)  
  
see -> [List of used capacitors for the "WIMA-Edition"](https://github.com/analoghifi/Thel-Phono-Preamps/blob/main/hardware/sound%20of%20silence/KiCad/WIMA-Edition/Capacitor_BOM.md)  
  
#### this is not the original Thel PCB but it's very like\* the original with the following exceptions:  
* different board dimensions original: 155mm x 60mm -> this PCB: 155mm x 64mm  
* different mounting hole spacing original: 148mm x 53mm -> this PCB: 148mm x 57mm  
* "C2" is 462nF (paralleled 14x33nF Wima FKP2 1%) 
* "C1" is 66nF (paralleled 2x33nF Wima FKP2 1%)
* "C1" is in a different location on the board  
* using WIMA FKP2 (instead of ceramics) for the input (load-) Capacitors as well C3 ..C7  
* more massive ground and power supply PCB tracks  
* additional GND track unterneath U1 and U2 
  
\*(same schematic / same 1-layer\** layout THT / same THT components in the same places on the board)  
\**(strictly speaking, this KiCad PCB is a two-layer PCB with plated-through holes, but you can also (let) produce it as a classic 1-layer PCB with non-plated holes if you wish, since all the tracks are on the bottom side only)  

----  

### remarks:  
#### R6,R7:  
one can use 23,7kΩ or 24kΩ instead  
or use 2x47kΩ in parallel each  
when using MM-Systems (choosing R<sub>in</sub> = 47kΩ [SW2=0]):  
for lower noise one may use low-TCR-types (25ppm/°C or lower) if available  
e.g. Vishay "[CMF Industrial](https://www.mouser.com/c/passive-components/resistors/film-resistors/metal-film-resistors-through-hole/?m=Vishay&series=CMF%20Industrial)" series  
or Vishay [PTF series](https://www.mouser.de/c/passive-components/resistors/film-resistors/metal-film-resistors-through-hole/?m=Vishay&series=PTF) (even lower TCR)  
or Tyco (TE Connectivity) type "[YR1B23k7CC](https://www.mouser.com/ProductDetail/TE-Connectivity-Holsworthy/YR1B23K7CC?qs=n4i9pByFsMSkJXItUSDcPw%3D%3D)" (23.7kΩ / 0.1% / 15ppm/°C) [from the Tyco ["YR1-series" (R-series)](https://www.mouser.com/c/passive-components/resistors/film-resistors/metal-film-resistors-through-hole/?m=TE%20Connectivity&series=R)]  
#### U1,U2,U3,U4,U5:  
instead of [LME49720](https://www2.mouser.com/ProductDetail/Texas-Instruments/LME49720NA-NOPB?qs=7lkVKPoqpbYtIqwyg5iDaA%3D%3D) you can use [LM4562](https://www2.mouser.com/ProductDetail/Texas-Instruments/LM4562NA-NOPB?qs=QbsRYf82W3Gc2w4DLq%252BZjw%3D%3D) (both Texas Instruments),  
these two are 100% identical (even regarding their inner guts).
  
----  
  
these are KiCad 6.x projects  
see how to get the proper 3D-Models from here: https://github.com/analoghifi/KiCad-3D-Models
  
----  
  
use kicanvas.org to view this KiCad project in your browser:  
https://kicanvas.org/?github=https%3A%2F%2Fgithub.com%2Fanaloghifi%2FThel-Phono-Preamps%2Ftree%2Fmain%2Fhardware%2Fsound%2520of%2520silence%2FKiCad%2FWIMA-Edition
