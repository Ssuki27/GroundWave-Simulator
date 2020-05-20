# GroundWave-Simulator
Ejecutable del simulador GroundWave Simulator para la determinación y representación de la intensidad de campo eléctrico recibido por onda de superficie para frecuencias entre 10 kHz y 30 MHz según la Rec. ITU-R P.368-9

                       Ground Wave Simulator

                    	Manual de Usuario

                        Javier Ojeda Prieto

                         Sevilla, 2020

------------------------------------------------------------------
			    INSTALACIÓN

Ubicar la carpeta descomprimida GWSim en Disco Local (C:), de 
manera que la ubicación quede: C:\GWSim
Abrir ejecutable GroundWave Simulator

Solo disponible para Windows.

------------------------------------------------------------------
				USO

El simulador basa sus datos en llamadas al programa GRWAVE escrito
en código Fortran. Para interpretar este código es necesario 
ejecutarlo en entorno MS-DOS. En algunos ordenadores funciona 
utilizando el terminal de Windows, y en otros es necesario el uso
de un emulador de MS-DOS (por ejemplo, DOSBox, ya incluido). Esto 
se podrá escoger en la primera interfaz de bienvenida y solo 
variará cómo se realizan las llamadas a GRWAVE. En MS-DOS los 
cálculos tardan más tiempo, pues se llama a GRWAVE numerosas veces
y el proceso de abrir el emulador automáticamente es lento.

Dentro del simulador existen dos escenarios a simular:

	- Terreno homogéneo: las características eléctricas del
	  suelo no varían a lo largo de la transmisión. Será
	  posible ejecutar para diversas frecuencias a la vez,
	  para comparar visualmente.
	  Solo es posible obtener la intensidad de campo eléctrico
	  en función de un valor de distancia cuando únicamente se
	  ha ejecutado una frecuencia.

	- Terreno mixto: la características del terreno varían
	  hasta 4 veces a lo largo de la transmisión. Es necesario
	  especificar la longitud de cada terreno, que será
	  utilizada para el cálculo de intensidad de campo recibida.
	  Los cálculos siguen el Método de Millington.

El rango de frecuencias permitido va desde los 10 kHz hasta 30 MHz.
Para la selección de terrenos, se han incluido algunos valores
predeterminados. Si se desea introducir manualmente, escoja la
opción Personalizado.

Las variables introducidas deben ser formato float.
Ejemplo: 26.15

Para información sobre los métodos utilizados para desarrollar el
simulador, véase la Rec. ITU-R P.368-9:
https://www.itu.int/rec/R-REC-P.368/es

Para información sobre las características eléctricas de los
terrenos predeterminados, en especial para Hielo de agua dulce,
véase la figura 17 de la Rec. ITU-R P.527-5:
https://www.itu.int/rec/R-REC-P.527-5-201908-I/es

Para cualquier duda o problema se adjunta la siguiente dirección
de correo electrónico: javojepri@alum.us.es
