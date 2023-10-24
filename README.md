# SemanaTec2
# Nombre: Emilio Rizo de la Mora
# Matricula: A01721612
# Carrera: IRS
# Semestre: 5o
## Practica de Github

# Comentario de Erick Schiller

**Bold Semana Tec 12**
*Italic*
---
1. Hot-cakes 🥞
2. Tacos Barbacha 🌮
3. Chilaquiles 🌮

---
- Piano 🎹
- Guitarra 🎸
- Bajo 🎸
- Violín 🎻
---
``` python
"""Paint, for drawing shapes.

Exercises

1. Add a color.
2. Complete circle.
3. Complete rectangle.
4. Complete triangle.
5. Add width parameter.
"""

from turtle import *

from freegames import vector


def line(start, end):
    """Draw line from start to end."""
    up()
    goto(start.x, start.y)
    down()
    goto(end.x, end.y)


def square(start, end):
    """Draw square from start to end."""
    up()
    goto(start.x, start.y)
    down()
    begin_fill()

    for count in range(4):
        forward(end.x - start.x)
        left(90)

    end_fill()


def circle(start, end):
    """Draw circle from start to end."""
    pass  # TODO


def rectangle(start, end):
    """Draw rectangle from start to end."""
    pass  # TODO


def triangle(start, end):
    """Draw triangle from start to end."""
    pass  # TODO


def tap(x, y):
    """Store starting point or draw shape."""
    start = state['start']

    if start is None:
        state['start'] = vector(x, y)
    else:
        shape = state['shape']
        end = vector(x, y)
        shape(start, end)
        state['start'] = None


def store(key, value):
    """Store value in state at key."""
    state[key] = value


state = {'start': None, 'shape': line}
setup(420, 420, 370, 0)
onscreenclick(tap)
listen()
onkey(undo, 'u')
onkey(lambda: color('black'), 'K')
onkey(lambda: color('white'), 'W')
onkey(lambda: color('green'), 'G')
onkey(lambda: color('blue'), 'B')
onkey(lambda: color('red'), 'R')
onkey(lambda: store('shape', line), 'l')
onkey(lambda: store('shape', square), 's')
onkey(lambda: store('shape', circle), 'c')
onkey(lambda: store('shape', rectangle), 'r')
onkey(lambda: store('shape', triangle), 't')
done()
Logo

Free Python Games


Donate
If you or your organization uses Free Games, consider donating:

Donate to Free Python Games

Related Topics
Documentation overview
Previous: Illusion
Next: Maze
Quick search

```

---
[Markdown](https://www.markdownguide.org/cheat-sheet/)

| Nombre | Actividad |
| -------- | -------- |
| Emilio | Dibujar algo |

- [x] Emilio Dibujar ALgo
- [ ] Miguel Angel No se
- [x] Lebron Dibujar

 Para crear un encabezado, agrega uno  a seis símbolos # antes del encabezado del texto.

 # Encabezado grande
 ## Encabezado Mediano
 ### Encabezado Pequeño

 Puedes indicar énfasis con texto en negritas, itálicas o tachadas en los campos de comentario.

 Estilo
 - Negrita ** ** **Este texto está en negrita**
 - Cursiva * * o _ _ *Este texto está en cursiva*
 - Tachado ~~ ~~ ~~Este texto está equivocado~~
 - Cursiva en negrita y anidada ** ** y __ **Este texto es _extremadamente_ importante**
 - Todo en negrita y cursiva *** *** ***Todo este texto es importante***

 # Usar emojis inicia escribiendo : + letra escoges el emoji que quieres
 🍎
 👏
 🥇
 🥈
 🥉

 # Cita de Texto
 > ITESM

 # Enlace 
 [Github Pages](https://pages.github.com/)

 # Imagen
 ![Github Pages](https://tec.mx/sites/default/files/repositorio/Home/tec-de-monterrey-newsroom.jpg)

 # SemanaTecOct2021

 ```geojson
 {
    "type":"Polygon",
    "coordinates":[
        [
            [-85,35],
            [-100.2155,25.6748],
            [-100.309,25.6714],
            [-101.35628,20.67675],
            [-85,30]
        ]
    ]
 }
```

# Listas 
Puedes realizar una lista desordenada al anteceder una o más líneas de texto con - o *.

- Panda Rojo
- Ron da error
- Los Picapiedra

1. Panda Rojo
2. Ron da error
3. Los Picapiedra

# Listas Anidadas
- Primer Concierto
    - Primer pijamada
        - Panda

# Lista de Tareas
- [x] #739
- [ ] 👩
- [ ] :tada:
