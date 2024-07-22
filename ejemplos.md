- 👋 Hi, I’m @wilsonhacker90
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...


*Queremos guardar los nombres y la edades de los alumnos de un curso.
Realiza un programa que introduzca el nombre y la edad de cada alumno. El
proceso de lectura de datos terminará cuando se introduzca como nombre un
asterisco (*) Al finalizar se mostrará los siguientes datos:
· Todos los alumnos mayores de edad.
· Los alumnos mayores (los que tienen más edad) */

#include <iostream>
#include <string.h>
#include <conio.h>

using namespace std;

int main(){
	

	char n;
	
	int       VECT1[5];
	string    VECT2[5];
	                 
	char ast;
	int edadmayor=0;
	string H;
	//llenado de los vectores de con la condicion descrita
			
	string titulos[5];
    string autores[5];
   
   
   
   for(int k = 0; k < 5; k++){
    	cout<<"\n dime las edades";
    	cin>>VECT1[k];
	}
	
	for(int k = 0; k < 5; k++){
    	cout<<"\n edades"<<VECT1[k];
	}
    
    
   
    for(int i = 0; i < 5; i++)
    {
       cout<<"\n dime los nombres";
	   cin>>VECT2[i];
       
       if(VECT2[i]=="*"){
        
	    for(int k = 0; k < 5; k++){
	   	if(VECT1[k]>=18){	
	   		cout<<"los mayores de edad son: "<<VECT1[k];
	   		if(VECT1[k]>edadmayor){
			edadmayor=VECT1[k];
			cout<<"la edad mayor es: "<<edadmayor;   
			}
	   			
		   }
	   	
	   }
	   i=5; //sale del ciclo para no leer mas datos cuando se presiona un asterisco
	   }
       
    }
	
    
}	

