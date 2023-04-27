#include <iostream>
#include <string>

using namespace std;

int valorletras(string f);

int main()
{
	string frase;
	cout<<"ingrese su frase"<<endl;
	getline(cin,frase);
	cout<<"valor de letras:"<<valorletras(frase);
	
	return 0;
}   
 
 int valorletras(string f)
 {
 int i=0,cont=0;
  for (i=0;i<f.size();i++)
     {
       if (f[i]== 'a' || f[i]== 'A' || f[i]== 'e' || f[i]== 'E' )
 		{
 			cont=cont + 1;			
		 }
		 
     if (f[i]== 'o' || f[i]== 'O' || f[i]== 's' || f[i]== 'S' )
 		{
 			cont+=2;		
		 }
		 
	 if (f[i]== 'd' || f[i]== 'D' || f[i]== 'i' || f[i]== 'I' || f[i]== 'n' || f[i]== 'N' || f[i]== 'r' || f[i]== 'R' )
   		 {
		     cont +=3;
		 }
		 
	if (f[i]== 'c' || f[i]== 'C' || f[i]== 'l' || f[i]== 'L' || f[i]== 't' || f[i]== 'T' || f[i]== 'u' || f[i]== 'U' )
   		 {
		 cont +=4;
		 }
		 
	if (f[i]== 'm' || f[i]== 'M' || f[i]== 'p' || f[i]== 'P' )
 		{
 		     cont+=5;		
		 }
	if (f[i]== 'b' || f[i]== 'B' || f[i]== 'f' || f[i]== 'F' || f[i]== 'g' || f[i]== 'G' || f[i]== 'h' || f[i]== 'H' || f[i]== 'j' || f[i]== 'J' || f[i]== 'q' || f[i]== 'Q' || f[i]== 'v' || f[i]== 'V' || f[i]== 'x' || f[i]== 'X' || f[i]== 'y' || f[i]== 'Y' || f[i]== 'z' || f[i]== 'Z'  )
   		 {
		     cont +=6;
		 }
		 if (f[i]== 'k' || f[i]== 'K' || f[i]== 'w' || f[i]== 'W' )
 		{
 			cont=cont + 7;			
		 }
     }
     
     
     return cont;

}
