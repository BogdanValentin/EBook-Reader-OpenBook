# Proiect - OpenBook

## Diagrama Bloc

![Diagrama Bloc](https://raw.githubusercontent.com/BogdanValentin/EBook-Reader-OpenBook/refs/heads/main/Images/TSC.png)  

## Pasii de implementare
Am realizat in primul rand schema electrica propusa pe OCW. Apoi am realizat board-ul avand grija prima data sa tai placa dupa dimensiunile precizate. Am pus componentele pe placa incercand sa urmez designul propus. Am pus cele 2 planuri de masa si am rutat firele. Am creat modelele 3D pt placa, baterie si ecran si le-am asamblat in produsul finit.

## Probleme & decizii luate
Senzorul BME688 nu se afla in biblioteca ci BME680 asa ca l-am folosit pe acela. Apar mai multe erori la conectarea firelor GND to GND, am inteles ca mai multi se confrunta cu aceasta problema asa ca am lasat asa. Mufa USB creaza o eroare Board Outline Clearance care, la fel, am inteles ca este una comuna.

## Bill of Materials (BOM)

| Componenta                           | Link de Achizitie           | Datasheet                                                  |
|--------------------------------------|--------------------------------------------|------------------------------------------------------------|
| **USB C connector**                  | [Link](https://ro.mouser.com/ProductDetail/GCT/USB4110-GF-A?qs=KUoIvG%2F9IlYiZvIXQjyJeA%3D%3D&utm_id=6470900573&utm_source=google&utm_medium=cpc&utm_marketing_tactic=emeacorp&gad_source=1&gclid=EAIaIQobChMIw8-8kMWjjAMVcheiAx1TPQ31EAAYAiAAEgLwovD_BwE)                 | [Datasheet](https://ro.mouser.com/datasheet/2/837/GCT_USB4110_Product_Drawing___20k_cycles-3455479.pdf)                                             |
| **ESD Protection**                   | [Link](https://ro.mouser.com/ProductDetail/STMicroelectronics/USBLC6-2SC6Y?qs=gNDSiZmRJS%2FOgDexvXkdow%3D%3D&utm_id=6470900573&utm_source=google&utm_medium=cpc&utm_marketing_tactic=emeacorp&gad_source=1&gclid=EAIaIQobChMI0PCv18SjjAMVl1qRBR1ivRIGEAAYASAAEgKdf_D_BwE)                   | [Datasheet](https://ro.mouser.com/datasheet/2/389/usblc6_2sc6y-1852505.pdf)                                             |
| **LDO Voltage Regulator**            | [Link](https://ro.mouser.com/ProductDetail/Torex-Semiconductor/XC6220A331MR-G?qs=AsjdqWjXhJ8ZSWznL1J0gg%3D%3D&utm_id=6470900573&utm_source=google&utm_medium=cpc&utm_marketing_tactic=emeacorp&gad_source=1&gclid=EAIaIQobChMIyO-xwcSjjAMVwxeiAx0qMg1NEAAYASAAEgLqI_D_BwE)                   | [Datasheet](https://ro.mouser.com/datasheet/2/760/xc6220-3371556.pdf)                                             |
| **SD Card**                          | [Link](https://store.comet.srl.ro/Catalogue/Product/43497/?mark=2)                   | [Datasheet](https://www.attend.com.tw/data/download/file/112A-TAAR-R03.rar)                                             |
| **ESP32 C6**                         | [Link](https://ro.mouser.com/ProductDetail/Espressif-Systems/ESP32-C6?qs=Imq1NPwxi75noDtUpuVuWw%3D%3D&srsltid=AfmBOopGsscg6owTrNYpzSD_A6PeAhrd-8P7Q2gDTU-QmgxBLIUltlA7)                   | [Datasheet](https://ro.mouser.com/datasheet/2/891/esp32_c6_datasheet_en-3304070.pdf)                                             |
| **Li-Po Battery Charging Controller**| [Link](https://ro.mouser.com/ProductDetail/Microchip-Technology/MCP73831-2ATI-MC?qs=hH%252BOa0VZEiCb32ZvHkqhBQ%3D%3D&utm_id=20109199409&utm_source=google&utm_medium=cpc&utm_marketing_tactic=emeacorp&gad_source=1&gclid=EAIaIQobChMIwvChgMajjAMVxRCiAx3PNB47EAAYASAAEgIkZPD_BwE)                   | [Datasheet](https://ro.mouser.com/datasheet/2/268/MCP73831_Family_Data_Sheet_DS20001984H-3441711.pdf)                                             |                                            |
| **E-Paper Drive Circuit**            | [Link](https://ro.mouser.com/ProductDetail/Vishay-Semiconductors/SI1308EDL-T1-GE3?qs=bX1%252BNvsK%2FBramh9tgpOaEw%3D%3D&srsltid=AfmBOop7VB2nsZ4y3AQijBvo753QWrx9w51296dR8UjRlpwp_qg7iivF)                   | [Datasheet](https://www.vishay.com/doc?63399)                                             |
| **E-Paper Display Header**           | [Link](https://ro.mouser.com/ProductDetail/Hirose-Connector/FH34SRJ-24S-0.5SH99?qs=vcbW%252B4%252BSTIpKBl5ap9J8Fw%3D%3D)                   | [Datasheet](https://ro.mouser.com/datasheet/2/185/FH34SRJ_24S_0_5SH_99__CL0580_1255_6_99_2DDrawing_0-1615044.pdf)                                             |
| **EPD Power**                        | [Link](https://ro.mouser.com/ProductDetail/Diodes-Incorporated/DMG2305UX-7?qs=L1DZKBg7t5F%2FNBHrjfxC%252Bg%3D%3D)                   | [Datasheet](https://www.diodes.com/assets/Datasheets/DMG2305UX.pdf)                                             |
| **Environmental Sensor BME688**      | [Link](https://ro.mouser.com/ProductDetail/Bosch-Sensortec/BME688?qs=IS%252B4QmGtzzqQoVDscqwx3A%3D%3D)                   | [Datasheet](https://ro.mouser.com/datasheet/2/783/bst_bme688_fl000-2307034.pdf)                                             |
| **Voltage Supervisor**               | [Link](https://ro.mouser.com/ProductDetail/ROHM-Semiconductor/BD5229G-TR?qs=4kLU8WoGk0vvnhrrYwdszw%3D%3D&srsltid=AfmBOoohF8UhLJmEpguPyHuoa_qfrAg1xACnmLecyTKeAsNQaT9m0ZF5)                   | [Datasheet](https://fscdn.rohm.com/en/products/databook/datasheet/ic/power/voltage_detector/bd52xxg-e.pdf)                                             |
| **Battery Charge Level**             | [Link](https://ro.mouser.com/ProductDetail/Analog-Devices-Maxim-Integrated/MAX17048G+T10?qs=D7PJwyCwLAoGnnn8jEPRBQ%3D%3D&srsltid=AfmBOooZpxDFB0Ef_1d_Z6ZaAY3DUJrF2tjhVNvrkbPhjCJpjsk7k4Qx)                   | [Datasheet](https://ro.mouser.com/datasheet/2/609/MAX17048_MAX17049-3469099.pdf)                                             |
| **RTC Module DS3231SN**              | [Link](https://ro.mouser.com/ProductDetail/Analog-Devices-Maxim-Integrated/DS3231SNTR?qs=1eQvB6Dk1vhN%252BEOl3KU%252Bjw%3D%3D)                   | [Datasheet](https://ro.mouser.com/datasheet/2/609/DS3231-3421123.pdf)                                             |                                            |                                            |
| **SPI ESD Protection Lines**         | [Link](https://ro.mouser.com/ProductDetail/Littelfuse/PGB1010603MR?qs=gu7KAQ731URLg4GSnNNN7Q%3D%3D)                   | [Datasheet](https://www.littelfuse.com/assetdocs/pulseguard-esd-suppressors-pgb1-datasheet?assetguid=8a337998-d54d-466b-be4e-dc5bcd1f9321)                                             |
| **External NORFlash 64MB**           | [Link](https://ro.mouser.com/ProductDetail/Winbond/W25Q512JVEIQ?qs=l7cgNqFNU1jw6svr3at6tA%3D%3D&srsltid=AfmBOooYdTG4zpB4g9XFVQog2As1CX3DBItEO5x_Lv8uh1fPEpwC9MRH)                   | [Datasheet](https://ro.mouser.com/datasheet/2/949/Winbond_W25Q512JV_Datasheet-3240039.pdf)                                             |

---

## 3. Descrierea Functionalitatii Hardware

## Componente Folosite:

1. **USB C connector & ESD protection**  
2. **LDO Voltage Regulator**  
3. **SD card**  
4. **ESP32 C6**  
5. **Li-Po Battery Charging Controller**  
6. **Display Type Selector**  
7. **E-Paper Drive Circuit**  
8. **E-Paper Display Header**  
9. **EPD Power**  
10. **Environmental Sensor BME688**  
11. **Voltage Supervisor + Reset & Boot/IO Button**  
12. **Battery ChargeLevel**  
13. **RTC Module DS3231SN**  
14. **Qwiic/Stemma QT**  
15. **Test Pads**  
16. **SPI ESD Protection Lines**  
17. **External NORFlash 64MB**

---

## 4. ESP32-C6 Pini

| Componenta                          | Pini ESP32       | Rol     |
|-------------------------------------|---------------------|-------------|
| **E-Paper Display**                 | SPI (MISO, MOSI, CLK, CS) | Afisare |
| **BME688**                          | I2C (SDA, SCL)      | Senzor multirol |
| **RTC DS3231SN**                    | I2C (SDA, SCL)      | Ceas / Temporizare  |
| **Li-Po Battery Controller**        | GPIO  | incarcare   |
| **SD Card**                         | SPI (MISO, MOSI, CLK, CS) | Stocare date |
| **Qwiic/Stemma QT**                 | I2C                  | -  |

---
