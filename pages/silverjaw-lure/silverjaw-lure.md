## Silverjaw Lure

The Silverjaw Lure is dual break-out board providing both an mPCIe and mSATA
slot via MinnowBoard development boards' HSE connector. This lure is produced and sold by [Tin Can Tools](http://www.tincantools.com/MinowBoard_Max_Add-ons/Silverjaw_Lure.html) 

**Note:** Lures are owned and supported by their respective owners and manufactures.
The community can only give you best effort support; issues should be taken
to the respective manufacturers and designers.

The Silverjaw Lure is an expansion board for MinnowBoard boards that plugs
into the High Speed Expansion (HSE) connector on the bottom of the board. 
It adds dual interfaces: mSATA socket and mPCIE socket. The Silverjaw Lure
provides switching power supplies (+3VDC & +1.5VDC) so it is very efficent and
minimizes the current draw from the board's main +5V power supply.

### mSATA

The mSATA socket interfaces to the board's PCI express bus which provides
a high bandwidth interface for memory cards. The board can be configured
to boot from the mSATA memory card. The mSATA socket supports both half-size and
full-sized mSATA memory cards.

### mPCIe

The mPCIe socket interfaces to the board's PCI express bus which provides
a high bandwidth interface for mPCIe cards. The mPCIe socket accepts the following
type of mPCIe cards: wifi, SATA drive interfaces, SD memory card, USB 2.0, USB 3.0,
RS-232 serial cards, etc.

**Note:** Tin Can Tools recommends using a +5VDC@3A power supply when using the
Silverjaw Lure with MinnowBoard development boards.

![Silverjaw Lure](pages/silverjaw-lure/1200px-Silverjaw_lure.png)

### Design files

- View the design files on [GitHub](https://github.com/MinnowBoard-org/design-files/tree/master/expansion-boards-lures). 
- All Silverjaw Lure design files are released under Creative Commons Attribution-ShareAlike 4.0 International License.
- Read about what this license allows for on the [Creative Commons website](http://creativecommons.org/licenses/by-sa/4.0/).

### Known Issues

#### Suspend / Resume disables PCI-E =

Suspending, and resuming, the boards that the Silverjaw is attached to may
cause the device on the PCI-E bus to not resume correctly. Rebooting should resolve
the issue. This is because the soft reset signal isn't connected. This is expected
to be fixed in the Rev B of the Silverjaw boards (no current ETA)
