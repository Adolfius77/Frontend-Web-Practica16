## Preguntas
¿por qué se usa un contexto y no props para la sesión?
se usa el contexto por que la sesion es un estado global de la app, no es un dato de un solo componente

¿qué pasa si un componente usa la sesión fuera del proveedor?
devuelve null y la funcion lanzara un error que dice que el useSesion tiene que usarse dentro del provedor sesion

¿dónde se guarda el token y qué riesgo tiene ese lugar?
se guarda en el localStorage con el token y tambien el usuario se guarda como json,
el riesgo es que en localStorage es legible desde el js del navegador así que esta expuesto a ataques de xss el
atacante puede robar el token y suplantar la sesión 
