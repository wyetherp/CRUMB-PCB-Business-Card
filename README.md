# CRUMB — PCB Business Card

**Make technology yours.**

A working business card built as a printed circuit board. It lights up and shares a website with your phone through NFC — without a battery.

| Front | Reverse |
| :---: | :---: |
| ![Front of the CRUMB PCB card](images/card-front.jpg) | ![Illustrated reverse of the CRUMB PCB card](images/card-back.jpg) |

[**Full build guide at buildcrumb.com/card →**](https://buildcrumb.com/card)

## How it works

A compatible phone generates an electromagnetic field that the card's NFC antenna harvests energy from. This powers the NFC circuitry and LED. The phone reads the stored website address and offers to open it.

## Make your own

This repository contains the Rev 3.0 design and manufacturing files.

| File | Purpose |
| --- | --- |
| [Gerber ZIP](CRUMB-PCB-Rev3-Gerbers.zip?raw=true) | Fabricate the physical board |
| [BOM](bom.xls?raw=true) | Identify the components needed for assembly |
| [Pick-and-place (CPL)](CRUMB_Rev3_JLCPCB_CPL_Formatted.csv?raw=true) | Tell the factory where and how to place components |
| [KiCad source](source/) | Inspect and customize the board and schematic |

### 1. Customize

Open the KiCad project, replace the artwork, contact information and QR code on the appropriate layers, and export new Gerber and assembly files. Preserve the functional antenna and circuit unless a qualified designer reviews your changes. Confirm the applicable reuse rights first.

### 2. Manufacture

Upload the Gerber ZIP (or your regenerated ZIP) to a PCB manufacturer such as JLCPCB. For assembled boards, also provide the matching BOM and CPL. Verify part selection, placement, orientation, board specifications and the factory preview before ordering a small prototype batch. The recovered source has not yet been independently checked by regenerating all manufacturing outputs.

### 3. Configure NFC

Use a compatible NFC-writing app to store your website URL as an NDEF URI record on a writable tag. Test the link, QR code and LED.

## What it cost

My original project cost about **$500**: $250 for the commissioned electrical design and $250 for manufacturing and assembly. That's approximately $30 per card all-in, including the one-time design expense. Small batches can be expensive; customizing an existing design and ordering larger quantities may reduce costs.

## About CRUMB

CRUMB is a free educational workshop for people who want to understand, build and customize technology. I developed the concept and worked with a PCB designer on the electrical design, then handled the manufacturing, testing and website integration.

See the repository's license, once added, for reuse terms. Until then, sharing the files does not itself grant permission to modify, manufacture or redistribute them.

**[Explore CRUMB](https://buildcrumb.com) · [Full guide](https://buildcrumb.com/card) · [Contact](mailto:wyeth@buildcrumb.com)**
