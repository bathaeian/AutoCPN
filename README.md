# AutoCPN
A java class for building Colored Petri Nets
Colored Petri nets are extended definitions of ordinary Petri nets that allow places have
different types of tokens.
CPN Tools is a tool for editing, simulating, and analyzing Colored Petri nets
By adding these 2 files, a programmer can make a .cpn file that can be analysed by CPN Tools.
API functions:
public void addPlace(String s) : adding place with the id of s
public void addTrans(String s) : adding transition with the id of s
public void addArc(Boolean orientation, String transendID, String placeendID, String annotText) : adding arc
          //orientation==> true:TtoP   false:PtoT
public void addVar(String ty, String i) : adding variable with type of ty and name of i
public void writeCPN(OutputStream output) throws IOException : writing the cpn file out.cpn
