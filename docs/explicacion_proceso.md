# Días de tele · explicación breve del proceso

La idea inicial partía de un Excel que simulaba un juego: cada casilla ocultaba un fragmento muy corto de una melodía de series de televisión antiguas, y el jugador debía adivinar el título de la serie.

El primer paso fue analizar el archivo original para comprobar si los audios estaban vinculados externamente o incrustados dentro del propio Excel. Al revisar la estructura interna, se localizaron los fragmentos como objetos de sonido incrustados y fue posible extraerlos como archivos WAV.

Después se reconstruyó la relación correcta entre cada casilla, su audio y el título de la serie correspondiente. Este paso fue importante porque el orden interno de los audios no siempre coincide con el orden visible del tablero.

Con esa información se creó una versión web del juego en HTML, CSS y JavaScript. El recurso permite seleccionar casillas, reproducir melodías, escribir respuestas, comprobar aciertos, mostrar soluciones y llevar un marcador de progreso.

En la versión final se añadió un estilo visual retro, inspirado en la televisión clásica y los juegos de los años 80/90. También se incorporó un sistema de guardado automático en el navegador y botones para exportar e importar el progreso mediante un archivo JSON.

El resultado es un mini-juego ligero, reutilizable y fácil de publicar online, creado a partir de un recurso existente que originalmente solo funcionaba dentro de Excel.
