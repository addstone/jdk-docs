JDK 1.1 Beta $B$N%$%s%9%H!<%k%G%#%l%/%H%j(B docs/guide/rmi/examples/stock 
$B$K%"%W%l%C%H$N:n$jJ}$r<($9NcBj$,$"$j$^$9!#$3$N%"%W%l%C%H$O%j%b!<%H%*%V(B
$B%8%'%/%H$r%(%/%9%]!<%H$7$F%9%H%C%/%5!<%P!<$+$i$NJQF0$9$k3t2A$r<u$1<h$j(B
$B$^$9!#%"%W%l%C%H$O%5!<%P!<$+$i$NDLCN$r<u$1<h$k$?$S$K3t2A$rF0E*$KI=<($7(B
$B$^$9!#$3$NNcBj$G;H$&%$%s%?%U%'!<%9(B/$B%/%i%9$O<!$NDL$j$G$9!#(B 

   - StockWatch $B$O%9%H%C%/%5!<%P!<$N$?$a$N%j%b!<%H%$%s%?%U%'!<%9$G$9!#(B 

   - StockNotify $B$O%9%H%C%/%*%V%6!<%P!<$N$?$a$N%j%b!<%H%$%s%?%U%'!<%9$G$9!#(B 

   - Stock $B$O3t2A%G!<%?$rJ];}$9$kD>Ns2=2DG=$J%*%V%8%'%/%H$G$9!#(B 

   - StockServer (StockWatch$B$r<BAu(B) $B$OCM$r<u$1<h$k$h$&$K@_Dj$5$l$?%j%b!<(B
     $B%H%*%V%8%'%/%H$K3t2AJQF0$rDLCN$7$^$9!#(B 

   - StockApplet (StockNotify$B$r<BAu(B) $B$O%j%b!<%H%*%V%8%'%/%H!J<+J,<+?H!K(B
     $B$r%(%/%9%]!<%H$7!"(BStockServer $B$X3t2AJQF0$NDLCN$rEPO?$7!"3t2AJQF0(B
     $BDLCN$r<u$1<h$k$H$=$l$rI=<($7$^$9!#(B 

Solaris $B$N>l9g!'(BJDK 1.1 Beta $B%j%j!<%9$r%@%&%s%m!<%I$7!"(B
docs/guide/rmi/examples/stock $B%G%#%l%/%H%j$K$"$k(B run $B%9%/%j%W%H$r<B9T(B
$B$7$^$9!#(B $B$3$N%9%/%j%W%H$ONcBj<B9TCf$K$=$N<B9TFbMF$r%W%j%s%H$7$^$9!#%9(B
$B%H%C%/%5!<%P!<$O<+J,$N%l%8%9%H%j$r:n@.$7$^$9$+$i(B "rmiregistry" $B$r%9%?!<(B
$B%H$5$;$kI,MW$O$"$j$^$;$s!#(B run $B%9%/%j%W%H$O4pK\E*$K<!$N%9%F%C%W$r<B9T(B
$B$7$^$9!#(B 

setenv CLASSPATH ../..:$CLASSPATH
javac -d ../.. *.java
rmic -d ../.. examples.stock.StockServer examples.stock.StockApplet
java examples.stock.StockServer &
appletviewer index.html 

$BCm0U(B: Appletviewer $B$r<B9T$9$kA0$K(B CLASSPATH $B$r85$NFbMF$K!J(B../..$B$r4^$a(B
$B$:$K!KLa$7$F$+$^$$$^$;$s!#$3$&$7$F$*$/$H%/%i%9$O(B CLASSPATH $B$+$i$G$O$J(B
$B$/%M%C%H%o!<%/$+$i%@%&%s%m!<%I$5$l$^$9!#(B 

Windows $B%7%9%F%`$N>l9g!'(BJDK 1.1 Beta $B%j%j!<%9$r%@%&%s%m!<%I$7(B,
docs/guide/rmi/examples/stock $B%G%#%l%/%H%j$K0\F0$7$F(B run.bat $B$r<B9T$7(B
$B$^$9!#NcBj$N%S%k%I$H<B9TCf$O3F%9%F%C%W$N@bL@$,I=<($5$l$^$9!#=*N;$7$^$7(B
$B$?$i%5!<%P!<%W%m%;%9$N$?$a$K:n$i$l$?%&%#%s%I%&$r>C$7$F$/$@$5$$!#(B 
