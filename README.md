# PRUEBA-INDIVIDUAL-RA2---HTML-CSS

## Ejercicio 1

### 1A. Pregunta
**¿Por qué NO se centra el texto del <h1> en este caso? Explícalo con tus palabras. (por qué visual y estructuralmente no aparece centrado entre el borde izquierdo y el menú)**
Visualmente, el texto no se centra porque con el "justify-content: space-between" el <h1> queda fijo en la izquierda y el <nav> a la derecha. Y estrucuralmente no se centra porque el "text-align" del <h1> solo afecta al texto en sí, no a todo.

### 1B. Ejercicio - Soluciona de dos formas diferentes
Con Flexbox se puede resolver alineando el texto en el centro con un "align-items" y añadiendo un padding, luego con un "margin: 0 auto", se eliminará el espacio que hubiera quedando centrado. Tal que así:
.site-header {
  display: flex;
  align-items: center;
  padding: 10px 16px;
}

.site-header h1 {
  margin: 0 auto;
  text-align: center;
}

### 1C. Ejercicio – Convertir la cabecera en dos filas
Añadimos un "flex-direction: column" para que el <h1> y el <nav> se posicionen uno sobre el otro y agregamos un gap de 30px para separarlos. Luego añado un "margin: 0" al <nav> para que se centre. Quedaría así:
.site-header {
    display: flex;
    align-items: center;
    flex-direction: column;
    padding: 10px 16px;
    gap: 30px; 
}

.site-header h1 {
    margin: 0;
    text-align: center;
}

.site-header .main-nav{
    margin: 0;
}

### 1D. Ejercicio – Dar relieve y separación visual al header
Aplicaria un background-color y un border-bottom.  
