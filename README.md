```
 padding: 0;
    margin: 0px;
    color: #1b2021;
    box-sizing: border-box;
```

*:esto indica que estoy tomando toda la pagina con los requerimientos dentro de los corchetes y el box-sizing evita el desbordamiento en toda la hoja

```
h1{
    font-size: 52px;
    text-align: center;
}
h2{
    text-align: center;
}
```

esto indica que todos los h1 y h2 tendrán esas propiedades, de alineación al centro 

```
.Menu{
    padding: 0px;
}
```

uso esta clase que en el html es un div el cual contiene el nav.

```
nav{
    display: flex;
    justify-content: space-around;
    align-items: flex-end;
}
```

uso en el nav un  flex que me va a yudar para ubicar de mejor forma los elementos que estan en el nav.

```
.navegadores{
    text-decoration: none;
}
.navegadores:hover{
    border: 3px solid #66101F;
}
```

defini clases especiales para agregar detalles en el menú como quitar la linea que acompaña el <a> y el hover para cuando se ubiquen en esta zona cree un borde

```
.logo{
    width: 400px;
    height: 150px;
}
```

esta es la imagen que esta dentro del nav le di una clase para arreglar cosas tales como su tamaño en ancho y largo(altura).

```
.mensaje{
    border: 2px solid black;
    padding: 20px;
    margin: 60px 50px 0 50px;
}
```

uso estas propiedades para darle un borde,una distancia entre el borde y eltexto que puse dentro de el y el margin genera que:

- arriba tenga una distancia de 60px.

- derecha:50px.

- abajo: cero.

- izquierda:50px.

  Realice esto con el fin de que cuando oprima en el nav "catalogo" aparezca solo esta pantalla sin notarse la siguiente que es "Quienes"

```
.divisiones{
    display: grid;
    grid-template: 90% /repeat(4,24%);
    gap: 15px;
    padding: 15px;
}
```

este es el div que contiene la informacion de "Quienes":
grid-template:busca crear una sola fila y 4 columnas de 24%.
gap:distancia entre las columnas.

```
.botoncito{
    display: flex;
    justify-content: center;
} 
```

un div que va a contener mi "button" y lo va a ubicar en el centro de la cajita que crea el div.

despues sigue unos arreglos para "button":

- [ ] **text-decoration: none:** Esta propiedad elimina cualquier decoración de texto
- [ ] **text-transform: uppercase:** Convierte todo el texto del botón a letras mayúsculas.
- [ ] **letter-spacing: 2px**: Aumenta el espacio entre las letras en 2 píxeles.
- [ ] **outline: 2px solid pink:** se usa para un contorno en mi "button"como si fuera un border pero este "outline" no afecta el resto del diseño.
- [ ] **padding: 30px 60px:** el relleno del botón.
- [ ] **position: relative:** posición del botón como relativa
- [ ] **overflow: hidden:** Oculta cualquier contenido que se desborde del área definida por el "button".
- [ ] **transition: color 1s:** Aplica una transición suave de 1 segundo al cambio de color del texto del botón.
- [ ] **button::before:** Crea un pseudo-elemento ::before que se coloca antes del contenido real del botón. Este pseudo-elemento se utiliza para crear un efecto visual adicional.
- [ ] **content: '':** Establece el contenido del pseudo-elemento como vacío.
- [ ] **position: absolute:** Posiciona el pseudo-elemento absolutamente con respecto al contenedor principal (el botón en este caso).
- [ ] **top: 0; left: -50px:** Coloca el pseudo-elemento en la parte superior del botón y lo desplaza 50 píxeles hacia la izquierda.
- [ ] **width: 0; height: 100%:** Inicialmente, el pseudo-elemento tiene un ancho de 0 y una altura del 100%, por lo que no es visible.
- [ ] **transform: skewX(35deg):**Hace que la rayita mientras se llena "button" sea inclinada
- [ ] **z-index: index -1:** Establece el índice Z del pseudo-elemento en -1, lo que lo coloca detrás del contenido real del botón.
- [ ] **transition: width 1s:** Aplica una transición suave de 1 segundo al cambio de ancho del pseudo-elemento. Cuando cambie el ancho, la transición se realizará de manera gradual durante 1 segundo.
- [ ] **button:hover::before:**  Cuando el mouse está sobre el botón, el ancho del pseudo-elemento cambia a 150%, creando un efecto visual.

