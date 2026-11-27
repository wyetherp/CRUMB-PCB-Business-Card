# CRUMB PCB Business Card

**Make technology yours.**

A battery-free NFC business card built as a printed circuit board. Bring a compatible phone near the antenna and the card's LED illuminates; the phone reads the stored website link.

**Full build guide:** [buildcrumb.com/card](https://buildcrumb.com/card)

| Front — NFC antenna and contact details | Reverse — CRUMB artwork |
| --- | --- |
| ![Front of the manufactured CRUMB card](images/card-front.jpg) | ![Reverse of the manufactured CRUMB card](images/card-back.jpg) |

## How it works

The phone generates a short-range electromagnetic field. The PCB antenna couples to that field, supplying energy to the passive NFC circuitry and LED. The phone reads the stored NFC data and offers to open the website. No battery or charging is required.

## From idea to product

I developed the concept, commissioned the electrical design from a PCB designer, and handled manufacturing preparation, ordering, testing, NFC configuration, and website integration. The original manufacturing process required additional work on the BOM and component placement files.

The purpose of this project is to help others understand how to turn a hardware idea into something they can hold and use.

## Manufacturing files — Rev 3.0

| File | Purpose |
| --- | --- |
| [Gerbers and drill files](CRUMB%20PCB%20card%20gerbers/) | Copper, solder mask, paste, silkscreen, board outline and holes |
| [bom.xls](bom.xls) | Assembly bill of materials |
| [JLCPCB-formatted CPL](CRUMB_Rev3_JLCPCB_CPL_Formatted.csv) | Component coordinates, board sides and rotations |
| [Original KiCad placement export](PCB_Business_card_Rev_3.0-all-pos.csv) | Reference placement data |

The Gerber job metadata describes a two-layer board approximately 86.65 × 54.81 mm, with nominal thickness of 1.6 mm. The photographed boards have a black-and-gold finish. Verify the actual manufacturing and finish options against the successful order; these are not a confirmed order specification.

**Release status:** A physical batch was successfully manufactured and tested by the project creator. The placement files were recovered from the original project records; the exact submitted order files, BOM part selections, and component orientations should be checked before placing another order. Editable KiCad source is not yet included.

## Make your own

1. Read the [complete project guide](https://buildcrumb.com/card).
2. Obtain the editable KiCad board and schematic files if you want to customize the design. The Gerbers are fabrication outputs, not editable design source.
3. Replace the personal contact details, QR code and artwork as appropriate, without disturbing the functional antenna, pads or traces. Have any electrical changes reviewed.
4. Zip the contents of the Gerber folder and upload them to your PCB manufacturer.
5. Select PCB assembly if you want populated boards. Upload the BOM and CPL in the manufacturer's accepted formats.
6. Confirm matched components, polarity, rotation, top/bottom placement, dimensions, finish and total quote before paying.
7. Inspect and test the finished boards. Use a compatible NFC-writing application to write your own website URL if the tag is writable; verify the link and QR code independently.

Start with a small prototype batch. Do not lock an NFC tag until you are certain the stored information is correct.

## What it cost

My first run cost approximately:

- Electrical design: **$250**
- Manufacturing and assembly order: **$250**
- Total project cost: **$500**

My approximate all-in cost was around $30 per card. This includes one-time design expense; it is not a manufacturing-only unit price or a quote. Small batches can be relatively expensive, and per-unit costs depend on quantity, finish, assembly, components, shipping and other fees.

## Licensing and credits

Project concept and manufacturing: Wyeth Anzilotti / CRUMB. Electrical design: commissioned PCB designer.

A public reuse license has not yet been added to this repository. Publication and reuse rights must be confirmed against the designer's agreement before granting a license. CRUMB branding, original artwork, and personal contact information should not be reused in a way that implies affiliation or endorsement.

## Connect

- [CRUMB Workshop](https://buildcrumb.com)
- [Full card guide](https://buildcrumb.com/card)
- [GitHub](https://github.com/wyetherp)
- Email: [wyeth@buildcrumb.com](mailto:wyeth@buildcrumb.com)
