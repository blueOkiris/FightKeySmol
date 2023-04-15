# Fight Key Smol

## Description

I made a [hitbox for myself](https://hackaday.io/project/185796-fight-key-wide) a while back that's big and has an enclosure and all that good stuff and cost me maybe $80 to make.

However, lately I've been seeing people pay well over $100 for something that should be maybe $50 max, so I'm redesigning that to fit the style people want, so there's a cheap alternative.

Now yes, you're paying for quality with the others. This doesn't come with an enclosure, and it's DIY; it's minimal, but for some people, that's worth not dropping >= $100. It's an option. That's all

So, this project aims to be a tiny, inexpensive, DIY, keyboard-based fighting-game controller.

![Image of Physical Fight Key](pics/board-pic.jpg)

## Software

The software included in the repo and releases is a pre-built version of the [GP2040-CE](https://github.com/OpenStickCommunity/GP2040-CE) firmware.

For version 1, there is a custom version due to Start and Select being switched. For version 2, this is not the case, and the stock software can be used.

## Parts

The only thing you need to source yourself are the key caps. You can get a cheap set for $2 on [Aliexpress](CapLink).

Beyond that, you'll want to use [Jlcpcb](https://jlcpcb.com) to order the board and use automatic assembly. This will place all the internals as well as the switches into the PCB and ship it to you.

Cost comes out to:

| Part                                              | Cost |
|:-------------------------------------------------:|:----:|
| PCB and Assembly                                  | $22  |
| PCB Shipping (Choose Global Standard for cheaper) | $10  |
| Key Caps                                          | $2   |
| Total                                             | $34  |

[CapLink]: https://www.aliexpress.us/item/3256803462871478.html?spm=a2g0o.productlist.main.15.fd98sl21sl21Ub&algo_pvid=9ed2559f-ab14-4ea8-b05c-93050b38520c&algo_exp_id=9ed2559f-ab14-4ea8-b05c-93050b38520c-7&pdp_npi=3%40dis%21USD%211.5%211.12%21%21%21%21%21%4021224e9b16806567975486574d074d%2112000026645768333%21sea%21US%210&curPageLogUid=vViLogs9j2Z2 "Aliexpress"

## Subdirectories

- pcb - Fight Key Smol KiCAD PCB project
- pics - Pics used for the README

## Ordering and Programming

1. Go to JLCPCB and click on "Instant Quote"
   ![jlcpcb instant](pics/instant-quote.png)
2. Click "Upload" and upload the "FightKeySmol-Gerber.zip" file from the GitHub Releases. You don't need to mess with any options here.
3. Scroll down to "PCB Assembly" and enable it. Select just one and click Submit
   ![jlcpcb assembly](pics/assembly-sel.png)
4. Click Next and then upload the "pcb/parts/BOM.xls" for the BOM and "pcb/parts/FightKey-CPL.xlsx" for the CPL. Then click process.
   ![jlcpcb bom](pic/bom-cpl.png)
5. Click to continue on the next page, and proceed to ordering the boards.
6. Once you have the board, you need to program it. You don't need to rebuild the code or anything.
   1. Press the pico's button down and plug it in to make it show up as a drive
   2. Copy the .uf2 file in the repo to the drive. It will unmount and program and auto-remount as a controller
   ![pico programming](pics/drag-n-drop.png)
7. Enjoy!