```
.producto{
    padding: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
}
```

Este es el div que contiene la imagen principal y hago que lo que hay dentro del div este centrado.

```
.referencia{
    width: 1000px;
}
.referencia:hover{
    filter: opacity(0.6);
    transform: scale(1.1);
}
```

**.referencia:**es la imagen que siempre tendra un tamaño de 1000px y cuando el mouse este sobre la foto se vaya hacia afuera con cierta opacidad.

```
.ejemplos{
    display: grid;
    border: 3px solid black;
    grid-template: 80%/repeat(3,20%);
    gap: 20%;
    padding: 30px;
    margin: 50px;
}

```

es el div que tendrá el "catalogo" y tiene como características una fila  de 80%  y tiene 3 columnas de 20%

```
.examples{
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0px;
}
```

es la información dentro de "ejemplos" son divs dentro de un div principal, alineados al centro y sin distancia entre borde y contenido

```
.imagenes{
    width: 300px;
    height: 200px;
    border: 3px solid #739072;
}
.imagenes:hover{
    filter: opacity(0.6);
    transform: scale(0.8);
}
```

son las imagenes dentro de "examples" y las dispongo todas de un mismo tamaño y que cuando se paren en ellas estas imagenes cambian de tamaño a una escala mas pequeña y con opacidad

```
.redes{
    display: flex;
    align-items: center;
    justify-content: center;
}
```

contenedor del "contactenos" asegurando la posición de los logos en el div.En html no solo aparece el icono cuando oprimes en el te redirecciona a otra pestaña con la pagina social

```
.contactos{
    margin-top:100px ;
}
```

distancia entre la pagina de arriba y la de contáctenos.

he creado nuevos html que contendrán la descripción de el producto que esta en el catalogo de la pagina principal. Las determiné a todas con la misma estructura y bajo un solo css que me regularlos 6 productos

**background: drop-shadow(#faecf2)**
esta función hace que  el fondo de la imagen tome el color seleccionado.

**overflow: hidden**;evita el desbordamiento osea que se salgan de los limites

```
.checkbtn{
        display: block;
    }
    ul{
        position: fixed;
        width: 100%;
        height: 30vh;
        top: 150px;
        left: -100%;
        text-align: center;
        transition: all .5s;
        background:#fdcae1;
    }
    nav ul li{
        display: block;
        margin: 50px 0;
        line-height: 30px;
    }
    nav ul li{
        font-size: 20px
    }
    li a.hover{
        background: none;
        color: red;
    }
    #check:checked ~ ul{
        left: 0;
    }
```

**.checkbtn** se utiliza para un tipo de botón para que el usuario puede hacer clic para abrir el menú.
**#check:checked ~ ul**: indica que cuando el elemento con el ID "check" está marcado

**position: fixed** lo fija en la pantalla.
**width: 100%** toma todo el ancho de la pantalla.
**height: 30vh** establece la altura en el 30% del alto de la ventana.
**top: 150px** lo coloca a 150 píxeles desde la parte superior.
**left: -100%** lo coloca fuera de la pantalla inicialmente.
**text-align:** center centra el contenido del menú.
**transition: all .5s** aplica una transición de medio segundo a todas las propiedades CSS.
**background:#fdcae1** establece un color de fondo.

Aplica estilos a los elementos de la lista dentro del menú.
**display: block** establece que cada elemento de la lista debe mostrarse como un bloque.
**margin: 50px 0** establece un margen superior e inferior de 50 píxeles.
**line-height: 30px** establece la altura de línea.

# PARA MEJOR VISUALIZACION USAR EL RESPOSIVE 768*812

