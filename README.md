![](../../workflows/gds/badge.svg) ![](../../workflows/docs/badge.svg) ![](../../workflows/test/badge.svg)

# SAP-1 Computer with an ASIC

Originally, Malvino and Brown presented the SAP-1 architecture in a book called Digital Computer Electronics. 
The design gained massive popularity when it was build as a bread board computer by Ben Eater on a series of YouTube videos. 
The architecture contains various modules, including
- Clock 
- Program Counter
- Register A
- Register B
- Adder
- Memory
- Instruction Register
- Bus
- Controller

This design doesn't have inputs, it is dependent only on the clock that coordinates sequence of the computer's operation. 
Its operation consists on the communication that that bus provides between modules; the signal load dumps information into a module
and the enable signal allows the bus to receive a signal. The bus is 8-bit width since it is an 8 bit computer, and the registers
are also 8-bit registers. 
The computer can only perform addition, whether it is positive numbers or negative numbers (substraction). 
The signals information is stored within the memory module. There bus operations are coordinated with a series of multiplexers and      
the instruction execution set gives the SAP-1 a total of six stages from 0 to 5, repeating all over again. 
The more important module      is the controller. It controlls the assertion execution according to the stimuli from the stages.
The stages 3 to 5 five depend on the instructions of the operation codes. 


# What is Tiny Tapeout?

TinyTapeout is an educational project that aims to make it easier and cheaper than ever to get your digital designs manufactured on a real chip.

To learn more and get started, visit https://tinytapeout.com.

## Verilog Projects

Edit the [info.yaml](info.yaml) and uncomment the `source_files` and `top_module` properties, and change the value of `language` to "Verilog". Add your Verilog files to the `src` folder, and list them in the `source_files` property.

The GitHub action will automatically build the ASIC files using [OpenLane](https://www.zerotoasiccourse.com/terminology/openlane/).

## How to enable the GitHub actions to build the ASIC files

Please see the instructions for:

- [Enabling GitHub Actions](https://tinytapeout.com/faq/#when-i-commit-my-change-the-gds-action-isnt-running)
- [Enabling GitHub Pages](https://tinytapeout.com/faq/#my-github-action-is-failing-on-the-pages-part)

## Resources

- [FAQ](https://tinytapeout.com/faq/)
- [Digital design lessons](https://tinytapeout.com/digital_design/)
- [Learn how semiconductors work](https://tinytapeout.com/siliwiz/)
- [Join the community](https://discord.gg/rPK2nSjxy8)

## What next?

- Submit your design to the next shuttle [on the website](https://tinytapeout.com/#submit-your-design). The closing date is **November 4th**.
- Edit this [README](README.md) and explain your design, how it works, and how to test it.
- Share your GDS on your social network of choice, tagging it #tinytapeout and linking Matt's profile:
  - LinkedIn [#tinytapeout](https://www.linkedin.com/search/results/content/?keywords=%23tinytapeout) [matt-venn](https://www.linkedin.com/in/matt-venn/)
  - Mastodon [#tinytapeout](https://chaos.social/tags/tinytapeout) [@matthewvenn](https://chaos.social/@matthewvenn)
  - Twitter [#tinytapeout](https://twitter.com/hashtag/tinytapeout?src=hashtag_click) [@matthewvenn](https://twitter.com/matthewvenn)
