# Math-Funtion-C
This project handles the mathematical function of the division, to be implemented in a standard calculator

 We are going to know the mathematical function of the division, 
 for which we are asked for a dividend and a divisor.
 Including a library at the top of the project, 
 called <math.h>, which brings a list of functions that allows us 
 to access more quickly.
 
 ```
 #include <stdio.h>
 #include <stdlib.h>
 #include <math.h>
 
 
int main()
{
    /**
    *   \mainpage Practice Division-Funtion
    *   \author Johan Martinez
    *   \date June 2019
    */

    /**
    *   In this program it is for the mathematical function of the division,
    *   the implementation can be given with a standard calculator
    */

    /** For this two variables are created that are the dividend and the divisor */
    double dividendo, divisor;
    /** Give a message to enter the values and then
    *   move to save it in their respective variables
    */
    printf("Ingrese el dividendo: \n");
    scanf("%lf", &dividendo);
    printf("Ingrese el divisor: \n");
    scanf("%lf", &divisor);

    /** Ask if the divisor is 0 */
    if(divisor == 0){
            /** If it is, it prints a message   */
        printf("No se puede dividir entre 0. No existe");
    } else {
        /** If not, do the procedure together with the fmod function
        *   fmod is an instance of the library <math.h>
        */
        printf("El resultado es: ",dividendo,divisor,fmod(dividendo,divisor));
    }
    system ("pause");
    return 0;
}
 ```
 
 
