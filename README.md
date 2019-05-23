# fpga-examples

These are some of the Verilog examples from the book
["Designing Video Game Hardware in Verilog"](https://www.amazon.com/gp/product/1728619440/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=1728619440&linkCode=as2&tag=pzp-20&linkId=c149f6365c0a676065eb6d7c5f8dd6ae)
ported to CRT monitor timing and tested against the [IceStorm](http://www.clifford.at/icestorm/) tools.

## Installation

On Ubuntu:

    sudo apt-get install yosys arachne-pnr
    git clone https://github.com/sehugg/fpga-examples
    cd fpga-examples/ice40
    
To syntheisize and upload to the FPGA:

    make starfield.bin
    iceprog starfield.bin

To connect the FPGA to a composite output, you might need to make a 2-bit DAC out of resistors, [like this one](https://web.archive.org/web/20181001053135/http://www.rickard.gunee.com/projects/video/pic/howto.php).

## License

All files in this repo are licensed under [CC0](https://creativecommons.org/publicdomain/zero/1.0/) (public domain)
