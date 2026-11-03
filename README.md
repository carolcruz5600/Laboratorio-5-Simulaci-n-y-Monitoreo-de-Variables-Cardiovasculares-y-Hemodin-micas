# Laboratorio 5

**Simulación y Monitoreo de Variables Cardiovasculares y Hemodinámicas**

1. Resumen

Se evaluó funcionalmente un monitor multiparamétrico Mindray uMEC 100 mediante un simulador Pronk OxSim OX-1 conectado al sensor de pulsioximetría. Se revisaron escenarios de bradicardia, hipoxemia, saturación alta/baja perfusión y taquicardia. Los videos muestran, entre otras lecturas, 40 bpm con 95 % de SpO₂, 80 bpm con 85 %, 80 bpm con 100 % y 140 bpm con 99 %. Los resultados experimentales suministrados incluyen tiempos de activación de alarmas y mediciones comparativas entre simulador y monitor.

2. Introducción

La pulsioximetría estima la saturación periférica de oxígeno (SpO₂) mediante la diferencia de absorción óptica de la hemoglobina oxigenada y reducida, generalmente con luz roja e infrarroja. La componente pulsátil de la señal permite identificar el pulso y obtener una frecuencia derivada de la fotopletismografía. Los simuladores de pulsioximetría permiten comprobar la respuesta de un monitor ante condiciones predefinidas sin conectar a un paciente. El resultado depende de la compatibilidad del sensor, la configuración del simulador, el procesamiento y los retardos de alarma del monitor.

3. Objetivos

General: operar el simulador Pronk OxSim OX-1 y el monitor Mindray uMEC 100 para realizar pruebas funcionales.

Específicos: (i) reconocer modos y variables simuladas; (ii) comprobar mediciones y alarmas ante escenarios fisiológicos y patológicos; (iii) calcular errores absolutos y relativos; (iv) analizar la forma de onda fotopletismográfica y las limitaciones experimentales.

## Parte A. Revisión bibliográfica y fundamentación técnica

**1. Revisión bibliográfica del monitor Mindray uMEC 100 y el simulador Pronk OxSim OX-1.**

### Equipos utilizados

Monitor Mindray uMEC 100: dispositivo multiparamétrico que muestra valores fisiológicos y permite configurar alarmas. En esta práctica se utilizó su módulo de SpO₂ y la frecuencia de pulso derivada del sensor. El monitor puede disponer de otros módulos según su configuración, pero no se evaluaron en esta práctica.

Simulador Pronk OxSim OX-1: dispositivo de prueba para sistemas de pulsioximetría que reproduce condiciones ópticas/pulsátiles detectables por un sensor compatible. Para esta práctica se consideran SpO₂ simulada, frecuencia de pulso y una condición de baja perfusión. No debe confundirse la frecuencia de pulso de SpO₂ (PR) con una frecuencia cardíaca medida por ECG (HR), aunque en estas pruebas se comparen numéricamente.

### a. ¿Cómo colocar el uMEC 100 en modo monitor?

En la guía se indica encender el uMEC 100 y seleccionar el modo “monitor”. La secuencia exacta de menús no está documentada en el material aportado; no se atribuye una ruta de botones sin verificar el manual correspondiente. Procedimiento seguro: con supervisión del personal del laboratorio, encender el equipo, confirmar que se encuentra en pantalla de monitorización, verificar que el módulo SpO₂ está habilitado y que se muestran los parámetros y sus límites de alarma; conectar el sensor al simulador y esperar estabilización. Si aparece un selector de modos, escoger “Monitor” según la interfaz y el manual de la versión instalada.

### b. ¿Qué parámetros fisiológicos puede simular el Pronk OxSim OX-1?

<div align="center">
<table>
<tr><th align="center">Parámetro</th><th align="center">Descripción</th><th align="center">Unidad</th></tr>
<tr><td align="center">SpO₂</td><td align="center">Porcentaje de saturación estimada a partir de la relación de absorciones ópticas roja/infrarroja.</td><td align="center">%</td></tr>
<tr><td align="center">Frecuencia de pulso (PR)</td><td align="center">Número de pulsaciones simuladas por minuto que el monitor estima desde la señal pulsátil.</td><td align="center">bpm</td></tr>
<tr><td align="center">Perfusión / amplitud pulsátil</td><td align="center">Intensidad relativa del componente pulsátil; una perfusión baja dificulta detectar pulsos y estimar SpO₂.</td><td align="center">Índice o modo según equipo</td></tr>
</table>
</div>

### c. ¿Cuáles son las tolerancias o errores máximos permitidos (EMP)?

