# MP2359-Buck-regulator
This is the first buck regulator I designed following the datasheet as correctly as I could without following any tutorial or anything
Here the voltage can be regulated more efficiently and 12V is stepped down to 3.3V
The enable pin has to have less than 6V for turning the chip on
The feedback resistors help in controlling the output to 3.3V
The A03401A p channel MOSFET works as a reverse polarity protection and better than the diode 1N4007 since the voltage drop in MOSFET is around 50-100mV while for the diode it is almost 0.7V.So the MOSFET is basically superior in terms of voltage drop,efficiency and heat dissipation
![Schematic](Schematic.png)
![3D_view](3D_view.png)


# Known Limitations and Future Improvements
The SW loop path with catch diode,inductor and capacitor needs to be as small as possible and clustered together.Even a few mm increase in trace introduce inductance causing voltage spike,electromagnetic interference and efficiency loss which needs to be improved in this design
