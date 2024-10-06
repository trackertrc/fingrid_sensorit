# fingrid_sensorit
Fingrid restfull api sensorit Home Assistantille

Tämä on osittain paranneltu versio tästä joka käyttää vanhaa api rajapintaa https://github.com/MarcoHyvonen/fingrid_json_app

Kaikki tällähetkellä saatavilla olevat API tiedot fingridiltä lisätty.

Käytössä uusi API data.fingrid.fi
API keyn voi luoda ilmaiseksi fingridin www sivustolla.

luo tiedosto secrets.yaml (jos ei ole) lisää sinne kohta:
fingrid_new_key: omaapikeysi

lisäksi lisää configuration.yaml tiedostoon kohta:
homeassistant:
  packages: 
    pack_1: !include fingrid_sensorit.yaml

lisäksi kopioi fingrid_sensorit.yaml tästä reposta /config kansioon homeassistantissa (sama kansio jossa on configuration.yaml)

Tämä luo Fingridin sähköjärjestelmän sensorit ja kuvaajan.

Bonuksena myös shf sensorit.

lisää configuration.yaml:

homeassistant:
  packages: 
    pack_1: !include fingrid_sensorit.yaml
    pack_2: !include spot-price.yaml

Tämä luo shf sensorit pörssisähköohjausta varten.

graafiikka malleja repossa.


gr