No existe un único EMP clínico universal aplicable indistintamente a todos los sensores, intervalos y condiciones. La precisión exigible se toma de la ficha técnica del conjunto monitor-sensor y de normas aplicables. Como referencia general, la ISO 80601-2-61 trata requisitos de seguridad y desempeño esencial de pulsioxímetros; los valores específicos deben confirmarse en la documentación del modelo y sensor. La precisión de SpO₂ suele expresarse como Arms (raíz cuadrática media de las diferencias frente a una referencia), que NO equivale a un límite máximo de error de una sola medición. Para PR, el criterio también depende de especificaciones del fabricante. Por ello, no se certifica conformidad metrológica usando un supuesto ±2 % o ±3 bpm sin fuente exacta.

## Parte B. Procedimiento experimental

1) Se encendió el monitor y se visualizó la pantalla de monitorización. 2) Se acopló el sensor de SpO₂ al OxSim OX-1. 3) Se realizaron ajustes de frecuencia y saturación para observar la respuesta. 4) Se examinaron las lecturas, la curva pletismográfica y los indicadores visuales de alarma. 5) Se contrastaron las capturas con las cuatro condiciones especificadas en la guía. Los videos no permiten reconstruir con precisión absoluta todos los instantes de cambio de consigna ni la configuración completa de los umbrales.

### Pasos 1 a 5. Preparación, conexión, bradicardia y registro PPG

**1.** Construir la tabla de verificación de alarmas (presentada en el apartado de alarmas).

**2.** Encender el uMEC 100 y seleccionar la pantalla de monitorización.

**3.** Conectar la pinza de pulsioximetría al Pronk OxSim OX-1.

**4.** Simular 40 bpm y SpO₂ de 95 %, y comparar los valores con los del monitor.

**5.** Observar y registrar la señal fotopletismográfica.

#### Registro de lecturas observadas

<div align="center">
<table>
<tr><th align="center">Condición / secuencia</th><th align="center">Referencia indicada en guía</th><th align="center">Lectura observada en video</th><th align="center">Interpretación</th></tr>
<tr><td align="center">Bradicardia</td><td align="center">40 bpm; SpO₂ 95 %</td><td align="center">40 bpm; SpO₂ 95 %</td><td align="center">Coincidencia puntual de ambas lecturas</td></tr>
<tr><td align="center">Hipoxemia</td><td align="center">80 bpm; SpO₂ 85 %</td><td align="center">80 bpm; SpO₂ 85 %</td><td align="center">Coincidencia puntual de ambas lecturas</td></tr>
<tr><td align="center">SpO₂ alta, baja perfusión</td><td align="center">SpO₂ 99 % (Low Perfusion)</td><td align="center">80 bpm; SpO₂ 100 % en una captura</td><td align="center">Diferencia de 1 punto porcentual si corresponde al mismo ajuste; modo Low Perfusion no verificable solo por la pantalla</td></tr>
<tr><td align="center">Taquicardia</td><td align="center">140 bpm; SpO₂ 98 %</td><td align="center">140 bpm; SpO₂ 99 %</td><td align="center">Coincidencia en pulso; diferencia de 1 punto porcentual en SpO₂ si la captura es estable y corresponde a la consigna</td></tr>
</table>
</div>

Se observan además valores intermedios durante las transiciones (por ejemplo, descensos progresivos de PR o SpO₂). No deben usarse como errores en estado estacionario.

### Pasos 6 a 10. Configuración y verificación de alarmas

**6.** Configurar el límite inferior de SpO₂ en 90 %.

**7.** Simular 80 bpm y SpO₂ de 85 %, comprobar la alarma a los 5 segundos y registrar su respuesta.

**8.** Configurar el límite superior de SpO₂ en 97 %.

**9.** Simular SpO₂ de 99 % en baja perfusión, comprobar la alarma y observar posibles cambios en la onda PPG.

**10.** Simular 140 bpm y SpO₂ de 98 %, observar la onda y comprobar la alarma de pulso elevado.

#### Tabla de verificación experimental de alarmas

<div align="center">
<table>
<tr><th>Escenario</th><th>Límite inferior SpO₂</th><th>Límite superior SpO₂</th><th>Límites FP (inferior / superior)</th><th>Consigna FP / SpO₂</th><th>Alarma a los 5 s</th><th>Activación (s)</th></tr>
<tr><td align="center">Bradicardia</td><td align="center">90 %</td><td align="center">100 %</td><td align="center">50 / 110 bpm</td><td align="center">40 bpm / 95 %</td><td align="center">Sí</td><td align="center">12</td></tr>
<tr><td align="center">Hipoxia</td><td align="center">90 %</td><td align="center">100 %</td><td align="center">50 / 110 bpm</td><td align="center">80 bpm / 85 %</td><td align="center">No</td><td align="center">8</td></tr>
<tr><td align="center">Baja perfusión</td><td align="center">90 %</td><td align="center">97 %</td><td align="center">50 / 110 bpm</td><td align="center">80 bpm / 99 %</td><td align="center">No</td><td align="center">12</td></tr>
<tr><td align="center">Taquicardia</td><td align="center">90 %</td><td align="center">97 %</td><td align="center">50 / 110 bpm</td><td align="center">140 bpm / 98 %</td><td align="center">Sí</td><td align="center">10</td></tr>
</table>
</div>

