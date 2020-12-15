# msa: An R Package for Multiple Sequence Alignment
The 'msa' package provides a unified R/Bioconductor interface to
the multiple sequence alignment algorithms ClustalW, ClustalOmega,
and Muscle. All three algorithms are integrated in the package,
therefore, they do not depend on any external software tools
and are available for all major platforms. The multiple sequence
alignment algorithms are complemented by a function for
pretty-printing multiple sequence alignments using the LaTeX
package TeXshade.

This is the source code repository. The package can be installed from
[Bioconductor](https://bioconductor.org/packages/release/bioc/html/msa.html).
Further information and installation instructions are also available from
http://www.bioinf.jku.at/software/msa/.

Although the package is maintained by Ulrich Bodenhofer, the package itself
has been implemented mainly by Enrico Bonatesta and Christoph Kainrath-Horejs.

# Modifications
I experimented some issues whilst trying to use the `msa::clustalw` function inside of
a parallel nested loop.

Small modifications found here implemented by Gustavo Magaña López, who claims
no ownership of this package.

# Caveats 

Compiling this package needs a **gcc** version lower than 10. 

I have achieved it using gcc-9 on Pop!\_OS.

```bash
gcc --version 
gcc (Ubuntu 9.3.0-18ubuntu1) 9.3.0
Copyright (C) 2019 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```

