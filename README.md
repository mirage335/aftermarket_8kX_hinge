Copyright (C) 2020- mirage335
See the end of the file for license conditions.
See license.txt for aftermarket_8kX_hinge license conditions.


Aftermarket hinges to attach Pimax Vision 8kX to Modular Audio Strap, at angles different from those supplied by the original manufacturer Pimax. As a '3D printable' aftermarket modification, including derived third-party work under apparent GNU GPL v2 license, these alternative hinges are an independent offering.

Still, "mirage335" wishes to extend significant gratitude to Pimax, as well as the community established around Pimax, for the introduction of useful VR technology, that such aftermarket products are intended to further support.


# Usage

Be prepared to do some adjustment and experimentation.

Best fit may be obtained when most pressure from the VR headset is placed at the top of the comfort kit, and some, perhaps one-third, is placed closer to the nose.

As little as 1 degree may be the difference between substantial discomfort, or greatly increased usability during long VR sessions, particularly for simulation and CAD VR users.

Take care to ensure symmetric alignment - both left and right hinges should be at the same angles except in rare cases of the human user not being exactly bilaterally symmetric.


# Distribution

Consider providing end-users an entire copy of this repository with all submodules, in addition to PDF documents. Physical USB flash devices may be suitable for the repository, printed hardcopy may be suitable for the PDF documents.

All manufactured copies of this design should include at least a link to the source repository, regardless of legal requirements to do so.


# Design


Partly derived from a third-party CAD model, which documented correct geometric dimensions for the hinges used by the Pimax Vision 8kX and attached Modular Audio Strap. Portions of this prior CAD model are directly included in the 'legacy' design.

https://www.thingiverse.com/thing:4590303/files
http://www.gnu.org/licenses/old-licenses/gpl-2.0.html
https://github.com/pavel-ruban/Pimax
https://cad.onshape.com/documents/fc37eacb99e7b11e2a322105/w/a07aab2718f48f7bca448c96/e/941ae8a6d26472d6f4b638b7


User 'mirage335' is expected to have needed the MAS strap to lower to a somewhat further angle than most users - apporximately 159deg which may have been slightly lower due to 3D printing tolerance at the time. Consequently, angles useful to others are expected to fall between 157deg-161deg with possible outliers at 155deg (provided by Pimax plastic hinges) or 163deg (expected to be rarely desirable).

Emboss font used is from '/usr/share/fonts/truetype/dejavu/DejaVuSansMono-Bold.ttf' (typical installed directory/file) , or similar, as specified in CAD model.

Angled (not flat) brackets may reduce screw length, reduce weight, improve adaptability (if flexible material), reduce plastic/material, reduce print time, and possibly add a small gap to improve compressibility under assembly screw pressure. Flat brackets may improve adjustability, improve repairability, increase layer adhesion, and reduce vibration during manufacturing (reducing wear on 3D printers).
Flat brackets, horizontal alignment, platter 10x, no pillar base, no pillar post...
* 90% Infill - 138% print time, 162% plastic
* 40% Infill - 116% print time, 135% plastic

Flat brackets, vertical alignment, platter 10x, no pillar base, no pillar post...
* 90% Infill - 153% print time, 175% plastic
* 40% Infill - 129% print time, 147% plastic


# Redistribution and Preservation

Entire 'recursive' clones of this repository with all submodules may be appropriate for redistribution and preservation.


# Safety


# FutureWork


# Reference

https://wiki.freecadweb.org/A2plus_Workbench
https://github.com/mirage335/freecad-assembly2



https://apps.dtic.mil/dtic/tr/fulltext/u2/a268661.pdf


https://www.fastenal.com/product/fasteners/screws/machine-screws/600059?categoryId=600059&level=3&aggregationSection=true&Dia%2FThread+Size=M2-0.4&Dia%2FThread+Size=M2.5-0.45&Dia%2FThread+Size=M2&Dia%2FThread+Size=M2.5&Length=12mm&showAll=Dia%2FThread+Size&showAll=Length&selectedAggregation=Length

https://www.amazon.com/s?k=m2x40mm&i=tools&ref=nb_sb_noss

https://www.pocketscrewdrivers.com/Logo_Pocket_Screwdrivers_s/3.htm


# Directory Specification

Consider keeping a copy of this specification alongside relevant projects for reference.

Please regard as a loose specification intended to offer unallocated regions for expansion and subordinate to any improvements that may be found in actual implementations.


Projects which may be assembled into larger projects, if sufficiently well-developed, should include their own appropriate directories, rather than referencing files shared within larger projects. That is to say, a sort of 'static linking' approach is strongly recommended.



Numbered directories with '[z]-' in their prefix and a '/' may substitute the '/' for either a '-' or separate directories.

Numbered directories of top-directories may be placed alongside top-directories if desired. Numbering scheme is intended to minimize conflicts.

Templates should populate only the most usual directories. Not all directories need be populated for a project.


