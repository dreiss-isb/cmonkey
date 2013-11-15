If you came here looking for the cMonkey R package, you can now grab it here.

#https://github.com/dreiss-isb/cmonkey/blob/master/cMonkey_4.9.10.tar.gz?raw=true

To install (in R):

```
install.packages('devtools', dep=T)
require(devtools)
install_github('cmonkey', 'dreiss-isb', subdir='cMonkey')
```

To install the data (or bigdata) packages:

```
install_github('cmonkey', 'dreiss-isb', subdir='cMonkey.data')
install_github('cmonkey', 'dreiss-isb', subdir='cMonkey.bigdata')
```

... and then go here 

http://baliga.systemsbiology.net/cmonkey 

to see some minimal documentation.

<!--
If you want to run cMonkey from raw R code, you've come to the right place. Once you've cloned your copy, you can run cMonkey locally (without the package), after doing the following (in R, of course):

```python
source( "cmonkey.R" )    ## This should be all you need
## source( "cmonkey-init.R" )
## source( "cmonkey-data-load.R" ) ## Functions for loading the data
## source( "cmonkey-motif.R" ) ## Functions for motif finding/scoring
## source( "cmonkey-plotting.R" ) ## Functions for all cmonkey plotting
## source( "cmonkey-postproc.R" ) ## Functions for all post-processing and analysis of cmonkey clusters
## source( "cmonkey-bigmem.R" ) ## Functions for using on-disk list and matrix storage for big organisms

## This is only necessary if you don't have the 'progs/' dir in your current dir (and will only work if
##     you have previously installed the cMonkey package):
progs.dir <- sprintf( "%s/progs/", system.file( package="cMonkey" ) )

cmonkey( ... ) ## run as you would if you had loaded the cMonkey package

## or:

e <- cMonkey.init(...); cmonkey( e, ..., dont.init=T )

## will work as well.
```

Visit http://cmonkey.systemsbiology.net/ for more useful instructions on actually using the code for your organism.
-->

