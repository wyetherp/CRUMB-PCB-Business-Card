# CRUMB PCB Business Card

**Make technology yours.**

A working, battery-free NFC business card, manufactured as a printed circuit board. Bring a compatible phone near the gold antenna and the card's LED lights up. The phone can read a stored website address.

CRUMB is a free educational workshop helping people understand, build and customize technology.

**[Explore the card and full manufacturing guide → buildcrumb.com/card](https://buildcrumb.com/card)**

| Front — NFC antenna and contact details | Reverse — CRUMB artwork |
| :---: | :---: |
| ![Front of the manufactured CRUMB PCB card](images/card-front.jpg) | ![Reverse of the manufactured CRUMB PCB card](images/card-back.jpg) |

## How it works

A compatible phone's NFC reader generates a short-range electromagnetic field. The antenna on the card couples to that field, supplying energy to the passive NFC circuitry and allowing the LED to illuminate. The phone reads the NFC data and offers to open the stored website. No battery or charging is required.

## From idea to product

I developed the concept, commissioned the electrical design from a PCB designer, and handled manufacturing preparation, ordering, testing, NFC configuration and website integration. The original assembly order required additional work preparing the bill of materials (BOM) and component placement list (CPL).

The point of this project is to show that you do not have to be an electrical engineer to begin turning a hardware idea into a physical product. Work with qualified designers when needed, understand what you are ordering, and verify the result.

## Project files — Rev 3.0

| File | What it is for |
| --- | --- |
| [**Download Gerber ZIP**](CRUMB-PCB-Rev3-Gerbers.zip?raw=true) | Upload this archive to a PCB fabrication service. It contains the existing copper, solder mask, paste, silkscreen, outline and drill outputs. |
| [Individual Gerbers and drill files](CRUMB%20PCB%20card%20gerbers/) | Inspect the original fabrication outputs. |
| [BOM — bom.xls](bom.xls?raw=true) | The existing component list; confirm part numbers, availability and assembly requirements with your manufacturer. |
| [JLCPCB CPL CSV](CRUMB_Rev3_JLCPCB_CPL_Formatted.csv?raw=true) | The supplied placement list for automated assembly: coordinates, sides and rotations. |
| [Original KiCad placement CSV](PCB_Business_card_Rev_3.0-all-pos.csv) | Unformatted reference placement export; not an additional component list. |
| [Editable KiCad source](source/) | Recovered Rev 3.0 project, board and schematic for inspection and customization, subject to permissions below. |

The Gerber job metadata describes a two-layer board approximately 86.65 × 54.81 mm, with a nominal thickness of 1.6 mm. The photographed boards have a black-and-gold finish. These are design observations, not a verified list of the exact manufacturing settings used for the successful order.

**Verification and limitations:** The project creator manufactured and tested a physical batch. The formatted CPL is byte-for-byte identical to the supplied file, and its four populated component placements match the recovered Rev 3.0 KiCad board. The original Gerber and BOM files are unchanged. The ZIP contains all twelve original fabrication-related files. The recovered KiCad board, schematic and project files are preserved byte-for-byte, but a fresh export has not yet been compared to the manufacturing package. Confirm the exact final revision, BOM part selection, component orientation and manufacturing settings against the successful order before submitting another order. Custom footprint libraries, artwork source assets and manufacturer order records may be needed for some edits and are not included in the current source folder.

## Make your own

1. Read the [step-by-step CRUMB guide](https://buildcrumb.com/card).
2. **Fabricating the existing board:** Upload the Gerber ZIP to a PCB manufacturer. Fabrication produces a bare board; choose component assembly if you want the electronics installed.
3. **Customizing the design:** Use the editable KiCad project, not the Gerber files. Verify reuse rights first. Replace the contact information, QR code and artwork on the correct layers. Preserve the antenna, traces, pads and component layout unless a qualified designer reviews changes. Regenerate and inspect the manufacturing exports after edits.
4. **Ordering assembled boards:** Provide the BOM and the JLCPCB-formatted CPL (or your factory's required equivalent). Ensure reference designators, part choices, rotations, pin 1, LED polarity, assembly sides and origin agree with the board. Review the assembly preview and quote before payment.
5. **Test:** Inspect the finished boards, confirm the LED response and check NFC functionality with a compatible phone.
6. **Program NFC:** If the tag is writable, use a compatible NFC-writing app to write an NDEF URI record containing your HTTPS website address. Read it back and test the link, and check the printed QR code independently. Do not permanently lock the tag until you have verified the final record.

Start with a small prototype batch. Manufacturing requirements and component availability vary; this repository is a reference, not a guarantee of successful fabrication or assembly.

## What it cost

| Expense | Approximate cost |
| --- | ---: |
| Commissioned electrical design | $250 |
| Manufacturing and assembly | $250 |
| **Total** | **$500** |

My approximate all-in cost was around **$30 per card**, including the one-time electrical design expense. This is not a manufacturing-only unit price or a guaranteed quote.

Customizing a design you have permission to reuse may reduce engineering costs. Larger orders can reduce the cost per card; finish, assembly setup, parts, quantity and shipping all affect the final price.

## Licensing and credits

Project concept and manufacturing: Wyeth Anzilotti / CRUMB. Electrical design: commissioned PCB designer.

The designer has given permission to share the design, as reported by the project creator. A public reuse license is **pending confirmation of rights to grant downstream modification, manufacture and redistribution**. The proposed license is [CERN Open Hardware Licence v2 — Permissive (CERN-OHL-P-2.0)](https://spdx.org/licenses/CERN-OHL-P-2.0.html). That license is not in effect merely because it is proposed here. Contact the project creator before reproducing, modifying or redistributing the design unless you have independent permission.

If granted, the hardware license will cover the specified electrical and manufacturing design files. CRUMB branding, original artwork, photographs and personal contact details are excluded from the proposed grant, including artwork incorporated into hardware files; replace them with your own material before distribution. Preserve any attribution required by the original designer.

## Connect

- [CRUMB Workshop](https://buildcrumb.com)
- [Full card guide](https://buildcrumb.com/card)
- [GitHub](https://github.com/wyetherp)
- [LinkedIn](https://www.linkedin.com/in/wyetherp/)
- [wyeth@buildcrumb.com](mailto:wyeth@buildcrumb.com)
