# PIA Control Óptimo

Proyecto final para la materia de Control Óptimo.

La presente instrucción de trabajo, presenta los requerimientos para el Producto Integrador para la materia de Control Óptimo a entregarse el día y hora indicada por el instructor del curso.

El proyecto a desarrollar es una compilación del aprendizaje teórico - práctico del curso _Control Óptimo_ impartido en el semestre agosto - diciembre 2022.

## Modelo a desarrollar:

El modelo físico a desarrollar es un sistema de 2o orden basado en dos resistores, dos capacitores y un POD. El conjunto, correctamente conectado, es capaz de generar respuestas a entradas básicas de control generadas a partir de la graduación del POD y los parámetros básicos del sistema.

La planta, de acuerdo al esquema mostrado a continuación, puede desarrollarse en la plataforma de trabajo _"Arduino"_, para lo cual se requerirá un Arduino Uno R3 (o cualquier otro modelo, tomando en cuenta la necesidad de modificar el diagrama y código de acuerdo a la placa base).

### Diagrama de alambrado

![Screenshot from 2022-11-16 21-59-35](https://user-images.githubusercontent.com/118387488/202351818-81c70051-0c5a-4230-9098-54f13c0eba3e.png)

### Diagrama esquemático

![image](https://user-images.githubusercontent.com/118387488/202359354-8879c1bb-7bd8-42d8-95c5-bf83b2e06bcd.png)


## Compontentes

En el reporte se debe de incluir una tabla que indique los valores[^1] de resistencias y capacitores utilizados en la planta[^2].

[^1]:Los valores indicados deberán coincidir con los cálculos, simulaciones y corridas _"on the wire"_ de la planta.
[^2]:Los valores de resistencias y capacitores no pueden ser iguales entre equipos, i.e. cada planta es **diferente** a las demás.

|Elemento| Cantidad | Valores utilizados en planta|
|:---|:---:|:---:|
|Arduino Uno R3|1|N.A.|
|Resistencias|2||
|Capacitores|2||
|Potenciómetro|1||
|Bread board|1|N.A.|
|Conectores|Los necesarios|N.A.|

## Instrucciones generales

* Genere el diagrama esquemático del sistema (de acuerdo al mostrado en clase).
* Desarrolle el sistema a partir de componentes simples.
* Calcule el valor de las capacitancias y resistencias de manera que las constantes de tiempo sean tales que puedan ser analizadas por la placa del Arduino.
* Anote los valores de las resistencias y capacitores utilizados en la tabla proporcionada (genere una igual en el reporte).
* Simule el sistema en las plantillas de python (Jupyter lab) facilitadas en las sesiones del curso.
* Incluya en su reporte un análisis de la diferencia entre el sistema simulado y el real.

## Elementos de análisis, cálculo y desarrollo a incluir en el reporte

* Modelo matemático del sistema.
* La codificación (se entrega plantilla base).
* Cálculos, comprobaciones y resultados a desarrollar:
  * Defina si el sistema puede ser controlado y si puede desarrollarse un observador para el mismo (hint: obtenga cálculos de controlabilidad y observabilidad).
  * Genere un control por asignación de polos de la manera clásica tal que el sistema tarde el menor tiempo posible en alcanzar el valor de estado estacionario (hint: grafíque el LGR del sistema y a partir del mismo, defina los valores ideales de la ganancia para que el sistema se comporte de la manera indicada).
  * Genere un control por asignación de polos de la manera clásica, tal que el sistema utilice la menor cantidad de señal de control. Si se requiere utilice un observador para completar el estado del sistema.
  * Genere, por medio de las plantillas de Jupyter Lab otorgadas en clase, las ganancias del sistema tal que cumplan con los criterios de diseño indicados en los dos puntos anteriores, en este caso, utilizando la teoría del control óptimo. (Hint: utilice un control de horizonte infinito - LQR).
* Lleve a cabo la realización física para cada uno de los subincisos del punto anterior.
* Aplique una entrada escalón y grafíque la salida del sistema en cada caso. *
* Compare el resultado del experimento con la simulación del cada caso. *
* ¿Cuál es la síntesis de comportamiento del sistema?
Para cada respuesta marcada con “*” genere la impresión a partir del puerto serial del sistema.

## Evidencias a entregar

* Fotografía del circuito armado.
* Video del sistema en funcionamiento.
* Memorias debidamente desarrolladas:
  * Planteamiento del problema.
  * Rigor del desarrollo, cálculo y respuestas.
  * Explicaciones debidamente soportadas por evidencia (cálculos, citas y referencias).
  * Gráficas claras y representativas.
  * Redacción impecable, así como buena caligrafía.
* Portada que incluya fecha, datos de integrantes del equipo (máximo 4), generales de la materia, nombre de la actividad.
* El sistema debe ser funcional (demostración mediante el video sometido).
