# Suomenkielinen oikoluku Linuxilla
## Suomeksi saatavilla olevat oikolukijat

Suomeksi on saatavilla neljä avoimen lähdekoodin oikolukuohjelmistoa. Voikko on näistä tunnetuin ja monipuolisin. Aspell on vanhanaikainen ja kehitetty ensisijaisesti fusionaalisiin kieliin eikä siksi sovellu suomen kaltaisiin agglutinoiviin kieliin. Hunspell ja Nuspell ovat Aspellia merkittävästi uudempia ja voivat olla tyydyttävä ratkaisu suomen kieleen, kun sanakirja on laadukas. Nuspellin kehityksessä on erityisesti huomioitu morfologisesti rikkaat kielet.

| Moottori  | Suositeltu sanakirja | Kielioppi |
|-----------|---------------------|-----------------|
| **Voikko** (libvoikko) | voikko‑fi 2.5 | Kyllä |
| **Hunspell** | hunspell‑fi 0.2 | Ei |
| **Nuspell** | hunspell‑fi 0.2 (yhteensopiva) | Ei |
| **Aspell** | aspell6‑fi‑0.7 (vanhentunut) | Ei |


### Voikko
Voikko on natiivi suomenkielinen oikoluku- ja tavutusohjelmisto, joka tukee myös kieliopin tarkistusta. Tämä on suomenkielen oikolukijoista ylivoimaisesti paras ja monipuolisin, sillä se käyttää morfologista analyysiä ja sisältää perussääntöihin perustuvan kielioppitarkistimen. Se on käytettävissä lukuisissa KDE-ohjelmissa ja avoimen lähdekoodin toimisto-ohjelmistoissa, kuten LibreOfficessa.

```bash
sudo apt install libvoikko1 voikko-fi libreoffice-voikko libenchant-2-voikko
```

#### LibreOffice
Debian-pohjaisissa jakeluissa Voikko asennetaan LibreOfficeen tyypillisesti suoraan pakettivarastosta:
```bash
sudo apt install libreoffice-voikko
```

#### KDE
Monissa KDE/Qt-sovelluksissa suomen kielen oikoluku toimii automaattisesti, kun kieli on valittu asetuksista. Oletuksena KDE:n ohjelmat käyttävät Sonnet-sovelluskehystä. Se voi kommunikoida suoraan Voikon kanssa, kuten Fedoran tapauksessa, tai Enchant-lisäosan avulla GNOME/GTK:n Enchant-sovelluskehyksen kanssa, joka puolestaan käyttää Voikkoa.

Fedorassa tämä näyttää seuraavalta:

`KDE‑sovellus → Sonnet → kf6‑sonnet‑voikko → Voikko`

Kubuntulla tämä näyttää seuraavalta: 

`KDE-sovellus → Sonnet → Enchant → libenchant-2-voikko → Voikko`

#### GNOME
Monissa GNOME/GTK-sovelluksissa suomen kielen oikoluku toimii automaattisesti, kun kieli on valittu asetuksista. Oletuksena GNOMEN ohjelmat käyttävät Enchant-sovelluskehystä, joka käyttää suoraan Voikko-implementaatiota.

`GTK-sovellus  → Enchant → libenchant-2-voikko → Voikko`

#### Sonnet ja Enchant
Sonnet- ja Enchant-sovelluskehykset eivät ole oikolukijoita itsessään vaan ne ovat edusta usealle eri oikolukijalle. Näiden sovelluskehysten avulla sovelluskehittäjien on helppo integroida oikolukutoiminnot Qt- ja GTK-pohjaisiin graafisiin käyttöliittymiin. Sonnet ja Enchant voivat käyttää taustajärjestelminään esimerkiksi Aspelliä, Hunspelliä ja Voikkoa. Lisäksi Sonnet voi käyttää Enchantia välikappaleena oikolukijoihin, joista on jo toteutus Enchantille.

#### Emacs
Voikkoa voidaan käyttää Emacs-tekstinkäsittelyohjelmassa `tmispell-voikko`-paketin avulla. Paketti voidaan asentaa Debian-pohjaisten käyttöjärjestelmien pakettivarastosta. Lisätietoja on paketin [Github-sivulla](https://github.com/voikko/tmispell).

### Aspell
Aspell-oikolukijan suomenkielistä sanakirjaa ei ole saatavilla Debianin ja sen siihen pohjautuvien käyttöjärjestelmien pakettivarastoissa. Se voidaan asentaa seuraavalla tavalla järjestelmän laajuisesti:
```bash
sudo apt install aspell

wget https://ftp.gnu.org/gnu/aspell/dict/fi/aspell6-fi-0.7-0.tar.bz2
tar xjf aspell6-fi-0.7-0.tar.bz2
cd aspell-fi-0.7-0
./configure
make
sudo make install
```

### Hunspell
Hunspell ei julkaise virallisesti suomenkielistä sanakirjaa. Se voidaan kuitenkin asentaa Linuxille käyttäen kieliteknologian tutkija Filip Ginterin kehittämää [Hunspell-fi](https://github.com/fginter/hunspell-fi)-sanakirjaa:
```bash
sudo apt install hunspell
wget https://github.com/fginter/hunspell-fi/releases/download/0.2/fi-spell-0.2.xpi
unzip fi-spell-0.2.xpi
sudo cp dictionaries/fi_FI/fi_FI.* /usr/share/hunspell/
```

#### Firefox
Firefox käyttää oikolukuun Hunspell-taustajärjestelmää. Filip Ginterin kehittämä Hunspell-fi-sanakirja voidaan manuaalisesti asentaa Firefoxiin avaamalla `fi-spell-0.2.xpi`-tiedosto Firefoxissa. Tiedosto on saatavilla [hunspell-fi:n Github-sivulla](https://github.com/fginter/hunspell-fi/releases/tag/0.2).

### Nuspell
Nuspell voidaan asentaa Debian-pohjaisten käyttöjärjestelmien pakettivarastosta

`sudo apt install nuspell`

Sen kanssa voidaan käyttää samoja sanakirjoja kuin Hunspellin.
