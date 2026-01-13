# Area-Calculating-In-Java
# WAP using class Rectangle and calculate area using method

importjava.util.*;
classMyProgram{
publicstaticvoidmain(String[]args){
Rectangler1=newRectangle();
Scannersc=newScanner(System.in);
System.out.print("enterheight:");
r1.height=sc.nextFloat();
System.out.print("enterwidth:");
r1.width=sc.nextFloat();
r1.calArea();
}
}
classRectangle{
floatheight;
floatwidth;
publicvoidcalArea()
{
System.out.println( "Area="+height*width);
}
}
