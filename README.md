# Custom evaluation board for stm32L432KCU6

This is a project of the custom evalution board for stm32L432KCU6.
The eval board was created for future test and prototypin during "2025/26 can-sat 🛰️ competition" organisated by ESA 🇪🇺 (European Space Agency), simultaneously it is a part of our PDR report 📑 (Preeliminary Desing Report).
By creating this board we want to show our capabilities in terms of electronics manufacturing ⚡📟.


<div style="display: flex; justify-content: center; gap: 20px;">
  <figure>
    <img src="images/logo_1 (2).png" alt="Photo 1" width="300">
    <figcaption style="text-align: center;">Logo of my team "Crius SPACE"</figcaption>
  </figure>
  <figure>
    <img src="images\ESA_Edu_Cansat_RGB-kopia-600x600.png" alt="Photo 2" width="300">
    <figcaption style="text-align: center;">We are taking part in can-sat competition by ESA</figcaption>
  </figure>
</div>

<div style="display: flex; justify-content: center; gap: 20px;">
  <figure>
    <img src="images\IMG_2160.jpeg" alt="Photo 1" width="300">
    <figcaption style="text-align: center;">Real images of soldered board (running code)</figcaption>
  </figure>
  <figure>
    <img src="images\kicad_render.png" alt="Photo 2" width="300">
    <figcaption style="text-align: center;">Render of the board in KiCAD</figcaption>
  </figure>
</div>


## future improvements, known issues and thing which are not tested
### known issues ⚠️❗:
- missing labels  - ()

- too small package - the capacitors for the LSE (Y2) are in size of 0402, (especially during manual soldering using hot-air gun or either conventional soldering iron (0603 is ratiobale limit for the size))

- space usage - board is bigger than the most popular eval boards like "blue/black pill" ❗

### probabable issues (not tested) ⚠️❗:
- reversd ESD protection for the usb (it is not necessary to use it)

### future improvements 📈🚀:
- components - no smaller than 0603 for manual soldering

- silk layer labels - complete silk layer labels


## customisation options ⚙️🛠️:
- as you can see on the photos of the real not everything is soldered:
1. 0ohm reistor on every diode - it allows you to reduce power usage in battery base aplications 🔋🪫.

2. 0ohm resistors on signal pins for usb - allows user to use pins in 2 different ways.

3. extra user button - with pull-up resistor and place for anit-debounce capacitor.

## extra files 📂:
1. stm32l432kcu6_eval_part_list.csv - file which contains list of the used elements with quantities for 1 board.

2. documentation folder - (in progress) folder which contains documentation for every component used in the project.

3. production_file_1.zip and production_file_1 - production ready files with current version of the project