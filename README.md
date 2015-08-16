##TRANS
#transform data files
#Copyright        Kristjan Haule
#Version 2.1            22.9.2011 
#modified  by Adriano Amaricci 2013-15

 trans [options] [file/stdin]

#Options:   -k=C; --key=C [default=#, allowed=#,%,$,_,@]

#Usage: 
 [... |] trans f1(C1, C2, ...), [f2(C1, C2, ...)] [file1 file2 ...]

 cat file | trans C1 C3-C2 'tan(C4)'

 trans C1, C2-C1, C3/C1 file1

#note: check your shell passes special characters to trans!
      characters like \,$,# need a double-quote or preceding slash!!