```

_lib	- software, records, etc, typically uniquely needed by specific CAD model

00[00]-RESERVED (do NOT use)


01[00]-Bundle
	0110-Frames
	0150-Actuators
	0151[z]-Thruster/Driver
		Components only used for these?
		Screws used within these?
	0160-Tools
		Nozzle
		Hot-End
		Cold-End
		Extension (Bowden Tube)
	0162-Supplementary
		Filament Storage
	0165-Slab (workpiece mounting surface)
	0170-Tray (surface to mount electronics and similar)
	0172-Rack (enclosure for electronics and similar, and/or junction box)
	0175-Cabinet (arbitrary storage)



11[00]-Structural (Passive, Cut To Size)
	1110[z]-Extrusions/Timbers
		_resized
	1112[z]-Sheets/Panels/Plates (for frames only)
		_rescaled (PreDrilled only)
	1115-Backing (Table)



30[00]-Conveyance
	3030[z]-Shaft/Piston
	3032-LeadScrew
	3033[z]-Belts
	3035- to 3038- RESERVED (do NOT use)

35[00]-Couplings (including flexible, u-joints, etc)
	3530-LeadScrew_to_Motor



50[00]-Effectors
	5050[z]-Motors/Steppers/Servos
	5051[z]-RotaryBearings/RotaryShims
	
	5052[z]-NutBlocks/PlatesEffectors/BracketsEffectors (typically belt tie-down points), etc.
	5053-RESERVED
	
	5054[z]-Guides (Wheels/Bushings/LinearBearings)
	
	5055-Pulleys
	5056-Gears
	
	5058-Limit Switch

55[00]-RESERVED (do NOT use)
	

(6000 RESERVED)

(7000 RESERVED)



80[00]-Endpoints
	8080-Plug
		RJ45
		misc
	8081-Jack
		RJ45
		misc
	8082-RESERVED (do NOT use)
	8083-RESERVED (do NOT use)

85[00]-Dissipator
	8580-Fans
	8581-Pump
	8582-Heatsink
	8585-Radiator

9000-Miscellaneous
	9090z-Screws/Bolts
	9095-frequent (most frequently used)
	9099-Misc
		zMisc (unsortred, typically uniquely needed by specific CAD model)

9100-KEEPOUT (solid objects used to mark regions reserved for future use)

94[00]
to
98[00]
	RESERVED for future use

99[00]-import
	RESERVED for future use


```


# Manufacturing

Recommended 3D printer 'slicer' settings...

* No 'Brim'.
* Solid infill threshold area >70mm^2 .
* >45% Fill, 'Rectilinear'
* <0.3mm Layer Height
* <0.5mm Extrusion Width
* 2 'vertical shells', 2 'horizontal shells'
* disable 'external perimeters first'


* >50% Infill/perimeters overlap


* <0.25mm or 0mm XY Size Compensation
* 0mm (full) 'Resolution'


* 3mm extruder
* 240mm/s travel speed
* 85mm/s print speed
* 65mm/s 'gap fill'


* disable 'complete individual objects'


Occasionally one overhanging perimeter may sag down from the hinge inner surface. Such a perimeter should be removed with tweezers, more than one such sagging perimeter line may be cause to consider the print a failure.

The pillar post and pillar base should easily fit together, and should not be tightened until held in place by screw and/or glue.

A vise may be used during screw tightening to ensure correct alignment. Screw should be tight enough to prevent rotation of the pillar post - this tightening will also ensure the pillar base does not separate from the underlying bracket when under pressure.

An M2.5 or M2 screw, length 12mm, 10mm, or 8mm, should be used to join pillar post and pillar base. Phillips head is specifically strongly discouraged.

Flexible material - such as NinjaFlex - may be able to maintain desired pressure towards the top of the head - with a wider variety of geometries and pressures. This has not been tested.


# Hinge Pins

Apparently these are 'headless shoulder bolts' or 'threaded link band screw' - perhaps M1/M2/M2.5 diameter/thread , 30mm shoulder length , 35mm total length . Despite some effort and progress in determining possible sources for these visibly standards resembling screws, at least their length seems to be unusual.

Heat shrink tubing around more typical M1/M2/M2.5x40mm screws may be a practical workaround.



# Third-Party Copyright Notices

Third-Party copyrights are noted within text files alongside directories containing the original files, and/or within text files alongside directories containing the modified files, and/or within version control commit history.

Some copyright licenses have specific requirements, and some authors have specific requests, to prominently display copyright notices - these are included here.

However, the manner some or all of these third-party files are used may in fact be fair use, in which case the third-party licenses would not in fact have any effect on the license requirements for the otherwise possibly derivative project.



While other files in the 'aftermarket_8kX_hinge' may, as stated, be redistributed under GNU GPL license versions later than version 2, all files derived from (or otherwise including) third party files obtained under apparent GNU GPL v2 license, must retain that license.




# Copyright

This file is part of aftermarket_8kX_hinge.

aftermarket_8kX_hinge is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 2 of the License, or
(at your option) any later version.

aftermarket_8kX_hinge is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with aftermarket_8kX_hinge.  If not, see <http://www.gnu.org/licenses/>.








