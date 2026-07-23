# Mecanum Wheel 100mm

Part of the [R-MODUS](https://github.com/R-MODUS) project — a modular indoor robot navigation stack — but this wheel can be used in other projects on its own.

<p align="center">
  <img src="image/mecanum-wheel.png" alt="Mecanum wheel 100 mm" width="48%"/>
  &nbsp;
  <img src="image/mecanum-wheel-1.png" alt="Mecanum wheel — detail" width="48%"/>
</p>

## Parameters

| Parameter | Value |
| --- | --- |
| Wheel diameter | 100 mm |
| Wheel width | 46 mm |
| Width with motor bushing | 56 mm |
| Number of rollers | 9 |
| Shaft bore | Ø 6 mm |
| Mass | ~0.33 kg |
| Part material | PLA (3D print) |
| Roller surface | polyolefin |
| Bearings | 623 |

## Bill of materials (one wheel)

A typical chassis uses 4× (2× standard + 2× mirrored).

| Item | Qty | Note |
| --- | --- | --- |
| Outer ring | 1 | `mecanum-outer-ring.stp` |
| Inner ring | 1 | `mecanum-inner-ring.stp` |
| Shaft interface | 1 | `mecanum-shaft-interface.stp` |
| Roller | 9 | `mecanum-cylinder.stp` |
| Bearing 623 | 18 | 2× per roller |
| Heat-shrink tubing Ø20 mm | 40 cm | electrical grade |
| Screw M4×14 DIN 912 | 4 | — |
| Screw M4×10 DIN 912 | 1 | — |
| Screw M3×50 DIN 912 | 9 | — |
| Nut M4 DIN 934 | 4 | hex |
| Washer 4 DIN 125 A | 4 | — |
| Washer 3 DIN 125 A | 18 | — |
| Heat insert M4 | 1 | brass, Ø6.3 × L 6 mm |
| Heat insert M3 | 9 | brass, Ø4.6 × L 5 mm |

## Assembly

1. Thoroughly clean all printed parts.
2. Cut the heat-shrink tubing into 4 cm pieces, slide them onto the rollers, and shrink with a heat gun (warm gently only so the roller does not deform).
3. In a vise, press two bearings into each roller — one from each side.

<p align="center">
  <img src="image/roller-cross-section.png" alt="Roller cross-section — tubing, bearings, screw" width="420"/>
</p>

4. Melt-install the M3 heat inserts into the outer ring.
5. Melt-install the M4 heat insert into the shaft interface.
6. Stack the shaft interface and both rings; lightly clamp them with four M4×14 screws and nuts. Place washers under the nuts. Orient screw heads toward the outer ring.
7. Insert the rollers one by one and secure them with M3×50 screws; put a washer on each side next to the bearing and tighten carefully.
8. Fully tighten the four M4 screws to lock the rings.
9. Fine-tune: tighten each M3 screw so the roller spins freely but has no axial play.

### Mounting on the motor

1. Slide the wheel onto the Ø 6 mm motor shaft.
2. Secure the wheel with an M4×10 screw.
