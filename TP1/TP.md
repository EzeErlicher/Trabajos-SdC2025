# Trabajo Practico 1

## Introducción
Para evaluar el rendimiento del hardware en función de las tareas diarias, podemos usar benchmarks específicos que reflejen la carga de trabajo real. A continuación, se presenta una tabla que asocia cada tarea con el benchmark más representativo.

## Benchmarks para Tareas Diarias

| Tarea                            | Benchmark Representativo                                  |
|----------------------------------|----------------------------------------------------------|
| Compilación de código fuente    | [Phoronix Test Suite - Build Linux Kernel](https://openbenchmarking.org/test/pts/build-linux-kernel-1.15.0) |
| Descarga de archivos            | [Speedtest CLI](https://www.speedtest.net/apps/cli)      |
| Ejecutar bases de datos         | [TPC-C Benchmark](https://www.tpc.org/tpcc/) - Simula cargas transaccionales en bases de datos |
| Uso general de aplicaciones y multitareas | [PCMark 10](https://benchmarks.ul.com/pcmark10) - Evalúa el rendimiento en tareas diarias como navegación web, edición de documentos y productividad en general |
| Reuniones online                | [WebRTC Benchmark](https://testrtc.com/) - Evalúa el rendimiento de video y audio en conferencias web |

Este conjunto de benchmarks permitirá medir el rendimiento del sistema en cada una de estas tareas, identificando posibles cuellos de botella y optimizaciones necesarias.

---

# Comparación de Procesadores para Compilación del Kernel de Linux

A la hora de evaluar cuál de los siguientes procesadores ofrece mejor rendimiento en la compilación del kernel de Linux, utilizamos las métricas proporcionadas por el benchmark:  
- [Phoronix Test Suite - Build Linux Kernel 1.16.0](https://openbenchmarking.org/test/pts/build-linux-kernel-1.16.0)

### Resultados de Benchmark

| Procesador            | Tiempo Promedio (seg) |
|----------------------|----------------------|
| **Intel Core i5-13600K**  | **83 ± 3**           |
| **AMD Ryzen 9 5900X**    | **97 ± 7**           |
| **AMD Ryzen 9 7950X**    | **53 ± 3**           |

### Análisis de Rendimiento

El **AMD Ryzen 9 7950X** se posiciona como el procesador con mejor rendimiento en esta prueba, logrando tiempos de compilación significativamente menores. Su arquitectura y mayor cantidad de núcleos permiten un procesamiento más eficiente en cargas de trabajo altamente paralelizables como la compilación del kernel.

El **Intel Core i5-13600K** ofrece un rendimiento sólido y se mantiene en una posición intermedia. Aunque no alcanza la velocidad del 7950X, sigue siendo una opción competitiva con un buen equilibrio entre costo y rendimiento.

Por otro lado, el **AMD Ryzen 9 5900X** muestra un desempeño inferior en comparación con los otros dos procesadores evaluados. Si bien sigue siendo una opción viable, su tiempo de compilación más alto indica que no aprovecha tan eficientemente sus recursos en esta tarea específica.

En conclusión, el Ryzen 9 7950X es la mejor opción para compilaciones rápidas, mientras que el i5-13600K ofrece un buen rendimiento a un precio más accesible. El 5900X, en este caso, queda rezagado frente a las opciones más modernas.

---

# Aceleración y Eficiencia en el Uso de Núcleos

### Aceleración al usar el AMD Ryzen 9 7950X  
Al comparar el **Ryzen 9 7950X** con el **Ryzen 9 5900X**, se espera una mejora significativa en tiempos de compilación debido al aumento en el número de núcleos y mejoras arquitectónicas. Aunque no disponemos de datos específicos de compilación del kernel, en pruebas generales, el **7950X** ha mostrado un rendimiento superior en tareas multihilo.  

### Eficiencia en el uso de núcleos  
El **Intel Core i5-13600K**, a pesar de tener menos núcleos físicos que los modelos de AMD mencionados, utiliza una arquitectura híbrida que combina núcleos de alto rendimiento y de alta eficiencia. Esto le permite manejar eficientemente tareas que requieren tanto rendimiento monohilo como multihilo.  

Sin embargo, en tareas altamente paralelas como la compilación del kernel, los procesadores con mayor cantidad de núcleos físicos, como el **Ryzen 9 7950X**, suelen tener una ventaja.

---

# Eficiencia en Términos de Costo  

- **Intel Core i5-13600K**: Ofrece una excelente relación rendimiento-precio, especialmente para usuarios que buscan un equilibrio entre costo y desempeño en tareas de compilación.  

- **AMD Ryzen 9 5900X**: Aunque su precio ha disminuido desde su lanzamiento, sigue siendo más costoso que el i5-13600K. Sin embargo, para tareas que aprovechan múltiples núcleos, puede justificar su precio.  

- **AMD Ryzen 9 7950X**: Es el más caro de los tres, pero también ofrece el mejor rendimiento en tareas altamente paralelas. Su eficiencia en términos de costo dependerá de la frecuencia y magnitud de las tareas de compilación que realices.  

---
