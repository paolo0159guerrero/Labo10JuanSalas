1.¿Por qué necesitamos Loki además de Prometheus si ya tenemos /metrics?
Porque prometheus nos sirve para detectar anomalías y alertar mientra que Loki nos dice exactamente en qué parte específica ocurrió
2.¿Qué ventaja aporta que las fuentes de datos de Grafana estén aprovisionadas como código y no creadas a mano?
Es como la ventaja de lo tradicional que antes se hacía a mano y había un alto porcentaje de errores humanos y lo más importante el tiempo en la actualidad al estar todo automatizado si se cae el servidor no habría problema en retomarlo
3.El panel "CPU contenedor" y el panel "CPU host" pueden mostrar valores muy distintos. ¿Por qué? ¿Cuál usarías para alertar sobre una aplicación concreta?
El cpu host mide el uso total de la máquina virtual o física mientras que el cpu contenedor el porcentaje que consumiendo ese proceso aislado. Se usuaria el cpu contenedor si la aplicación web se frizea necesitamos el estado de ese contenedor en específico
4.¿Qué diferencia hay entre el evaluation interval y el pending period de una alarma?
Evaluation interval define cada cuanto tiempo se evalua la condición mientras que pending period cuánto tiempo debe mantenerse la condición.
