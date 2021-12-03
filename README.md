# Vaja7-PWM-STM32F

Vprašanja na odgovore:

 Kateri pin ste omogočili? 
   Pin PE9. 
   Kaj se izpiše poleg pina?
   TIM_CH1.
   
 Koliko je vrednost Perscaler (namig; delitelj)?
   16.
 Parameter Counter Period nastavimo na 100 in s tem še dodatno znižamo takt časovnika. Koliko znaša sedaj?
   10kHz.

 V PWM Generation Channel nastavite Pulse (16 bits value) na 50. Kaj pomeni ta parameter?
   Širina signala (duty cycle).

Poiščite prenastavljeni parameter Pulse (ki je 50) v vaši kodi in prepišite ukaz, ki ga je generiral CubeMX: sConfigOC.Pulse = 50;.
V kodi spremenite vrednost širine pulza na 25 %. Zapišite popravljeni ukaz v kodi: sConfigOC.Pulse = 25;. Zapišite kaj počnejo ukazi
v 1. 2. in 3. vrstici (v user code begin 3):

  Ukaz 1 : Nastavi spremenljivko duty cycle.
  Ukaz 2 : Spremeljivki prišteje 10.
  Ukaz 3 : Če ima spremenljivka duty cycle vrednost ki je večja od 90, nastavi spremenljivko na 10.

Komentar: 
  Imela sva nekaj težav pri nastavitvi parametrov in s kodo, pri vezavi osciloskopa pa nisva imela večjih težav.
  Naloga se nama je zdela zanimiva in drugačna od prejšnjih.
