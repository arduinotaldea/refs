# refs

Common references

## Acher

Prototipo de sistema de control de matrices de LEDs basado en el microcontrolador Atmega48

 - **Acher.pdf** memoria que describe la aplicación en el PC (basada en Labview), la transimisión (UART), y la programación del microcontrolador
 - **Prototipo/** fotografías del montaje
 - **Fuentes**/
   - **atmega48/** código fuente en C
   - **images/** esquemas
   - **labview/** aplicación en VI
   - **latex/** contenido de la memoria en LaTeX
 
## PID_TimerOne

Ejemplo de integración de las librerías PID y TimerOne con el modo sleep. Se genera una señal de referencia (senoidal, triangular o cuadrada) que se compara con una entrada analógica correspondiente a la lectura de posición de un motor, obteniendo una medida de error. Se utiliza el PID para regular una salida PWM y reducir el error a, idealmente, cero. El modo sleep, junto con el timer, permiten ahorrar en consumo actuando únicamente cuando es necesario realizar cálculos. En cada iteración, se envían los valores de entrada/salida a través del puerto serie.

 - **sketch_tanqueolas.ino** código fuente para Arduino
 - **libraries.7z** librerías utilizadas en el sketch
 - **graph_matlab.m** script de Matlab para graficar la información recibida a través del puerto serie
