/* 
Practica 7                                   Hernandez Sanchez Valeria Danaee
fecha de entrega: 22 de noviembre de 2020
*/

//seccion de librerias
#include <conio.h>
#include <stdio.h>
//Declaracion de funciones
int main()
{
	//Declaracion de variables
	/*Variables usadas para contar puntos del marton messier*/
    int loc, des, dib, m ;
    float h=0.254;
    char cat='M';
    
    /*Bloque de instrucciones*/
    
    //Bloque para contar los puntos por objeto messier
    printf("\n\n\t Categoria del concuarsante: %c \n\n", cat);
    printf( "\n   Introduce los puntos por localizacion: \t " );
    scanf( "%d", &loc );

    printf( "\n   Introduce los puntos por descripcion:\t" );
    scanf( "%d", &des );
    
    printf( "\n   Introduce los puntos por el dibujo:\t\t" );
    scanf( "%d", &dib );
    
    //Bloque para mostrar y calcular el puntaje total
    printf( "\n\n\n  Los puntos acumulados por este objeto son : %d", loc + des + dib);
    printf( "\n\n \t\t  El avance hasta ahora es de : %d \n\n", (loc + des + dib) / 3 );
    printf("\t\t\t\t Region abarcada: %f \n\n", loc * h);
 
    //Bloque para saber cuantos objetos le faltan al concursante 
    printf( "\n\v\r \f\f  Escribe la cantidad de objetos que se llevan observados:  " );
    scanf( "%d", &m );
    
    printf( "\n\t\t\f\f\a\b Cantidad de objetos que faltan por observar: %d \n\n", 110 - m );
    return 0;
}
