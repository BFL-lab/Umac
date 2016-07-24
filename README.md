# umac

Umac is a multiple alignment converter.

This package is based on activities of the [OGMP](http://megasun.bch.umontreal.ca/ogmp/) (i.e, priori to 2002), and
becomes open source as part of [MFannot](http://megasun.bch.umontreal.ca/RNAweasel/).

## Install

To install umac you just need to copy the `umac` file in one of your executable directory (e.g: a directory list in $PATH). **Note**: At this point the installation of umac was only tested on Unix system (Ubuntu and CentOS).

## Usage

In order to get the the help page of umac you need to type `umac -h` in your terminal.

#### List of known formats and the programs which use them

Format (-f) | Description | Programs (-p)
------------|-------------|---------------
CLUSTAL     | Clustal W (interleaved) |  clustalw
FASTA       | FASTA (Pearson)         |  jknife, phyms
GDE         | GDE                     |  gde
NEXUS       | NEXUS (Paup)            |  paup
Phylip-I    | Phylip interleaved      |  IQPNNI, RAxMLHPC
Phylip-N    | Phylip non-interleaved  |  pb
RAW         | Raw (one line per seq)  |  RNAfold
STOCKHOLM   | Stockholm (interleaved) |  hmmer, infernal

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) and [CONDUCT](CONDUCT.md) for details.

## Credits

- [All Contributors](https://github.com/natacha-beck/bf-umac/graphs/contributors)

## License

GNU General Public License v3.0. Please see [License File](LICENSE.md) for more information.
