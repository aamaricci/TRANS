## _TRANS_
### transform data files

*(c) Adriano Amaricci (-2015) [from an original work of Kristjan Haule (2011)]*

Version 0.3 [17.Aug.2015]

### trans [options] [trans operations] [file/stdin]

#### Options:
  - `-k=; --key=`   [column prefix, (default=#)  (allowed=#,%,$,_,@) ]
  - `-c=; --cmt=`   [comment character (default=#)]
  - `-l=; --lines=`  [select specific line(s) to plot, single or first:last]
  - `-b; -wl; --with-line=`   [print line number as first column]
  - `-lf=; --legend-file=`   [specify legend file (default=trans.info)]

#### Usage:
[... | ] **trans** *[options]* [file_index:]function(column1) [file1 file2 ...]

` $ cat file | trans #1 #3-#2 'tan(#4)'`

` $ trans co1, #2-#1, #3/#1 file1 file2`

*note: check your shell passes special characters to trans! characters like \,$,# need a double-quote or preceding slash!!*
