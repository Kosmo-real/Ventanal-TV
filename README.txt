VENTANAL V9.6 — AUTOMÁTICO
- Noticias ya NO usan OpenAI ni OPENAI_API_KEY.
- Noticias se obtienen desde un servidor externo de noticias actualizado continuamente y se renuevan automáticamente.
- Sin créditos de OpenAI para Noticias.
- Reproductores YouTube mantienen controls=0, disablekb=1 y fs=0 para aspecto TV.
- Qué Dice Chile queda de 19:15 a 21:00 los días de semana, sin el solapamiento de las 20:00.
- Cine/Kids continúan buscando contenido embebible y reproducible mediante YouTube Data API.
- La API key de YouTube y las credenciales Firebase siguen solo en Vercel.


VENTANAL V9.7 — HORARIO ACTUALIZADO
- Deportes extremos: 18:00 todos los días.
- Días de semana: Qué Dice Chile 19:15–21:00.
- Fin de semana: Pantalla grande desde las 19:00.
- Noticias: 06:30, 13:30 y 21:00.
- Mantiene Noticias automáticas sin OpenAI, Kids, Cine y modo TV.


VENTANAL V9.8 — SEÑAL TV
- El reproductor no recibe clics/taps: no se puede pausar tocando la pantalla.
- Controles de YouTube ocultos y teclado desactivado.
- La señal principal busca exclusivamente emisiones que YouTube marca como LIVE mediante eventType=live.
- Se mantiene el botón externo Activar sonido.


VENTANAL V9.9 — TV LINEAL
- Los bloques siguen el reloj de Ventanal: el siguiente programa entra a su hora exacta.
- Los videos reproducibles se solicitan con la duración objetivo del bloque.
- Los videos de YouTube quedan configurados en loop para cubrir el tiempo restante si terminan antes.
- La señal En Vivo mantiene prioridad por transmisiones realmente LIVE.
- La pantalla del reproductor sigue sin interacción directa de play/pausa.
- Deportes Extremos: 18:00; Qué Dice Chile: 19:15–21:00 de lunes a viernes.
- Noticias automáticas sin depender de créditos OpenAI.

VENTANAL V10 — SEÑAL SINCRONIZADA
- Todos los visitantes reciben la misma selección de video por fecha y bloque.
- El reloj de Ventanal se sincroniza con el servidor y se corrige cada 30 segundos.
- En videos bajo demanda, quien entra tarde salta a la posición correspondiente del bloque.
- Las transmisiones LIVE usan la misma emisión en vivo para todos.
- Los últimos 3 minutos de cada bloque se reservan para una tanda propia de Ventanal.
- La tanda inicial incluye promos propias de Ventanal Kids, Cine, Noticias y Ventanal TV.
- A la hora exacta del siguiente bloque, la señal cambia automáticamente.
- No se muestran nombres de canales/fuentes externas en la interfaz de reproducción.
- El reproductor no acepta clic/tap para play o pausa.
NOTA: si el contenido se reproduce desde YouTube, YouTube puede insertar publicidad propia; Ventanal no puede eliminarla. Para cero publicidad externa garantizada se necesita contenido propio/licenciado servido desde hosting/CDN sin anuncios.


VENTANAL V10.1 — ENTRETENCIÓN LIVE
- Buenos días, Chile pasa a un formato de juegos/concursos.
- Barrio adentro se reemplaza por Desafío Ventanal.
- La sobremesa se reemplaza por Tarde de juegos.
- Qué Dice Chile usa búsqueda específica; Caso Cerrado y contenido adulto/judicial quedan bloqueados.
- La señal principal exige contenido en vivo y cambia automáticamente de señal si una emisión termina o falla.
- Se agregó botón Expandir pantalla.
- Los últimos 3 minutos de cada bloque son una tanda propia creada para Ventanal: Kids, Cine, Desafío Ventanal y Ventanal TV.
- La interfaz no muestra nombres de plataformas ni canales fuente.
- Se agregó soporte opcional para otras fuentes LIVE autorizadas mediante VENTANAL_LIVE_FEEDS_JSON (HLS/direct live feed). Si no hay feeds configurados, usa el proveedor live existente.
- Si la señal falla repetidamente, Ventanal se recupera y refresca automáticamente.
- Se mantiene el reloj del servidor para cambios de bloque sincronizados.


VENTANAL V10.2 — FAMILIAR
- Desafío Ventanal prioriza concursos, preguntas y respuestas, trivia, cultura general,
  desafíos familiares, talentos y juegos divertidos.
- Tarde de Juegos y Buenos días, Chile también priorizan entretención familiar.
- Filtro reforzado contra realities de parejas, citas, infidelidad, sexo, contenido adulto,
  juicios, Caso Cerrado, true crime, violencia gráfica, casinos y apuestas.
- Mantiene señal LIVE, cambio automático de señal, pantalla completa y tanda propia de 3 minutos.


VENTANAL V10.3 — FILTRO FAMILIAR ESTRICTO
- Buenos días Chile, Desafío Ventanal y Tarde de Juegos ya no aceptan cualquier transmisión LIVE.
- Para esos bloques el contenido debe incluir señales claras de concurso, trivia, preguntas,
  juegos, talentos, cultura general o entretenimiento familiar.
- Se rechazan explícitamente realities, parejas/citas, farándula, contenido sexual/adulto,
  juicios, Caso Cerrado, crimen, violencia, casinos y apuestas.
- Si no existe una señal familiar aprobada en vivo, Ventanal muestra una señal propia segura
  y sigue buscando automáticamente en vez de poner contenido aleatorio.


VENTANAL V10.4 — LIVE + RESPALDO FAMILIAR
- Orden de búsqueda: concurso/juego familiar LIVE -> entretenimiento familiar LIVE seguro ->
  concurso/juego familiar grabado seguro como respaldo.
- Nunca usa contenido adulto/reality/juicios como respaldo.
- Si entra un respaldo grabado, se sincroniza con el minuto del bloque.
- Mientras hay respaldo, Ventanal vuelve a comprobar periódicamente si apareció una señal LIVE segura.
- Ya no queda infinitamente en la pantalla 'Estamos buscando...'.
- Se mantienen anuncios propios en los últimos 3 minutos y el cambio exacto de bloque.
