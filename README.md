# Embudos y prueba test A/B
En esta tarea se rastrearon los eventos ocurridos en eun app de alimentos, se hizo una separación en dos grupos para determinar diferencias estadisticas.

📘 Descripción del proyecto.
PAra esta tarea se  estudió el embudo de ventas. Descubrimos cómo los usuarios llegan a la etapa de compra. ¿Cuántos usuarios realmente llegan a esta etapa? ¿Cuántos se atascan en etapas anteriores? ¿Qué etapas en particular?

Luego, observamos los resultados de un test A/A/B . Al equipo de diseño le gustaría cambiar las fuentes de toda la aplicación, pero la gerencia teme que los usuarios piensen que el nuevo diseño es intimidante. Por ello, deciden tomar una decisión basada en los resultados de un test A/A/B.

⚙️ Herramientas y tecnologías usadas.
1.-pandas
2.-numpy
3.-seaborn
4.-scipy

💡 Desafío o caso de uso.
En este ejercicio se buscaban contestar diversas preguntas
Estudiar y comprobar los datos

¿Cuántos eventos hay en los registros?
¿Cuántos usuarios hay en los registros?
¿Cuál es el promedio de eventos por usuario?
¿Qué periodo de tiempo cubren los datos? Encuentra la fecha máxima y mínima. Traza un histograma por fecha y hora. ¿Puedes tener seguridad de que tienes datos igualmente completos para todo el periodo? Los eventos más antiguos podrían terminar en los registros de algunos usuarios por razones técnicas y esto podría sesgar el panorama general. Encuentra el momento en el que los datos comienzan a estar completos e ignora la sección anterior. ¿Qué periodo representan realmente los datos?
¿Perdiste muchos eventos y usuarios al excluir los datos más antiguos?
Asegúrate de tener usuarios de los tres grupos experimentales.

Estudiar el embudo de eventos

Observa qué eventos hay en los registros y su frecuencia de suceso. Ordénalos por frecuencia.
Encuentra la cantidad de usuarios que realizaron cada una de estas acciones. Ordena los eventos por el número de usuarios. Calcula la proporción de usuarios que realizaron la acción al menos una vez.
¿En qué orden crees que ocurrieron las acciones? ¿Todas son parte de una sola secuencia? No es necesario tenerlas en cuenta al calcular el embudo.
Utiliza el embudo de eventos para encontrar la proporción de usuarios que pasan de una etapa a la siguiente. Por ejemplo, para la secuencia de eventos A → B → C, calcula la proporción de usuarios en la etapa B a la cantidad de usuarios en la etapa A y la proporción de usuarios en la etapa C a la cantidad en la etapa B.
¿En qué etapa pierdes más usuarios?
¿Qué porcentaje de usuarios hace todo el viaje desde su primer evento hasta el pago?

Estudiar los resultados del experimento

¿Cuántos usuarios hay en cada grupo?
Tenemos dos grupos de control en el test A/A, donde comprobamos nuestros mecanismos y cálculos. Observa si hay una diferencia estadísticamente significativa entre las muestras 246 y 247.
Selecciona el evento más popular. En cada uno de los grupos de control, encuentra la cantidad de usuarios que realizaron esta acción. Encuentra su proporción. Comprueba si la diferencia entre los grupos es estadísticamente significativa. Repite el procedimiento para todos los demás eventos (ahorrarás tiempo si creas una función especial para esta prueba). ¿Puedes confirmar que los grupos se dividieron correctamente?
Haz lo mismo para el grupo con fuentes alteradas. Compara los resultados con los de cada uno de los grupos de control para cada evento de forma aislada. Compara los resultados con los resultados combinados de los grupos de control. ¿Qué conclusiones puedes sacar del experimento?
¿Qué nivel de significancia has establecido para probar las hipótesis estadísticas mencionadas anteriormente? Calcula cuántas pruebas de hipótesis estadísticas has realizado. Con un nivel de significancia estadística de 0.1, uno de cada 10 resultados podría ser falso. ¿Cuál debería ser el nivel de significancia? Si deseas cambiarlo, vuelve a ejecutar los pasos anteriores y comprueba tus conclusiones.

📊 Resultados o aprendizajes.
Como parte de las conclusiones generales Se realizaron todas las combinaciones, solo en un caso , en un evento pudimos rechazar la hipotesis y fue usando un valor de alpha bastante permitivo, en los demas casos no se pudo rechazar, entonces la conclusión es que los 3 grupos pueden considerarse similares y no resalta ninguno en contraste a otro.
Tambien se preguntó  ¿Qué nivel de significancia has establecido para probar lashipótesis estadísticas mencionadas anteriormente? Calcula cuántas pruebas de hipótesis estadísticas has realizado. Con un nivel de significancia estadística de 0.1, uno de cada 10 resultados podría ser falso. ¿Cuál debería ser el nivel de significancia?
Para esto se usó alpha como 0.1 y como 0.05, la idea original era usarlo tambien como 0.01 pero se concluyó que no habia caso, esto por que al usar 0.1 solo hubo un caso donde se rechazó la hipotesis y era la tasa mas permisiva, despues e probó con 0.05 y en este caso ya no se rechazó ninguna hippotesis, por lo tanto 0.01 iba a ser aún mas improbable, siendo 0.05 el valor estandar para pruebas cientificas creo que podemos mantenernos firmnes en nuestras conclusiones donde noo hay diferencia entre los grupos.

