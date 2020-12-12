# Descripció

Aquest dipòsit conté els fitxers i instruccions necessaris per a alliberar i configurar les aspiradores de Xiaomi en català.

# Dispositius compatibles

 * 1a generació: Rockrobo V1
 * 2a generació: Roborock S5/S50/S51/S55

Els dispositius més recents (S5-Max, S6, 1S, etc.) **NO** són compatibles.

# Alliberament del dispositiu

*PENDENT*

# Veu en català

Per a configurar la veu de l'aspiradora en català, hi ha dues opcions: utilitzar una veu sintetitzada o crear un paquet de veu personalitzat.

## Veu sintetitzada

[Aquí](https://github.com/MarcRiera/roborock-catala/releases) teniu dos paquets de veu sintetitzada en català, gràcies al projecte [FestCat](http://festcat.talp.cat/). Baixeu el fitxer corresponent en funció de si voleu la veu de l'Ona (`ca_festival_ona.pkg`) o la d'en Pau (`ca_festival_pau.pkg`).

Els fitxers de so originals estan disponibles a la carpeta `audio` d'aquest dipòsit.

## Paquet de veu personalitzat

Podeu crear un paquet de veu a partir d'una carpeta que contingui els fitxers `.wav` que ha de reproduir l'aspiradora. Podeu trobar el nom dels fitxers i el text estàndard en català [aquí](https://github.com/dgiese/dustcloud/blob/master/devices/xiaomi.vacuum/audio_generator/language/audio_ca.csv).

Amb l'ordre següent es pot generar el fitxer `.pkg` que posteriorment instal·lareu en el dispositiu (requereix `tar` i `ccrypt`):

```
cd <carpeta amb els fitxers .wav> && tar zc *.wav | ccrypt -e -K "r0ckrobo#23456" > <nom del paquet>.pkg
```

## Instal·lació

*PENDENT*
