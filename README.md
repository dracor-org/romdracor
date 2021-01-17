# RomDraCor
Roman Drama Corpus, **36 plays** in [TEI P5](https://tei-c.org/guidelines/p5/) format, adapted from [Perseus Digital Library](http://www.perseus.tufts.edu/hopper/opensource/download), first converted to DraCor format in June 2019. Licensed under [CC BY-SA 3.0 US](https://creativecommons.org/licenses/by-sa/3.0/us/).

The corpus was enhanced and is maintained by Julia Jennifer Beine (Ruhr University Bochum), Frank Fischer and Boris Orekhov (both Higher School of Economics, Moscow). For a list of changes please see below.

Content: 20 comedies by **Plautus**, 6 comedies by **Terence**, 10 tragedies by **Seneca**.

Frontend: https://dracor.org/rom

## Scans of the editions on which Perseus Digital Library based their digitisation:

* Plauti Comoediae. Recensuit et emendavit Fridericus Leo.
  * [Volumen prius. Berlin: Weidmann 1895.](https://archive.org/details/comoediaerecensu01plauuoft)
    * Amphitruo. Asinaria. Aulularia. Bacchides. Captivi. Casina. Cistellaria. Curculio. Epidicus. Menaechmi. Mercator.
  * [Volumen alterum. Berlin: Weidmann 1896.](https://archive.org/details/comoediaerecens00plaugoog)
    * Miles Gloriosus. Mostellaria. Persa. Poenulus. Pseudolus. Rudens. Stichus. Trinummus. Truculentus. <s>Vidularia.</s> <s>Fragmenta.</s>

* [Publii Terentii Comoediae sex. With a commentary by the rev. E. St. John Parry, M.A. London. Whittaker and Co. 1857.](https://archive.org/details/comoediaesexwith00tereuoft)
  * Andria. Eunuchus. Heautontimorumenos. Adelphi. Hecyra. Phormio.

* [L. Annaei Senecae Tragoediae. Recensuerunt Rudolfus Peiper et Gustavus Richter. Leipzig: Teubner 1921.](https://archive.org/details/tragoediaerecens00seneuoft)
  * Hercules Furens. Troades. Phoenissae. Medea. Phaedra. Oedipus. Agamemno. Thyestes. Hercules Oetaeus. Octavia.

## Changelog
### 25.06.2019
* Import of 36 plays.
* Adjust filenames (e.g., "pl.am_lat.xml" → "plautus-amphitruo.xml").
* ```xmllint --format --encode UTF-8```

### 26.06.2019
* Add DraCor ID to ```publicationStmt```.
* Add Wikidata IDs for authors and plays.
* Add licence information.
* Add ```who``` attributes to ```<sp>```.
* Add ```<particDesc>```.

### 09.12.2019
* Add gender information.

### 10.12.2019
* Add ```xml:lang="lat"``` to root element.

### 15.06.–12.08.2020
* Major correction of character IDs.

### 16.07.2020
* Add written act/scene indicators for Plautus following Leo's edition.

### 24.07.2020
* Reduce ```<div1>``` and ```<div2>``` to ```<div>```.

### 29.07.2020
* Add "written" and "premiere" dates if available.

### 14.08.2020
* Add bibliographic record for each play.

### 18.08.–09.09.2020
* Add act segmentation for Seneca following Fitch 2018.

### 02.09.2020
* Add page numbers for Terence.
* Add written act/scene indicators for Terence.

### 17.01.2021
* Recode author information. ([commit](https://github.com/dracor-org/romdracor/commit/5ff2a2fedf1abbf5afa1f3fd8cd2fab93ef0f555))

## Known issues
* V/U incongruencies between different authors: especially for contrastive analyses, the different handling by the editors has to be taken into account (e.g., "ut" vs. "vt"; "ubi" vs. "vbi").
