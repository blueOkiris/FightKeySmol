# Fight Key Smol

THIS PROJECT IS NOT FINISHED YET!!!!!!!

Don't use

## Description

I made a [hitbox for myself]() a while back that's big and has an enclosure and all that good stuff and cost me maybe $80 to make.

However, lately I've been seeing people pay well over $100 for something that should be maybe $40 max, so I'm redesigning that to fit the style people want, so there' a cheap alternative.

Now yes, you're paying for quality with the others. This doesn't come with an enclosure, and it's DIY; it's minimal, but for some people, that's worth not dropping >= $100. It's an option. That's all

So, this project is a tiny, inexpensive, DIY, keyboard-based fighting-game controller.

![Image of Physical Fight Key](/pics/fk-smol.jpg)

## Parts

| Part        | Link                          | Cost |
|:-----------:|:-----------------------------:|:----:|
| PCB         | [Jlcpcb](https://jlcpcb.com/) | $..  |
| Switches    | [Amazon][SwitchLink]          | $7   |
| Key Caps    | [Amazon][CapLink]             | $10  |
| Pico        | [Amazon][PicoLink]            | $8   |
| Rubber Feet | [Amazon][FeetLink]            | $6   |
| Total       | -                             | $..  |

There are probably cheaper ways to get parts like switches, but here's some starting points.

[SwitchLink]: https://www.amazon.com/Keyswitch-Replaceable-Switches-Mechanical-Keyboard/dp/B07V4S3QDK/ref=sr_1_1?crid=2KVKUIIAKWWWM&keywords=cherry+mx&qid=1680653938&refinements=p_85%3A2470955011&rnid=2470954011&rps=1&s=electronics&sprefix=cherry+mx%2Celectronics%2C119&sr=1-1 "Amazon"

[CapLink]: https://www.amazon.com/Keycap-Keycaps-Percent-Mechanical-Keyboard/dp/B08BR8KSNM/ref=sr_1_33?crid=1NH5LM0OYZRB3&keywords=cherry+mx+keycaps&qid=1680653223&refinements=p_85%3A2470955011&rnid=2470954011&rps=1&s=electronics&sprefix=cherry+mx+key+cap%2Celectronics%2C118&sr=1-33 "Amazon"

[PicoLink]: https://www.amazon.com/seeed-studio-Raspberry-Microcontroller-Dual-core/dp/B08TQSDP28/ref=sr_1_5?crid=2AFT7S4T0WLWI&keywords=raspberry+pi+pico&qid=1680652784&s=electronics&sprefix=raspberry+pi+pico%2Celectronics%2C132&sr=1-5 "Amazon"

[FeetLink]: https://www.amazon.com/UOTOO-Laptop-Diameter-Replacement-MacBook/dp/B087774VG5/ref=sr_1_3?crid=F02BRHEO012B&keywords=sticky+rubber+feet&qid=1680652823&s=electronics&sprefix=sticky+rubber+feet%2Celectronics%2C111&sr=1-3 "Amazon"

## Subdirectories

- pcb - Fight Key Smol KiCAD PCB project
- GP2040-CE - submodule containing code.

## Build Instructions

1. Order the board from Jlcpcb. Can just use default options
   ![jlcpcb order](pics/jlcpcb-order.png)
2. Solder the pico to the board.
   ![pico soldering](pics/pico-soldering.png)
3. Solder the switches to the board.
   ![switch soldering](pics/switch-soldering.png)
4. Add caps.
   ![cap installation](pics/cap-installation.png)
5. Add feet.
   ![feet installation](pics/feet-installation.png)
6. Program the pico
   - ![pico programming step 1](pics/prog-1.png)
   - ![pico programming step 2](pics/prog-2.png)
7. Enjoy!

