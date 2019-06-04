[![Build Status](https://travis-ci.org/tseemann/phastaf.svg?branch=master)](https://travis-ci.org/tseemann/phastaf)
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
![Don't judge me](https://img.shields.io/badge/Language-Perl_5-steelblue.svg)

# phastaf

Identify phage regions in bacterial genomes for masking purposes

## Introduction

## Quick Start

```bash
% head -n 4 contigs.fna
>AE004092.2 Streptococcus pyogenes M1 GAS, complete genome
TTGTTGATATTCTGTTTTTTCTTTTTTAGTTTTCCACATGAAAAATAGTTGAAAACAATAGCGGTGTCCC
CTTAAAATGGCTTTTCCACAGGTTGTGGAGAACCCAAATTAACAGTGTTAATTTATTTTCCACAGGTTGT
GGAAAAACTAACTATTATCCATCGTTCTGTGGAAAACTAGAATAGTTTATGGTAGAATAGTTCTAGAATT

% phastaf --outdir out contigs.fna

% cat out/phage.bed
AE004092.2	529586	570503	370.1
AE004092.2	778519	821003	370.2
AE004092.2	1189119	1222648	370.3
AE004092.2	1773338	1786887	370.4
```

## Installation

### Homebrew

```
brew install brewsci/bio/phastaf  # COMING SOON
phastaf --check
```
Using Homebrew will install all the dependencies for you: 
[Linux](http://linuxbrew.sh) or [MacOS](http://brew.sh)

### Conda

```
conda install -c bioconda phastaf  # COMING SOON
phastaf --check
```
Learn more about [Bioconda](https://bioconda.github.io/).

### Source

```
git clone https://github.com/tseemann/phastaf.git
./phastaf/bin/phastaf --help
./phastaf/bin/phastaf --check
```
You will need to install all the dependencies manually:
* diamond >= 0.9
* bedtools >= 2.0
* any2fasta >= 0.4
* sort (GNU or BSD)

## Feedback

Please file questions, bugs or ideas 
to the [Issue Tracker](https://github.com/tseemann/phastaf/issues)

## License

[GPLv3](https://raw.githubusercontent.com/tseemann/phastaf/master/LICENSE)

## Citation

Not published yet.

## Authors

* Torsten Seemann
* Jake Lacey
* Sharif Shaaban
* Federica Palma 
* Rebecca Ji Bengtsson
* Nabil-Fareed Alikhan
* Carlus Deneke
