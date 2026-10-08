# Bitácora de IA — Laboratorio 1

Nombre: Javier Cordero     Fecha: 07/10/2026

> Regla del curso: la IA se usa para APRENDER y REVISAR, no para que haga el trabajo por ti.
> Si no puedes explicar una línea, no la entregues.

| # | Qué le pregunté a la IA (resumen) | Qué me respondió | ¿Lo usé? ¿Qué corregí y por qué? | Cómo lo verifiqué |
| 1 |¿Por qué la imagen no se visualiza?|el atributo SRC apunta a un archivo que no existen|descargar la imagen y le asigne el mismo nombre|Usando Live Server para comprobar que la imagen se muestra en la pagina|
| 2 |                                   |                   |                                 |                   |

## Diagnóstico del sitio antiguo (Paso 1)
Tres problemas que encontré en `sitio-antiguo.html` y por qué son un problema hoy:
1.<CENTER>, <FONT>, <MARQUEE> y el atributo BGCOLOR son considera obsoleto por validator que los marca como error y el navegador deja de renderizarlas
2.<HEAD> sin <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <html> sin lang. Mala accesibilidad y la página no se adapta al celular.
3. <title>sendero</title> no describe lo que es la pagina 
   <A> sin cerrar en la linea 12 <DIV> innecesario y <DIV> sin cerrar en la linea 21
   No aparece bien en Google, mezcla estructura con presentación y no es semántico.

## Reflexión (3-4 líneas)
¿Qué aprendí hoy sobre la diferencia entre "que se vea" y "que esté bien construido"?
aprendi que si una pagina se vea bien no significa que este bien estructurada ya que si esta mal estructurado a futuro la aplicacion puede presentar fallas, es muy complicado hacerle mantenimiento y actualizarlo. los problemas que puede ver sin usar el validator fue que hay etiquetas que no estan cerrados como en la linea 12 y 23 y etiquetas que no eran necesario utilizarlas como el <div>

