# github-representa-readmes

Este es el README de un proyecto real. Tienes 3 minutos, tú solo, para reescribirlo con lo que sabes de él. Usa la plantilla de siete secciones y no inventes nada: todo lo que necesitas está en la ficha.

## Ficha

<ul>
<li>Qué es: un temporizador de estudio hecho con JavaScript y CSS, sin librerías.</li>
<li>Para quién: estudiantes que se distraen con el móvil.</li>
<li>Por qué existe: las apps de pomodoro que probó su autora tenían anuncios, pedían registro o no avisaban al cambiar de pestaña.</li>
<li>Qué hace: alterna bloques de 25 minutos de trabajo y 5 de descanso, cuenta los bloques del día, avisa con sonido y texto, y se maneja con teclado (espacio para pausar, R para reiniciar).</li>
<li>Una decisión: el tiempo restante se anuncia al lector de pantalla solo al cambiar de minuto, porque cada segundo lo volvía inútil.</li>
<li>Lo que le costó: el temporizador se desajustaba al cambiar de pestaña; lo arregló guardando la hora de inicio y calculando el tiempo restante en cada tick.</li>
<li>Pendiente: historial semanal, modo oscuro y más pruebas con lectores de pantalla.</li>
</ul>

# Pomodoro

App de pomodoro hecha con JavaScript.

## Instalar

npm install
npm start

## TODO

- arreglar bug
- estilos

<br>
<br>
<br>
<br>

# Pomodoro-Estudio

Un temporizador de estudio para quien se distrae con el móvil: trabaja 25 minutos, descansa 5 y ve cuántos bloques llevas hoy. [Demo en vivo](https://pomodoro-estudio.example.com) 

![Captura del temporizador en marcha con el contador de bloques del día](https://freesvg.org/img/pomodorotimer.png)

## El problema

Las apps de pomodoro que probé tenían anuncios, pedían registro o no avisaban si cambiaba de pestaña. Quería algo que se abriera y funcionara.

## Qué hace

- Alterna bloques de trabajo (25 min) y descansos (5 min), configurables.
- Muestra cuántos bloques has completado hoy.
- Avisa con sonido y con texto cuando termina un bloque.
- Se maneja entero con teclado: espacio para pausar, `R` para reiniciar.

## Cómo lo construí

JavaScript sin librerías y un poco de CSS. El tiempo restante se anuncia con `aria-live="polite"` solo al cambiar de minuto, porque anunciarlo cada segundo volvía inútil el lector de pantalla.

## Cómo probarlo

```bash
git clone https://github.com/usuario/pomodoro-estudio.git
cd pomodoro-estudio
npm install
npm start
```

Abre `http://localhost:3000`.

## Aprendizajes

El temporizador se desajustaba si cambiabas de pestaña, porque el navegador frena los `setInterval`. Lo arreglé guardando la hora de inicio y calculando el tiempo restante en cada tick, en vez de restar un segundo cada vez.

## Próximos pasos

- Guardar el historial de bloques por semana.
- Modo oscuro.
- Probarlo con más lectores de pantalla.