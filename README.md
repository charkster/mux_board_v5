# mux_board_v5
Custom PCB with SAMD21 QT PY controlling TWO ADG1606BRUZ 16 input muxes! This board is 30% smaller than V3 and uses a single 16x2 pin header. There are two firmwares for this board, as the backside input pin numbering does not match the topside numbering. You can select which side you would like to be on-top... the QT PY board is much taller than the ADG1606BRUZ packages, and I plan to have the backside on-top (to aviod any unwanted contact with the boards that I connect to).

![picture](https://github.com/charkster/mux_board_v5/blob/main/mux_board_v5_top_side.png)

![picture](https://github.com/charkster/mux_board_v5/blob/main/mux_board_v5_back_side.png)

Check-out my **PDF** [schematic](https://github.com/charkster/mux_board_v5/blob/main/mux_board_v5.pdf) !!

The SAMD21 QT PY can be  programmed with the qt_py_samd21-usbtmc.uf2 file (drag-n-drop) and has the same USBTMC commands that my [Mux Board V1](https://github.com/charkster/mux_board_v1) had. Here is the list:

**MUX1:EN 1** # enable MUX1, a zero will disable the mux

**MUX1:SEL 1** # select S1 input, values 1 through 16 are valid

**MUX1:EN?** # this query returns the state of MUX1

**MUX1:SEL?** # this query returns the presently selected input

***RST** # disables all MUX enables

***IDN?** # returns valid commands and this URL

![picture](https://github.com/charkster/mux_board_v5/blob/main/2x16_pin_header_aliexpress.png)

2x16 2.54mm stacking headers can be found on [Aliexpress](https://www.aliexpress.us/item/2255800630914427.html)

![picture](https://github.com/charkster/mux_board_v3/blob/main/SAMD21_QT_PY_.jpg)

SAMD21 QT PY and ADG1606BRUZ ICs can be found on Digikey/Mouser.
