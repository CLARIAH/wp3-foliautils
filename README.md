[![Build Status](https://travis-ci.org/LanguageMachines/foliautils.svg?branch=master)](https://travis-ci.org/LanguageMachines/foliautils) [![Language Machines Badge](http://applejack.science.ru.nl/lamabadge.php/foliautils)](http://applejack.science.ru.nl/languagemachines/) [![DOI](https://zenodo.org/badge/36356660.svg)](https://zenodo.org/badge/latestdoi/36356660) [![GitHub release](https://img.shields.io/github/release/LanguageMachines/foliautils.svg)](https://GitHub.com/LanguageMachines/foliautils/releases/) [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)

# FoliAutils

  (c) CLST/TiCC/CLiPS 2019
  https://github.com/LanguageMachines/foliautils

    Centre for Language and Speech Technology, Radboud University Nijmegen
    Tilburg centre for Cognition and Communication, Tilburg University and
    Centre for Dutch Language and Speech, University of Antwerp

  This file is part of foliautils
  foliautils provides a series of programs to make FoLiA processsing more
  easy.
  This includes:
  FoLiA-2text : convert FoLiA documents into plain text
  FoLiA-txt   : convert plain text documents into FoLiA
  FoLiA-page  : convert PAGE documents into FoLiA
  FoLiA-hocr  : convert hocr documents into FoLiA
  FoLiA-alto  : convert ALTO DIDL files into series of FoLiA documents.
  FoLiA-langcat : assign language tags to the words in a FoLiA document.

  FoLiA-idf     : count words in a serie of FoLiA documents and generate
  		  a .tsv files describing the IDF.
  FoLiA-stats   : gather n-gram statistics from series of FoLiA files
  FoLiA-collect : collect n-gram statistics of .tsv files produced by
  		  FoLiA-stats


  FoLiA-correct : correct FoLiA files using correction candidates generated by
  		  TICCL-rank (from the ticcltools package)

  foliautils is free software; you can redistribute it and/or modify
  it under the terms of the GNU General Public License as published by
  the Free Software Foundation; either version 3 of the License, or
  (at your option) any later version.

  Comments and bug-reports are welcome at our issue tracker at
  https://github.com/LanguageMachines/timbl/issues or by mailing
  lamasoftware (at) science.ru.nl.

-----------------------------------------------------------------------

This software has been tested on:
- Intel platforms running several versions of Linux, including Ubuntu, Debian,
  Arch Linux, Fedora (both 32 and 64 bits)
- MAC platform running OS X 10.10


Contents of this distribution:
- Sources
- Licensing information ( COPYING )
- Build system based on GNU Autotools

Dependencies:
To be able to succesfully build libfolia from source, you need the following dependencies:
- ticcutils (https://github.com/LanguageMachines/ticcutils)
- folia (https://github.com/LanguageMachines/folia)
- libicu-dev
- libexttextcat-dev OR libtextcat-dev (OS dependant)
- A sane C++ build environment with autoconf, automake, autoconf-archive, make, gcc or clang, libtool, pkg-config

To install libfolia, first consult whether your distribution's package manager has an up-to-date package.
If not, for easy installation of libfolia and all dependencies, it is included as part of our software
distribution LaMachine: https://proycon.github.io/LaMachine .

To compile and install manually from source, provided you have all the
dependencies installed:

 $ bash bootstrap.sh
 $ ./configure
 $ make
 $ make install
