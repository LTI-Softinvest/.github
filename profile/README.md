## Rappel hiérarchie des projets

```
\dev
├── factuElectro
│   ├── libraries
│   │   ├── AdinvUtils
│   │   ├── CBuildPdf
│   │   ├── cycleVie
│   │   ├── FactureFV10
│   │   ├── FacturXReader
│   │   ├── FacturXSender
│   │   ├── FacturXWriter
│   │   ├── LifeCycleDecoder
│   │   ├── PAUtils
│   │   └── CodePassword
│   │
│   └── mains
│       ├── FacturX
│       └── GetPdfFromPA
│
├── libraries
│   ├── Hfcertifcs
│   ├── OracleUtils
│   ├── pathFiles
│   ├── SignLib
│   ├── SqlUtils
│   ├── stringExt
│   └── vive
│
├── Demat
└── FeTiers
```

## Script pour tout cloner

```bash
#!/usr/bin/env bash

# dans git bash
# chmod +x getall.sh
# ./getall.sh

SRC_PATH=https://github.com/LTI-Softinvest
DEST_PATH="C:/dev"

# mains
git clone $SRC_PATH/GetPdfFromPA "$DEST_PATH/factuElectro/mains/GetPdfFromPA"
git clone $SRC_PATH/FacturX "$DEST_PATH/factuElectro/mains/FacturX"
git clone $SRC_PATH/Demat  "$DEST_PATH/Demat"

# librairies (factuElectro)
git clone $SRC_PATH/AdinvUtils  "$DEST_PATH/factuElectro/libraries/AdinvUtils"
git clone $SRC_PATH/CBuildPdf  "$DEST_PATH/factuElectro/libraries/CBuildPdf"
git clone $SRC_PATH/cycleVie  "$DEST_PATH/factuElectro/libraries/cycleVie"
git clone $SRC_PATH/FactureFV10  "$DEST_PATH/factuElectro/libraries/FactureFV10"
git clone $SRC_PATH/FacturXReader  "$DEST_PATH/factuElectro/libraries/FacturXReader"
git clone $SRC_PATH/FacturXSender  "$DEST_PATH/factuElectro/libraries/FacturXSender"
git clone $SRC_PATH/FacturXWriter  "$DEST_PATH/factuElectro/libraries/FacturXWriter"
git clone $SRC_PATH/LifeCycleDecoder  "$DEST_PATH/factuElectro/libraries/LifeCycleDecoder"
git clone $SRC_PATH/PAUtils  "$DEST_PATH/factuElectro/libraries/PAUtils"

# librairies (globales)
git clone $SRC_PATH/Hfcertifcs  "$DEST_PATH/libraries/Hfcertifcs"
git clone $SRC_PATH/OracleUtils  "$DEST_PATH/libraries/OracleUtils"
git clone $SRC_PATH/pathFiles  "$DEST_PATH/libraries/pathFiles"
git clone $SRC_PATH/SignLib  "$DEST_PATH/libraries/SignLib"
git clone $SRC_PATH/SqlUtils  "$DEST_PATH/libraries/SqlUtils"
git clone $SRC_PATH/stringExt  "$DEST_PATH/libraries/stringExt"
git clone $SRC_PATH/vive  "$DEST_PATH/libraries/vive"
```
