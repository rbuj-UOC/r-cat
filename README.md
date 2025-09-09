# UOC - Laboratori de Python i R

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/UOC%2Feimt%2Fdatascience%2FLAB%2Fr-cat/HEAD?urlpath=rstudio)

Aquest repositori conté materials educatius per al Laboratori de Python i R de la UOC (Universitat Oberta de Catalunya). El laboratori està estructurat com una col·lecció de scripts i notebooks de R organitzats per activitats que ensenyen progressivament conceptes de ciència de dades amb R.

## Accés Ràpid amb Binder

Feu clic al botó _launch binder_ de dalt per executar els notebooks del laboratori directament al navegador amb totes les dependències ja configurades.

L'entorn de [Binder](https://mybinder.org/) inclou:
- R 4.3 amb totes les llibreries necessàries preinstal·lades
- RStudio Server llest per usar
- Tots els conjunts de dades i materials del laboratori

## Estructura del Repositori

```
R/
├── A1/  # Instal·lació de programari R i introducció a RStudio
├── A2/  # Lectura i escriptura de fitxers de dades (CSV, Excel, JSON)
├── A3/  # Manipulació de dades amb tidyverse
├── A4/  # Tècniques de neteja de dades
├── A5/  # Estadística descriptiva
├── A6/  # Visualització de dades amb ggplot2
├── A7/  # Avaluació de models
└── A8/  # Exemple complet de flux de treball
```

## Configuració de l'Entorn de Desenvolupament

### Prerequisits
- R 4.0 o superior instal·lat al vostre sistema
- RStudio (recomanat)

### Configuració

1. **Descarregueu i instal·leu R:**
   - Visiteu https://cran.r-project.org/
   - Descarregueu la versió més recent per al vostre sistema operatiu

2. **Descarregueu i instal·leu RStudio:**
   - Visiteu https://posit.co/download/rstudio-desktop/
   - Descarregueu RStudio Desktop

3. **Obriu el projecte:**
   - Inicieu RStudio
   - Utilitzeu `File > Open Project` i navegueu fins al directori del projecte
   - O simplement obriu RStudio i configureu el directori de treball

4. **Instal·leu les llibreries necessàries:**
   ```r
   # Totes les dependències estan llistades a install.R
   source("install.R")
   ```

## Llibreries Principals

El curs utilitza les següents llibreries clau:

**Manipulació i anàlisi de dades:**
- **readr**, **readxl** - Lectura de fitxers de dades (CSV, Excel)
- **dplyr** - Manipulació de dades
- **data.table**, **plyr** - Processament de dades addicional
- **ggplot2**, **reshape2** - Visualització i transformació de dades

**Aprenentatge Automàtic:**
- **caret** - Framework principal d'aprenentatge automàtic
- **randomForest**, **rpart** - Algoritmes d'arbres
- **e1071**, **kernlab** - Support Vector Machines
- **xgboost** - Gradient boosting
- **C50**, **ipred** - Algoritmes addicionals de classificació
- **caretEnsemble** - Mètodes d'ensemble
- **pROC** - Avaluació de models
- **nnet** - Xarxes neuronals
- **mlbench** - Conjunts de dades de referència

**Documentació:**
- **rmarkdown** - Generació d'informes

## Començar

1. **Configureu l'entorn** seguint les instruccions anteriors

2. **Obriu RStudio** i navegueu fins al projecte

3. **Comenceu amb l'Activitat 1:**
   - Navegueu fins a `R/A1/` al panell de fitxers de RStudio
   - Obriu `instalacio-programari-r.R`
   - Executeu el codi línia per línia o tot el script

## Estructura de les Activitats

Cada carpeta d'activitat conté:
- Scripts principals de R (.R) amb exercicis i explicacions
- Carpeta `data/` amb conjunts de dades utilitzats en els exercicis
- Carpeta `images/` amb imatges i diagrames de suport
- Fitxers R Markdown (.Rmd) per a informes i documentació

## Activitats del Laboratori

- **A1:** Configuració de l'entorn amb R i RStudio, introducció als conceptes bàsics
- **A2:** Operacions d'E/S de fitxers (formats CSV, Excel, JSON)
- **A3:** Tècniques de manipulació de dades amb tidyverse
- **A4:** Neteja i preprocessament de dades
- **A5:** Anàlisi estadística i estadística descriptiva
- **A6:** Tècniques de visualització de dades amb ggplot2
- **A7:** Avaluació de models d'aprenentatge automàtic
- **A8:** Exemple de flux de treball complet de ciència de dades

## Resolució de Problemes

### Problemes comuns amb R
- **Errors de permisos:** Executeu RStudio com a administrador o configureu una biblioteca personal
- **Paquets no trobats:** Assegureu-vos que els repositoris CRAN estiguin configurats correctament
- **Errors d'instal·lació de paquets:** Proveu instal·lar des d'un mirror diferent de CRAN

### Problemes amb RStudio
- **Projecte no reconegut:** Configureu el directori de treball correcte amb `setwd()` o utilitzeu `Session > Set Working Directory`
- **Errors de codificació:** Configureu l'encoding a UTF-8 a `Tools > Global Options > Code > Saving`
- **R no detectat:** Verifiqueu que R estigui instal·lat i accessible des de `Tools > Global Options > R General`
