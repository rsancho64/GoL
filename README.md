# The Conway's Game of Life (GoL: el juego de la vida de Conway)

El juego de la vida es un automata celular creado por John H. Conway en 1970. Es un juego de 0 jugadores (lo empiezas y sigue solo) es decir: una configuracion inicial 2D es el comienzo del resto de la historia.

Esta implementación (programacion del juego) usa python 3.5 y se renderiza en terminal (es una aplicación CLI)

## Reglas

Las siguientes 4 reglas son la lógica de la evolucion del tablero, que termina -junto al juego- en una situacion estática, o con todas las celulas muertas (vacias) o en un caso intermedio, cuando solo hay osciladores -o naves- estables.

1. _**despoblacion**_ - Si una celula viva está rodeada por menos de dos vecinos igualmente vivos, muere de soledad -no pasa a la siguiente generacion-.
2. _**equilibrio**_ - Si una celula viva está rodeada por dos o tres vecinos igualmente vivos, se mantiene viva -pasa a la siguiente generacion-.
4. _**sobrepoblacion**_ - Si una celula viva está rodeada por mas de tres vecinos igualmente vivos, muere de agobio -no pasa a la siguiente generacion-.
7. _**reproduccion**_ - Si una celula muerta está rodeada por tres vecinas vivas, revive -aparece viva en la  siguiente generacion-.

## How to Run

Solo hace falta Python 3.5+ instalado. [ver aqui](https://www.python.org/downloads/).

Para iniciar se puede abrir una terminal/consola (el CLI) y navegar a la carpeta del ejecutable -`/source`- y una vez dentro ejecutar el comando **`python main.py`** para iniciar el programa/juego. Una vez iniciado, se idican las dimensiones del tablero en las dos entradas siguientes: input the number of **rows** and **columns** 

