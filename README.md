

# Caso de Estudio: Inferencia Estadística para la Predicción y Control de Rockburst en Minería Subterránea

## Breve descripción de la actividad:
Desarrollo de un estudio de Data Science aplicado a la geotecnia para una mina subterránea. El proyecto consistió en el análisis inferencial de un dataset sintético para cuantificar la relación estadística entre la sismicidad, los esfuerzos del macizo rocoso (MPa) y las condiciones operacionales, con el fin de predecir eventos de daño dinámico o estallidos de roca (rockburst).
​

## Desafío principal que implicaba:
El reto analítico era demostrar de manera matemáticamente rigurosa —más allá de la simple intuición visual— si los niveles de esfuerzo estimado (stress_mpa) eran significativamente mayores durante los turnos donde ocurrían estallidos de roca. Además, el proyecto exigía cuantificar la incertidumbre de los datos y evaluar los riesgos operativos (Errores Tipo I y Tipo II) de implementar protocolos de alerta temprana basados en esta información.
​

## Solución propuesta:
Se aplicó el método científico estructurando un diseño observacional analítico. Se formularon hipótesis testables (H0 y H1) y se ejecutaron simulaciones de remuestreo (Bootstrapping) para validar el Teorema del Límite Central. Posteriormente, se calcularon intervalos de confianza paramétricos y se ejecutó un test de significancia (t-Student) comparando dos muestras independientes: un grupo de control (turnos sin incidentes) y el grupo de interés (turnos con rockburst).
​

## Herramientas técnicas utilizadas:

Lenguaje: Python.

Librerías: scipy.stats (tests de hipótesis y distribuciones), numpy, pandas (simulación y manipulación de datos), matplotlib/seaborn (visualización de diagramas de caja e histogramas).

Entorno: Jupyter Notebook / GitHub.
​

## Principales aprendizajes alcanzados:

Profundicé en la importancia crítica de la formulación correcta de hipótesis de negocio y cómo traducir un problema operativo de seguridad minera a un lenguaje estadístico evaluable.
​

Aprendí a interpretar el valor-p no solo como un número abstracto, sino en el contexto del impacto real: comprendiendo que minimizar el Error Tipo II (no detectar un peligro real) es vital cuando se trata de la seguridad de las personas y la infraestructura subterránea.
​

## Métricas de impacto logradas:

Validación estadística: Se rechazó la hipótesis nula con un altísimo nivel de confianza (valor-p = 0.00011, muy inferior al alfa de 0.05), demostrando estadísticamente que el esfuerzo medio en eventos con rockburst (49.35 MPa) es superior al de turnos normales (32.83 MPa).
​

Optimización de precisión: A través del análisis del tamaño muestral, se logró reducir drásticamente el margen de incertidumbre del intervalo de confianza para el esfuerzo poblacional, pasando de una amplitud de 21.63 MPa (con n=10) a solo 3.37 MPa (con n=200).
​

## Habilidades técnicas aplicadas:

Inferencia Estadística y Tests de Hipótesis (A/B testing conceptual).
​

Simulaciones estocásticas y Bootstrapping (Remuestreo).
​

Cálculo e interpretación de Intervalos de Confianza y Error Estándar.
​

Análisis de Probabilidades (Teorema de Bayes, Probabilidad Condicional, Árboles de Probabilidad).
​

## Justificación de por qué elegí este proyecto para formar parte del portafolio:
Elegí este proyecto porque demuestra mi capacidad para ir más allá de la construcción de modelos predictivos y aplicar un rigor matemático fundamental para entender la naturaleza de los datos. En la industria tecnológica, especialmente en roles de Data Science y análisis, la capacidad para validar causalidades con pruebas de significancia y comunicar los riesgos asociados a las decisiones basadas en datos es una competencia altamente valorada que complementa perfectamente mi conocimiento del negocio minero.
