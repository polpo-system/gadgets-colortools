# gadgets-colortools

ColorTools for the gadgets of [polpo](https://github.com/polpo-system/polpo): a colour picker
gadget; a click on one of its colours runs its command (the Cmd attribute) with the colour.

```
portia.Install gadgets-colortools
```

## Using

    Gadgets.Insert ColorTools.NewColorPicker ~   a picker at the caret
    ColorTools.ChangeColor                       the picked colour for the selected text

## What is here

    src/ColorTools.Mod        the picker
    tools/ColorTools.Tool
    test/ColorToolsTest.Mod

ColorTools is by Johannes Marais. The source comes from ETH Linux Oberon (OLR, 2017-06-18), converted from an Oberon text to plain
text; the first commit has it unchanged. It compiles unchanged with all five of polpo's compilers
(x86, ARM, ARMv7, RISC-V, MIPS).

## Tests

    ColorToolsTest.Run      1 check: a picker made; it needs the desktop's display

The license is GPL-3 (`LICENSE`); the code comes from ETH Oberon, whose license (`LICENSE.ETH`)
asks to keep its copyright notice and conditions, which `LICENSE.ETH` does.
