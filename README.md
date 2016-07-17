# umac

Umac is a multiple alignment converter.

This package is based on activities of the [OGMP](http://megasun.bch.umontreal.ca/ogmp/) (i.e, priori to 2002), and
becomes open source as part of [MFannot](http://megasun.bch.umontreal.ca/RNAweasel/).

## Install

To install umac you just need to copy the `umac` file in one of your executable directory (e.g: a directory list in $PATH).

## Usage

umac [-@[n]] [-v] [-c] [-K] [-S #] [-f format|-p program] [-i infile] [-o outfile] [-F -g global_percent -s sp_percent -n nt_percent]

- i is the input file, containing one or many multiple alignments
- o is the output file, converted
- f is the output format
- p is an alternative to -f, where you specify which external program will use this output; the -f format will be selected for you
- v makes the program more verbose
- c tells the program to check the alignments for errors/inconsistencies
- K tells the program to allow any and all non blank characters in sequence data
- S # indicates that the first # sequences are structure descriptions
- F use filter for STOCKHOLM if only -F is defined used default value for -g, -n, -s
- g retain sequence columns that are of value defined in g (*,9,8...;  #=GC PP_cons default: '*')
- n retain sequence columns with a percentage of sequence characters larger than or equal as defined in n (default: 70% retain)
- s replace sequences for every species that are worse than the value defined default: '*'

Leaving -i and/or -o blank or supplying a single '-' can be used
to mean STDIN or STDOUT for the files.

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