#### Condiciones de activación de alarmas

<div align="center">
<table>
<tr><th>Escenario</th><th>Condición respecto al umbral</th><th>Alarma esperada</th></tr>
<tr><td align="center">Bradicardia</td><td align="center">FP: 40 &lt; 50 bpm</td><td align="center">FP baja</td></tr>
<tr><td align="center">Hipoxia</td><td align="center">SpO₂: 85 &lt; 90 %</td><td align="center">SpO₂ baja</td></tr>
<tr><td align="center">Baja perfusión</td><td align="center">SpO₂: 99 &gt; 97 %</td><td align="center">SpO₂ alta</td></tr>
<tr><td align="center">Taquicardia</td><td align="center">FP: 140 &gt; 110 bpm; SpO₂: 98 &gt; 97 %</td><td align="center">FP alta y SpO₂ alta</td></tr>
</table>
</div>

#### Cálculo de errores absolutos y porcentuales

$$
E_{\mathrm{abs}}=\left|V_{\mathrm{monitor}}-V_{\mathrm{simulado}}\right|
$$

$$
E_{\%}=\frac{E_{\mathrm{abs}}}{\left|V_{\mathrm{simulado}}\right|}\times100
$$

<div align="center">
<table>
<tr><th>Escenario</th><th>Variable</th><th>Valor simulado</th><th>Valor del monitor</th><th>Error absoluto</th><th>Error porcentual</th></tr>
<tr><td align="center">Bradicardia</td><td align="center">SpO₂ (%)</td><td align="center">95</td><td align="center">96</td><td align="center">1 pp</td><td align="center">1,05 %</td></tr>
<tr><td align="center">Bradicardia</td><td align="center">FP (bpm)</td><td align="center">40</td><td align="center">40</td><td align="center">0 bpm</td><td align="center">0,00 %</td></tr>
<tr><td align="center">Hipoxia</td><td align="center">SpO₂ (%)</td><td align="center">85</td><td align="center">85</td><td align="center">0 pp</td><td align="center">0,00 %</td></tr>
<tr><td align="center">Hipoxia</td><td align="center">FP (bpm)</td><td align="center">80</td><td align="center">80</td><td align="center">0 bpm</td><td align="center">0,00 %</td></tr>
<tr><td align="center">Baja perfusión</td><td align="center">SpO₂ (%)</td><td align="center">99</td><td align="center">100</td><td align="center">1 pp</td><td align="center">1,01 %</td></tr>
<tr><td align="center">Baja perfusión</td><td align="center">FP (bpm)</td><td align="center">80</td><td align="center">80</td><td align="center">0 bpm</td><td align="center">0,00 %</td></tr>
<tr><td align="center">Taquicardia</td><td align="center">SpO₂ (%)</td><td align="center">98</td><td align="center">99</td><td align="center">1 pp</td><td align="center">1,02 %</td></tr>
<tr><td align="center">Taquicardia</td><td align="center">FP (bpm)</td><td align="center">140</td><td align="center">140</td><td align="center">0 bpm</td><td align="center">0,00 %</td></tr>
</table>
</div>

El error absoluto de SpO₂ se expresa en puntos porcentuales (pp) y el de frecuencia de pulso en bpm. Los tiempos de activación y el estado a los 5 segundos se consignan según el registro experimental suministrado.

#### Forma de onda fotopletismográfica (PPG)

<div align="center">

$$
T=\frac{60}{\mathrm{PR}}
$$

</div>

La señal PPG representa cambios pulsátiles del volumen sanguíneo detectados ópticamente. Con 40 bpm el periodo esperado entre pulsos es 60/40 = 1,50 s; con 80 bpm, 0,75 s; con 140 bpm, aproximadamente 0,43 s. Si la amplitud se mantiene, al aumentar la frecuencia los picos aparecen más juntos. Una señal de baja perfusión puede mostrar amplitud reducida, pérdida de pulsos o mayor susceptibilidad al ruido; no se puede afirmar distorsión específica de forma concluyente a partir de estas capturas sin una ampliación de la curva y una referencia temporal estable.

## Parte C. Análisis de resultados

La guía contiene una pregunta sobre energía de desfibrilación que no corresponde a los equipos empleados. Se sustituye por el análisis estadístico descriptivo de los errores de SpO₂ y frecuencia de pulso medidos en esta práctica.

