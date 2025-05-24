Comandos básicos de netlogo
En el cuadro de Command Center - Observer>

PRIMER ELEMENTO CENTRAL DE NETLOGO- TORTUGAS.
  Elemento central de Netlogo es una TORTUGA
  create-turtles 1 #Crea tortugas
  ask turtles [forward 10] #Se le solicita a las tortugas moverse 10 pasos adelante.
  ask turtles [back 10]    ##Se le solicita a las tortugas moverse 10 pasos hacia atrás.
  ask turtles [right 90]   # que se mueva a la derecha 90 grados
  ask turtles [ left 180 ] # que se mueva a la izqueirda 180 grados
  ask turtles [set size 5 ] #que su tamaño sea 5
  ask turtles [ set shape "turtle"] #que su forma sea una tortuga.
  ask turtles [ set color blue ] 
  ask turtles [ set xcor 10]     #que se mueva 10 pasos a su coordenada x a la derecha.
  ask turtles [ set ycor 10 ]    #que se mueva 10 pasos a la coordenada y positivo.
  ask turtles [ pen-down ]      #bajar la pluma para ver su trazo.
  clear-all                #elimina todo lo anterior.
  create-turtles 50       #crea 50 tortugas en el centro.
  ask turtles [ setxy random-xcor random-ycor ]   #posiciones aleatorias en x,y
  ask turtles [ pen-down ]
  ask turtles [ forward 5 right 90 forward 5]
Flechita hacia arriba vuelvo a reproducir el comando.
  clear-drawing          #borrar los caminos del pen-down
  ask turtles [ die ]   # se mueren las tortugas
_____
Dibujo de cuadro
  create-turtles 1
  ask turtles [ pen-down ]
  ask turtles [repeat 4 [forward 5 right 90]]  # dibujar un cuadrado
Dibujar una estrellita
  ask turtles [repeat 10 [ forward 5 right 160]] 
Dibujar un circulo con estrellas.
  ask turtles [ repeat 5 [forward 4 right 30 repeat 4 [forward 5 160]]]

SEGUNDO ELEMENTO CENTRAL DE NETLOGO - PARCHES

  ask patches [ set pcolor yellow ] #pintar todos los parches con color amarillo
  ask patches with [ pxcor = 0 ][set pcolor blue]  #pintar los parches con coordenada x=0 los pinte azul
  ask patches with [ pycor = 0 ] [ set pcolor blue ] pintar parches coordenada y =0 azul
  create-turtles 100 
  ask turtles [setxy random-xcor random-ycor]
  ask turtles [set pcolor color]   #se le pide a las tortugas que cambien el color del parche al color que tienen
  ask patches [ set pcolor white ]
  ask turtles [ facexy 0 0 ]
  VER EL MODELO DE SEGREGACIÓN SIMPLE
  VER EL MODELO DE VOTING COMPONENT VERIFICATION

