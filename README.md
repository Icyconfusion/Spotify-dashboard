# Spotify-dashboard
A display with buttons and an encoder for showing spotify tracks and controlling things like volume.

The project is based on an ESP32 with an ST7735 TFT LCD. I made this project because its a cool way to control music, but also to learn about spi and display control.
<img width="810" height="598" alt="image" src="https://github.com/user-attachments/assets/76fb007c-bee8-4ae9-8c32-edf821f77c9f" />
<img width="812" height="549" alt="image" src="https://github.com/user-attachments/assets/a7512c3e-2fb2-4e51-b5c6-bc0b4b1feaa6" />

# CAD

The CAD is pretty simple, its basically just two parts that click together using a small lip on the back cover. The front cover has a cutout for the screen, keys and encoder, as well as a notch to hold the esp32 in place. The back cover has a cutout for power.
<img width="909" height="662" alt="image" src="https://github.com/user-attachments/assets/2ccf7bc1-a4d1-48fe-a5e1-fe123c198a2e" />

<img width="916" height="605" alt="image" src="https://github.com/user-attachments/assets/8112ca2e-7230-4dad-946e-956815eb4c3f" />

# Electronics
The wiring requires the TFT to be connected via SPI. The pushbuttons and encoder can be attached to any input pins (just need to update the firmware if they are changed) and GND.
<img width="680" height="747" alt="image" src="https://github.com/user-attachments/assets/5b3d7ddb-404e-4e18-8cc1-3cdc527eccd2" />


# Firmware
The firmware using the ESP32spotify library.

# BOM
**Printed Parts**
|Name| Quantity| Picture|
|--|--|--|
|Case| 1| <img width="909" height="662" alt="image" src="https://github.com/user-attachments/assets/fc91b9d5-ec68-47b3-a3d2-8751bf4e03db" /> |
| Back plate| 1| <img width="916" height="605" alt="image" src="https://github.com/user-attachments/assets/81f9969a-eb25-453b-bed4-cc8b0be54698" /> |

**For ease of print, these are combined into one .step file in the repo

**Electronics**

|Name| Quantity| Description| Cost (USD)| Link|
|--|--|--|--|--|
|ESP32|1| The MCU of the project, any esp32 works| $4.50 |https://www.aliexpress.com/item/1005005953505528.html?spm=a2g0o.productlist.main.1.3ed47404vjRFbB&algo_pvid=e75c5d9e-cd52-441e-98f5-ac219f941793&algo_exp_id=e75c5d9e-cd52-441e-98f5-ac219f941793-0&pdp_ext_f=%7B%22order%22%3A%2215159%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21AUD%216.42%211.41%21%21%2130.94%216.81%21%402103123917725849678445010e6571%2112000035007650505%21sea%21AU%210%21ABX%211%210%21n_tag%3A-29910%3Bd%3A7206fb8d%3Bm03_new_user%3A-29895%3BpisId%3A5000000197843401&curPageLogUid=hkIk8oxswLMs&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005005953505528%7C_p_origin_prod%3A \
|LCD | 1| The ST7735 LCD to display track and artist etc| $7.53 | https://www.aliexpress.com/item/32847628219.html?spm=a2g0o.productlist.main.5.2dff3df0EAOllR&algo_pvid=e20e1612-e182-4d38-9a59-614ca70b7886&algo_exp_id=e20e1612-e182-4d38-9a59-614ca70b7886-4&pdp_ext_f=%7B%22order%22%3A%222516%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21AUD%218.83%211.41%21%21%216.18%210.98%21%402101d97817725854775072406e5de0%2166452845724%21sea%21AU%210%21ABX%211%210%21n_tag%3A-29910%3Bd%3A7206fb8d%3Bm03_new_user%3A-29895%3BpisId%3A5000000197843401&curPageLogUid=nYLKUvLWZOvH&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A32847628219%7C_p_origin_prod%3A |
| MX switches | 3| Switches to control spotify e.g pause | $4.68 | https://www.aliexpress.com/item/1005006091988869.html?spm=a2g0o.productlist.main.4.235f3a60U3KZRB&aem_p4p_detail=202603031646083477721552828640000773857&algo_pvid=1ef28bdd-c7cd-41bc-bc2a-aaca5634276e&algo_exp_id=1ef28bdd-c7cd-41bc-bc2a-aaca5634276e-3&pdp_ext_f=%7B%22order%22%3A%22875%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21AUD%216.67%211.41%21%21%2132.11%216.77%21%4021032f3717725851680988022ea544%2112000035698597729%21sea%21AU%210%21ABX%211%210%21n_tag%3A-29910%3Bd%3A7206fb8d%3Bm03_new_user%3A-29895%3BpisId%3A5000000197843477&curPageLogUid=ehMRPQgwfEZ6&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005006091988869%7C_p_origin_prod%3A&search_p4p_id=202603031646083477721552828640000773857_1 |

I also require one rotary encoder, but I already have that and keycaps at home, so I don't need to purchase them.

