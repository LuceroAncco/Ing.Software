## Reflexión

**¿Por qué Git es crítico en proyectos colaborativos?**

Git es crítico porque permite que varias personas trabajen en el mismo proyecto de forma
simultánea sin pisarse el trabajo entre sí. Cada integrante puede hacer cambios en su propia
copia local, y Git se encarga de combinar (mergear) esos cambios de manera ordenada. Además,
mantiene un historial completo de quién hizo cada cambio, cuándo y por qué (gracias a los
mensajes de commit), lo que facilita la comunicación y la trazabilidad dentro del equipo.

**¿Qué problemas evita?**

- Pérdida de código: si algo se rompe, siempre se puede volver a una versión anterior que
  funcionaba (con `git log` y `git checkout`/`git revert`).
- Sobrescritura de trabajo: sin control de versiones, dos personas editando el mismo archivo
  podrían borrar el trabajo de la otra sin darse cuenta. Git detecta estos conflictos y obliga
  a resolverlos manualmente.
- Falta de trazabilidad: sin Git no se sabría quién hizo qué cambio ni cuándo, dificultando
  encontrar el origen de un error.
- Dependencia de un solo dispositivo: al subir el código a un repositorio remoto (como GitHub),
  el proyecto no depende de una sola computadora; si esta falla, el trabajo no se pierde.