# Connector reference model

`178780-1_reference.step` is the connector-only reference used by the Toyota76
project. It contains no enclosure, PCB, or mounting hardware.

## Source and transformation

Derived from the rusEFI hellen-one library's related 178780-1 model:
https://github.com/andreika-git/hellen-one/blob/67bbd4aae1d23e1ba5f4fffe9fc006b45069af81/kicad/models/178780-1.STEP

Original source SHA-256:
`8f98b92d4ba5ef5ed379239fe2efaab320ef6014399f4fa7bb19bc82936d5734`

The source geometry was rotated -90 degrees about X, then 180 degrees about Y,
and translated by (65.71434, 25.4, 0) mm, using FreeCAD 1.0.2. These transforms
are baked into the supplied STEP geometry. Upstream model provenance is retained;
this addition does not assert ownership or a new license over third-party geometry.

## KiCad registration

The P25 model entry uses offset (-69.20027, 0, 0) mm, unit scale, and zero rotation.
The X offset compensates for the difference between P25's footprint origin and
the centred Toyota76 connector footprint. Pad coordinates, holes, tracks, zones
and net assignments in this repository have not been changed.

## Fit limitations

The source is **178780-1**, not a certified **3-178780-6** model. The family
reference and imported footprint differ: required X translations vary by about
0.349 mm between pin sections, and the locating-hole positions differ. Central
visual alignment does not establish interchangeability or approve drilling,
enclosure dimensions, or mating fit. Verify the actual part and manufacturer
drawing before manufacture.
