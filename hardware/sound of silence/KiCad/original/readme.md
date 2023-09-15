this is not the original Thel PCB but it's very like\* the original with the following exceptions:  
* different board dimensions original: 155mm x 60mm -> this PCB: 155mm x 69.65mm  
* different mounting hole spacing original: 148mm x 53mm -> this PCB: 148mm x 62mm  
* make use of my \"universal capacitor footprint\" for the filter caps (C1,C21,C22,C23,C24,C25,C26,C27) -> see here T.B.D.  
* C1 is in a different location on the board  
* using a combined 5.0mm/7.5mm pin spacing footprint for all other small (foil and ceramic) caps (C3,C4,C5,C6,C7,C8,C9,C10,C11,C14,C15)  
* more massive ground and power supply PCB tracks  
* additional GND track unterneath U1 and U2 
  
\*(same schematic / same 1-layer\** layout THT / same THT components in the same places on the board)  
\**(strictly speaking, this KiCad PCB is a two-layer PCB with plated-through holes, but you can also (let) produce it as a classic 1-layer PCB with non-plated holes if you wish, since all the tracks are on the bottom side only)  

----  

### remarks:  
#### C3,C4,C5,C6,C7:  
use ceramic C0G capacitors (tolerance: 1% to 2,5% / rated DC Voltage: 50V, 63V or 100V / PCM 5mm or 7,5mm)  
e.g. KEMET "[goldmax 300](https://github.com/analoghifi/capacitors/blob/main/audio%20and%20filter%20capacitors/docs/datasheets/C0G/KEMET_C1049_GOLDMAX_C0G_THT.pdf)" Series in THT version  
or alternatively if you don't like ceramic capacitors:  
small polypropylene Film/Foil Capacitors (tolerance: 1% to 2,5% / rated DC Voltage: 63V or 100V / PCM 5mm or 7,5mm)  
e.g. KEMET [PFR-("Evox")](https://github.com/analoghifi/capacitors/blob/main/audio%20and%20filter%20capacitors/docs/datasheets/kp/KEMET_PFR_Serie_KP.pdf)-Series  
or WIMA [FKP2-Series](https://github.com/analoghifi/capacitors/blob/main/audio%20and%20filter%20capacitors/docs/datasheets/kp/WIMA_FKP_2__NEW_ROHS__EN.pdf) (not FKP**0**2)  
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
these two are 100% identical.
  
----  
  
these are KiCad 6.x projects  
see how to get the proper 3D-Models from here: https://github.com/analoghifi/KiCad-3D-Models
  
----  
  
use kicanvas.org to view this KiCad project in your browser:  
https://kicanvas.org/?github=https%3A%2F%2Fgithub.com%2Fanaloghifi%2FThel-Phono-Preamps%2Ftree%2Fmain%2Fhardware%2Fsound%2520of%2520silence%2FKiCad%2Foriginal