### Análisis 1. Diferencias entre los valores simulados y medidos

En las capturas comparables, la lectura del monitor reproduce los valores nominales de 40/95 y 80/85. Las diferencias de 1 pp en las condiciones de saturación elevada y taquicardia son pequeñas, pero por sí solas no demuestran cumplimiento de una especificación: es necesario conocer precisión declarada, incertidumbre del simulador, compatibilidad del sensor y estabilidad de la medición. Las secuencias muestran un proceso de actualización y estabilización, de modo que comparar un transitorio con una consigna fija exageraría artificialmente el error.

### Análisis 2. Relación entre la forma de onda PPG, la frecuencia de pulso y la SpO₂

La frecuencia del pulso se relaciona inversamente con la separación temporal de los máximos de la PPG (T = 60/PR). La SpO₂ no se obtiene directamente de la distancia entre picos, sino de la relación óptica de componentes roja e infrarroja. Por eso dos señales pueden tener la misma frecuencia y diferente SpO₂; igualmente, un pulso más rápido no implica necesariamente menor saturación.

### Limitaciones del análisis

Los videos muestran principalmente la pantalla del monitor y no ofrecen una vista simultánea legible y continua de todos los parámetros del simulador. Tampoco proporcionan un patrón de referencia independiente, cronometraje sincronizado, confirmación auditiva inequívoca ni series de repeticiones. No es posible realizar una evaluación estadística de repetibilidad o un ensayo de precisión clínica con estas evidencias.

## Preguntas de discusión

### Pregunta 1. ¿Cuál es el principio de operación del Pronk OxSim OX-1 para simular una onda pulsátil?

El equipo genera una modulación controlada de la señal óptica que el sensor interpreta como variaciones periódicas de absorción asociadas al pulso arterial. Al definir frecuencia, saturación simulada y condiciones de perfusión, se reproduce una respuesta óptica compatible con escenarios preestablecidos. El monitor procesa la señal recibida para calcular PR y SpO₂ y representar una curva pletismográfica. El detalle de implementación interna exacto del OX-1 debe contrastarse con su manual técnico.

### Pregunta 2. ¿Por qué una SpO₂ baja puede ser un falso positivo en mala perfusión?

Con perfusión periférica reducida, la componente pulsátil de la señal óptica disminuye respecto al ruido y a las componentes no pulsátiles. El movimiento, la luz ambiente y el acoplamiento del sensor pueden alterar la relación de señales, producir estimaciones inestables o lecturas erróneamente bajas y activar alarmas sin una desaturación arterial real. Una lectura baja también puede ser verdadera; por tanto, debe verificarse la calidad de la señal, el estado del sensor y el contexto clínico, y no desestimar automáticamente la alarma.

## Conclusiones

1. El montaje con el OxSim OX-1 permitió observar la respuesta del monitor uMEC 100 a cambios simulados de frecuencia de pulso y SpO₂.

2. Las lecturas puntuales de 40 bpm/95 % y 80 bpm/85 % coincidieron con las consignas descritas en la guía. Para otras condiciones se encontraron diferencias de 1 pp en SpO₂ bajo comparaciones condicionales.

3. La representación PPG es coherente con una relación inversa entre frecuencia y periodo de pulsación; su evaluación morfológica detallada requiere registros ampliados y estables.

4. Las capturas muestran indicaciones visuales compatibles con eventos de alarma, pero no bastan para medir el retardo de activación ni certificar el componente sonoro.

5. Para emitir un juicio metrológico de conformidad es indispensable verificar los manuales de los equipos, el sensor usado, las tolerancias aplicables y la incertidumbre del patrón.

## Organización del repositorio GitHub

Para cumplir la guía, crear el repositorio desde la cuenta de un integrante, invitar a los demás como colaboradores y comprobar que todos aparezcan con acceso y contribuciones registradas.

## Referencias y fuentes

[1] Universidad Militar Nueva Granada. Guía de preparación, práctica de laboratorio: Simulación y Monitoreo de Variables Cardiovasculares y Hemodinámicas, revisión 3, 2025.

[2] ISO 80601-2-61, Medical electrical equipment — Particular requirements for basic safety and essential performance of pulse oximeter equipment (referencia normativa general; verificar edición vigente).

[3] Manual de operación y especificaciones Mindray uMEC 100, pendiente de adjuntar/validar edición y configuración de sensor.

[4] Manual/ficha técnica Pronk OxSim OX-1, pendiente de adjuntar/validar edición.

## Anexo: evidencias visuales

![Fotograma del video 01](evidencias/video_01_medio.jpg)

![Fotograma del video 03](evidencias/video_03_medio.jpg)

![Fotograma del video 06](evidencias/video_06_medio.jpg)

![Fotograma del video 10](evidencias/video_10_medio.jpg)

