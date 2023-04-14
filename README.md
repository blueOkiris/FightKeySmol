# Fight Key Smol

## Description

I made a [hitbox for myself](https://hackaday.io/project/185796-fight-key-wide) a while back that's big and has an enclosure and all that good stuff and cost me maybe $80 to make.

However, lately I've been seeing people pay well over $100 for something that should be maybe $50 max, so I'm redesigning that to fit the style people want, so there's a cheap alternative.

Now yes, you're paying for quality with the others. This doesn't come with an enclosure, and it's DIY; it's minimal, but for some people, that's worth not dropping >= $100. It's an option. That's all

So, this project aims to be a tiny, inexpensive, DIY, keyboard-based fighting-game controller.

![Image of Physical Fight Key](pics/board-pic.jpg)

## Parts

It currently costs \~$31 for materials, but shipping is another $20, so I will likely continue to look for more options to cut costs as even $50 is absurd.

| Part         | Link                                             | Cost |
|:------------:|:------------------------------------------------:|:----:|
| PCB          | [Jlcpcb](https://jlcpcb.com/)                    | $10  |
| PCB Shipping | Choose Global Standard for cheaper               | $10  |
| Switches     | [Amazon][SwitchLink]                             | $7   |
| Key Caps     | [Aliexpress][CapLink]                            | $2   |
| Pico         | [Amazon][PicoLink]                               | $8   |
| Rubber Feet  | [Aliexpress][FeetLink] (Hot Glue is alternative) | $3   |
| Total        | -                                                | $40  |

There are probably cheaper ways to get parts like switches, but here's some starting points.

[SwitchLink]: https://www.amazon.com/Keyswitch-Replaceable-Switches-Mechanical-Keyboard/dp/B07V4S3QDK/ref=sr_1_1?crid=2KVKUIIAKWWWM&keywords=cherry+mx&qid=1680653938&refinements=p_85%3A2470955011&rnid=2470954011&rps=1&s=electronics&sprefix=cherry+mx%2Celectronics%2C119&sr=1-1 "Amazon"

[CapLink]: https://www.aliexpress.us/item/3256803462871478.html?spm=a2g0o.productlist.main.15.fd98sl21sl21Ub&algo_pvid=9ed2559f-ab14-4ea8-b05c-93050b38520c&algo_exp_id=9ed2559f-ab14-4ea8-b05c-93050b38520c-7&pdp_npi=3%40dis%21USD%211.5%211.12%21%21%21%21%21%4021224e9b16806567975486574d074d%2112000026645768333%21sea%21US%210&curPageLogUid=vViLogs9j2Z2 "Aliexpress"

[PicoLink]: https://www.amazon.com/seeed-studio-Raspberry-Microcontroller-Dual-core/dp/B08TQSDP28/ref=sr_1_5?crid=2AFT7S4T0WLWI&keywords=raspberry+pi+pico&qid=1680652784&s=electronics&sprefix=raspberry+pi+pico%2Celectronics%2C132&sr=1-5 "Amazon"

[FeetLink]: https://www.aliexpress.us/item/3256802824831274.html?spm=a2g0o.order_list.order_list_main.4.21ef18022VpwPs&gatewayAdapt=glo2usa&_randl_shipto=US "Aliexpress"

## Subdirectories

- pcb - Fight Key Smol KiCAD PCB project
- GP2040-CE - submodule containing code.
- pics - Pics used for the README

## Build Instructions

1. Order the board from Jlcpcb. Can just use default options
   ![jlcpcb order](pics/jlcpcb-order.png)
2. Add feet.
   ![feet installation](pics/feet-installation.jpg)
3. Solder the pico to the board.
   ![pico soldering](pics/pico-soldering.jpg)
4. Add caps.
   ![cap installation](pics/cap-installation.jpg)
5. Solder the switches to the board.
   - Press down to make sure they all get put evenly. You may need to 
   - If not even, you can reheat a joint and push on the switch to adjust the angle.
   ![press down](pics/press-down.jpg)
   ![switch soldering](pics/keys-soldered.jpg)
6. Program the pico. You don't need to rebuild it.
   1. Press the pico's button down and plug it in to make it show up as a drive
   2. Copy the .uf2 file in the repo to the drive. It will unmount and program and auto-remount as a controller
   ![pico programming](pics/drag-n-drop.png)
7. Enjoy!

