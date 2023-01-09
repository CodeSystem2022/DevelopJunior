# DevelopJunior
Programando varios lenguajes, creando varios proyectos y ejercicios
	
	                   .  .            
	                   |\_|\           
	                   | a_a\          
	                   | | ´]           
	               ____| ´-\___         
	              /.----.___.-´\                               
	             //        _    \                               
	            //   .-. (~v~) /|
	           |´|  /\:  .--  / \
	          // |-/  \_/____/\/~|
	         |/  \ |  []_|_|_] \ |       c^>            c^>             c^>           c^>
	         | \  | \ |___   _\ ]_}
	         | |  ´-´ /   ´.´  |
	         | |     /    /|:  |
	         | |     |   / |:  /\
	         | |     /  /  |  /  \
	         | |    |  /  /  |    \
	         \ |    |/\/  |/|/\    \
	          \|\ |\|  |  | / /\/\__\
	           \ \| | /   | |__
	                / |   |____)
	               |_/
<h1>Construyendo algoritmos utiles en JavaScript</h1>
</br>
Este código crea una escena de Three.js con una cámara perspectiva y un conjunto de partículas que se mueven alrededor del cursor del mouse. También hay dos animaciones en loop en el código, una que hace que el conjunto de partículas se escale de manera periódica y otra que hace que gire en torno a sus ejes x e y.
</br>

Ver la ejecución desde AQUÍ: (https://codesystem2022.github.io/DevelopJunior/)
</br>
</br>
Aquí está la descripción completa del código:

El código comienza creando una escena y una cámara en Three.js, y luego agrega un controlador de eventos para el evento "mousemove" al documento. Cuando se produce este evento, se llama a la función onMouseMove(). Además, se crea un renderizador WebGL y se establece su tamaño en el ancho y alto de la ventana del navegador, y se agrega el elemento <canvas> del renderizador al cuerpo del documento HTML. También se agrega un controlador de eventos para el evento "resize" de la ventana. Cuando se produce este evento, se ajusta la relación de aspecto de la cámara y el tamaño del renderizador al ancho y alto de la ventana.

Luego, se crea una geometría vacía y se llena con 1600 vectores aleatorios con coordenadas basadas en valores aleatorios de theta y phi. A continuación, se crea un conjunto de partículas a partir de esta geometría y un material de puntos con un color rosa claro y un tamaño de 2. La esfera de colisión del conjunto de partículas se establece en 50.

Se crean dos grupos vacíos y se añaden el conjunto de partículas y el primer grupo al segundo. Finalmente, se añade el último grupo a la escena y se establece la posición z de la cámara en 400.

La función animate() se llama a sí misma utilizando requestAnimationFrame() y renderiza la escena utilizando la cámara. La función onMouseMove() se utiliza para cambiar la rotación del conjunto de partículas en el eje x y y basándose en la posición del cursor del mouse. También se utiliza la biblioteca GSAP para crear dos animaciones que cambian la escala y la rotación del último grupo en el ciclo.
