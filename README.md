# PRUEBA-INDIVIDUAL-RA2---HTML-CSS

## Ejercicio 1

### 1A. Pregunta
**¿Por qué NO se centra el texto del h1 en este caso? Explícalo con tus palabras. (por qué visual y estructuralmente no aparece centrado entre el borde izquierdo y el menú)**
Visualmente, el texto no se centra porque con el "justify-content: space-between" el h1 queda fijo en la izquierda y el nav a la derecha. Y estrucuralmente no se centra porque el "text-align" del h1 solo afecta al texto en sí, no a todo.

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
Añadimos un "flex-direction: column" para que el h1 y el nav se posicionen uno sobre el otro y agregamos un gap de 30px para separarlos. Luego añado un "margin: 0" al nav para que se centre. Quedaría así:
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

### 4. - Informe de evidencias del proyecto (Defensa técnica simple)
## 4.1 Introducción
El tema de mi web es el Taekwondo WTF. He incluido, una breve bienvenida a la página, además de una galería de imagenes en las que trato de mostrar las cosas mas representativas de este deporte; también he añadido una tabla donde incluyo todos los grados de cinturón que existen, el tiempo que hay que llevarlos para poder ascender al siguiente grado y la edad mínima que se debe tener para obtener cada cinturón; un pequeño cuestionario donde se pregunta por el nivel del usuario, formas de contactar con la federación de Taekwondo WTF y mi experiencia personal como practicante de este deporte desde hace más de 8 años. La idea de diseño era hacer un diseño simple, sin mucha carga visual, con colores poco llamativos. 
## 4.2 Evidencias de HTML5
<img width="731" height="327" alt="image" src="https://github.com/user-attachments/assets/66e7c70d-534e-4585-8cbd-559fdae0d0ea" />

>Header


<img width="729" height="547" alt="image" src="https://github.com/user-attachments/assets/f7fa725d-43de-45da-b423-277c9bcbd4d6" />

>Main y Section


<img width="731" height="108" alt="image" src="https://github.com/user-attachments/assets/246f782c-dd6c-4143-baaf-7f1074bf8feb" />

>Footer


---

<img width="735" height="250" alt="image" src="https://github.com/user-attachments/assets/a8d48e17-2641-413d-9e64-6b40ebc45d63" />

>Menú superior


<img width="727" height="284" alt="image" src="https://github.com/user-attachments/assets/1fdb6d3d-505f-4c2c-b1ca-51ea5c4a413c" />

>Menú lateral


---

<img width="730" height="160" alt="image" src="https://github.com/user-attachments/assets/8391cf48-8a17-49d7-b4f8-0851ee16670a" />

>Seccion Hero


<img width="728" height="264" alt="image" src="https://github.com/user-attachments/assets/b4e2016b-bd45-45d4-a169-1b2da524f13e" />

>Seccion Galeria


<img width="749" height="902" alt="image" src="https://github.com/user-attachments/assets/25e867b2-568f-4376-be4a-8e2d9cbc4173" />


>Sección Clasificación (Tabla)


<img width="731" height="430" alt="image" src="https://github.com/user-attachments/assets/f163a45b-b3ce-4153-a694-38cdb7302150" />

>Seccion Formulario

---

## 4.3 Evidencias de CSS
He empleado selectoresde tipo, de clase, descendente... También he empleado pseudoclases, Flexbox, sombras... 

<img width="60" height="29" alt="image" src="https://github.com/user-attachments/assets/25dab07e-b0ae-4403-af78-4f82a08a89ce" />

>Selector de tipo


<img width="123" height="25" alt="image" src="https://github.com/user-attachments/assets/2fde762c-d110-40b3-adca-a1b7f2d0c4c3" />

>Selector de clase


<img width="121" height="26" alt="image" src="https://github.com/user-attachments/assets/b948dce4-57b2-4172-95b2-342c73cc4533" />

>Selector descendente


<img width="157" height="29" alt="image" src="https://github.com/user-attachments/assets/e9556cee-d96d-412c-b281-0d1d6615241f" />

>Pseudoclase


<img width="248" height="61" alt="image" src="https://github.com/user-attachments/assets/4e9449be-bfc1-447c-8e52-f7d53fcb5449" />

>Flexbox


<img width="229" height="164" alt="image" src="https://github.com/user-attachments/assets/01078982-94cc-43ed-8004-aa4d6d54153b" />

>Sombra

---

## 4.5 Menú lateral: breve explicación
Al pulsar el boton se despliega un menú lateral con el índice de la página con enlace a los respectivos puntos. Cambia la clase "open-menu", que se activa haciendo que el menú aparezca. El menu se encuentra oculto fuera de la pantalla con un "left: -230px". Al activarse el menu, la posicion pasa a "left: 0px" con una transicion "transition: left 0.3s ease".
## 4.6 Conclusión personal
He aprendido a crear una página web partiendo de una pequeña base, realizando tanto el codigo en HTML como el CSS para que visualmente se vea atractiva.
Podría mejorar ciertas cosas de la página, que le darían un toque más profesional, como por ejemplo que el menú lateral fuese algo más llamativo, o las imagenes estuviesen ordenadas de una forma más profesional. 
Lo que mas me ha costado ha sido la tabla, porque era muy repetitiva y enredada.
La parte de mi web que mas me gusta, es la parte en la que cuanto mi experiencia porque me hace recordar los buenos momentos que me ha dado este deporte.
