# K1SS Components — KiCad Library

Symboles et footprints pour les projets hardware K1SS.

## Symboles disponibles

| Composant | Description | Statut |
|-----------|-------------|--------|
| **STM32MP257** | Dual Cortex-A35 + M33, GPU, NPU | ✅ 130 broches |
| **CS42448** | Audio CODEC 6ADC/8DAC | 🚧 En cours |
| **BQ25890** | Chargeur Li-ion I²C + Power Path | 🚧 En cours |

## Symboles > STM32MP257

130 broches organisées par fonction :

- **Gauche** (35) : Alimentation (VDD/VSS), Boot, JTAG, Horloges
- **Droite** (34) : DDR LPDDR4 (DQ0-15, DQS, CA, contrôle)
- **Haut** (22) : eMMC/SDMMC, USB×2, Ethernet RGMII
- **Bas** (39) : Audio SAI/I²S, I²C×2, SPI, UART, GPIO PA/PB/PC

Format : KiCad 10.0+ (version 20241209)
Licence : CERN-OHL-W-2.0

## Utilisation

1. Ajouter le fichier `.kicad_sym` dans vos librairies :
   - Préférences → Gérer les librairies de symboles
   - Ajouter : `Symbols/STM32MP257.kicad_sym`
2. Touche A → chercher le composant
3. Placer sur le schéma

## Contribuer

Pull requests bienvenues. Conventions :
- Pas de demi-grille (toujours en pas de 2.54mm)
- Broches groupées par fonction
- Noms explicites
