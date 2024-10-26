# APUNTES-SEGUNDO-CORTE-
## NESTOR ALEXANDER AVILA 
## JUAN CAMILO VILLABON 
## ALEJANDRO MANRIQUE
##
##
# Sistemas Eléctricos

Los sistemas eléctricos estudian el comportamiento y la evolución de sistemas eléctricos complejos a lo largo del tiempo, centrándose en cómo las variables internas y externas afectan su funcionamiento. Es especialmente relevante para redes eléctricas, donde el flujo de energía debe ser estable y confiable.

En esta área, los modelos de dinámica de sistemas ayudan a simular y prever cómo responden los sistemas eléctricos a cambios en la carga, generación, fallos y otras perturbaciones. Esto incluye el análisis de:

1. **Estabilidad de Voltaje**: Cómo el sistema mantiene niveles de voltaje dentro de un rango aceptable frente a fluctuaciones en la demanda o generación.

2. **Frecuencia de Operación**: Las redes eléctricas deben operar a una frecuencia constante (por ejemplo, 50 o 60 Hz), y las variaciones pueden causar problemas en la operación de equipos.

3. **Flujos de Potencia**: Analiza cómo se distribuye la energía en una red y se optimiza para minimizar pérdidas y maximizar la eficiencia.

4. **Control Automático y Respuesta a Contingencias**: Los sistemas eléctricos cuentan con dispositivos de control automático para ajustar voltaje, frecuencia y flujo de potencia en tiempo real, asegurando estabilidad en caso de fallos o picos de demanda.

5. **Dinámica de Generación y Demanda**: Evalúa cómo el sistema reacciona ante cambios en la generación de energía (por ejemplo, variabilidad en la producción de fuentes renovables) y en la demanda (por ejemplo, consumo industrial o doméstico).

![download](https://github.com/user-attachments/assets/cfb076c1-8efb-48c5-a30b-1f4a7db98923)
##
##
# Redes RLC

Las redes RLC son circuitos eléctricos compuestos por tres elementos básicos:

1. **Resistor (R)**: Limita el flujo de corriente y disipa energía en forma de calor.
2. **Inductor (L)**: Almacena energía en un campo magnético cuando la corriente fluye a través de él y se opone a cambios rápidos de corriente.
3. **Capacitor (C)**: Almacena energía en un campo eléctrico y se opone a cambios rápidos en el voltaje.

## Tipos de Redes RLC

Las redes RLC pueden ser configuradas en serie o en paralelo, con propiedades diferentes en cada caso:

- **RLC en Serie**: Los componentes R, L y C están conectados uno tras otro. En esta configuración, la corriente que pasa por cada elemento es la misma. La impedancia total se calcula sumando las impedancias individuales:

  
  $$Z = R + j\omega L - \frac{j}{\omega C}$$

  donde $$\omega$$ es la frecuencia angular $$\omega = 2\pi f$$.

- **RLC en Paralelo**: Los componentes R, L y C están conectados en paralelo. En esta configuración, el voltaje a través de cada componente es el mismo, pero la corriente se divide. La admitancia total se calcula como la suma de las admitancias individuales:


$$Y = \frac{1}{R} + j\omega C - \frac{j}{\omega L}$$

## Comportamiento Dinámico y Frecuencia de Resonancia

Un aspecto importante de las redes RLC es su frecuencia de resonancia $$(f_0\)$$, que ocurre cuando la impedancia total es puramente resistiva (sin parte imaginaria). Esto sucede cuando la reactancia inductiva y capacitiva se cancelan entre sí:


$$f_0 = \frac{1}{2 \pi \sqrt{LC}}$$


En esta frecuencia, el circuito responde con una amplitud máxima en la corriente o voltaje, dependiendo de la configuración.

## Aplicaciones

Las redes RLC se utilizan en diversos sistemas, como:

- **Filtros de Frecuencia**: Para seleccionar o bloquear ciertas frecuencias.
- **Sintonización en Radiofrecuencia**: Ajustando la frecuencia de resonancia, es posible seleccionar señales específicas en radios y transmisores.
- **Cortes de Pico o Sobretensión**: Usados en sistemas de protección para reducir picos de tensión o corriente.

---

# Leyes Fundamentales y Comportamiento de los Componentes en Redes RLC

El comportamiento de las redes RLC está gobernado por varias leyes y principios fundamentales de la electricidad.

## Leyes de Kirchhoff

1. **Ley de Corrientes de Kirchhoff (LCK)**: La suma de las corrientes que entran y salen de un nodo es cero. Esto se expresa como:

  $$ \sum I_{\text{entrada}} = \sum I_{\text{salida}}$$

2. **Ley de Voltajes de Kirchhoff (LVK)**: La suma de las caídas de voltaje alrededor de cualquier lazo cerrado es cero. Esto se representa como:

   
   $$\sum V = 0$$

## Ley de Ohm

La ley de Ohm establece la relación entre voltaje $$(V\)$$, corriente $$(I\)$$ y resistencia $$(R\)$$:


$$V = IR$$

## Comportamiento de los Capacitores (Carga y Descarga)

La carga y descarga de un capacitor en una red RLC son fenómenos transitorios:

- Durante la carga:

  
  $$V_C(t) = V_0 \left(1 - e^{-\frac{t}{RC}}\right)$$

- Durante la descarga:

  
  $$V_C(t) = V_0 e^{-\frac{t}{RC}}$$

## Comportamiento de los Inductores (Carga y Descarga)

La carga y descarga de un inductor se describen con las ecuaciones:

- Durante la carga:

  
  $$I_L(t) = I_0 \left(1 - e^{-\frac{tR}{L}}\right)$$

- Durante la descarga:


  $$I_L(t) = I_0 e^{-\frac{tR}{L}}$$

## Ecuación Diferencial de un Circuito RLC

Para un circuito RLC en serie, la ecuación diferencial que modela su comportamiento es:


$$L \frac{d^2q}{dt^2} + R \frac{dq}{dt} + \frac{q}{C} = 0$$

donde $$(q\)$$ es la carga en el capacitor.



# Amplificadores Operacionales

Los amplificadores operacionales tienen una gran ganancia de voltaje y pueden realizar funciones como amplificación, filtrado, integración y diferenciación.

## Principios Básicos del Amplificador Operacional

- **Entrada no inversora $$(+\)$$**: Incrementa el voltaje de salida si el voltaje en esta entrada aumenta.
- **Entrada inversora $$(-\)$$**: Incrementa el voltaje de salida en sentido opuesto si el voltaje en esta entrada aumenta.

## Configuraciones Comunes de Amplificadores Operacionales

1. **Amplificador Inversor**

   
   $$V_{\text{out}} = -\frac{R_f}{R_{\text{in}}} V_{\text{in}}$$

2. **Amplificador No Inversor**

   
   $$V_{\text{out}} = \left(1 + \frac{R_f}{R_{\text{in}}}\right) V_{\text{in}}$$

3. **Sumador Inversor**

   
   $$V_{\text{out}} = -\left(\frac{R_f}{R_1} V_1 + \frac{R_f}{R_2} V_2 + \cdots\right)$$

4. **Integrador**

   $$V_{\text{out}} = -\frac{1}{RC} \int V_{\text{in}} \, dt$$

5. **Diferenciador**

   
   $$V_{\text{out}} = -RC \frac{dV_{\text{in}}}{dt}$$

## Aplicaciones de los Amplificadores Operacionales

- **Filtros Activos**
- **Amplificadores de Instrumentación**
- **Osciladores**
- **Convertidores A/D y D/A**
- **Control de Retroalimentación**

---

# Amplificador No Inversor: Análisis con Leyes de Kirchhoff

Para analizar un amplificador no inversor:

1. **Estructura del Circuito**:
   - La señal de entrada $$(V_{\text{in}}$$) se aplica a la entrada no inversora.
   - La entrada inversora está conectada a un divisor de tensión formado por $$(R_1\)$$ y $$(R_f\)$$.

2. **Análisis con Leyes de Kirchhoff**:
   - Debido a la alta ganancia del amplificador, $$(V_+ = V_-\)$$.
   - La corriente de entrada es prácticamente cero.
#
#
# SISTEMAS HIDRAULICOS 

Los sistemas hidráulicos se refieren a aquellos que involucran el flujo de líquidos (generalmente agua o aceite) a través de conductos o dispositivos, utilizando principios como la presión y el caudal. 
Estos sistemas se modelan mediante ecuaciones que relacionan las variables como presión, caudal, volumen y resistencia hidráulica.

## Definición: 
Un sistema hidráulico es un conjunto de componentes interconectados (bombas, válvulas, conductos, etc.) que controlan el movimiento y la presión de un fluido, usando las leyes de la mecánica de fluidos. 
Se utilizan frecuentemente en maquinaria industrial, frenos y sistemas de potencia.
## Ejemplo: 
Un sistema de frenos hidráulico en un automóvil, donde el líquido de frenos se presiona para accionar las pinzas de freno.

## MODELO MOTO DC 
El modelo de un motor de corriente continua (DC) basado en la corriente de campo se refiere al análisis y representación matemática del motor, considerando el comportamiento de la corriente que fluye a 
través de los devanados de campo, que genera el campo magnético necesario para el funcionamiento del motor. A continuación se describe cómo se modela este tipo de motor.
![download](https://github.com/user-attachments/assets/044f1086-566b-4cd1-9a16-eb99f5f61b0c)

# MOTOR DC POR CORRIENTE DE CAMPO 
En los motores de corriente continua con excitación separada o serie, el campo magnético se genera mediante una corriente de campo que circula por los devanados del estator, mientras que la armadura (rotor) 
es la parte giratoria. La velocidad y el par motor dependen tanto de la corriente de la armadura como de la corriente de campo.
![images](https://github.com/user-attachments/assets/fbc94591-14a3-46ce-8dde-e14d25b28f0a)

## Ecuaciones fundamentales:

Vf=Rf⋅If+LfdI/dtf
​
 
 
## Donde:

**𝑉𝑓:** es el voltaje aplicado al circuito de campo.

**𝐼𝑓:** es la corriente de campo.

**𝑅𝑓:** es la resistencia del devanado de campo.

**𝐿𝑓:** es la inductancia del devanado de campo.
##
## Ecuación de la corriente de armadura:
##
$$V_a = R_a \cdot I_a + L_a \frac{dI_a}{dt} + E_b$$
##
# Donde:

**$$𝑉_𝑎$$:**   es el voltaje aplicado a la armadura.

**$$𝐼_𝑎$$:**   es la corriente de armadura.

**$$𝑅_𝑎$$:** es la resistencia de la armadura.

**$$𝐿_𝑎$$:**  es la inductancia de la armadura.

**$$𝐸_𝑏$$:** es la fuerza contraelectromotriz (back-EMF), que es proporcional a la velocidad angular 
𝜔.
##
## PAR MOTOR (TORQUE):
$$T=K_t⋅ϕ⋅I_a$$
​
## Donde:

**$$𝐾_𝑡$$:** es la constante de torque del motor.

**𝜙:** es el flujo magnético generado por la corriente de campo.

**$$𝐼_𝑎$$:** es la corriente de armadura.

## COMPORTAMIENTO DINAMICO DEL SISTEMA:
El comportamiento dinámico de un motor DC con control por corriente de campo se puede describir mediante un sistema de ecuaciones diferenciales que relacionan el flujo magnético 
𝜙, la corriente de armadura $$𝐼_𝑎$$, la corriente de campo $$𝐼_𝑓$$, y la velocidad 𝜔. El control de la corriente de campo permite modificar el flujo magnético 
𝜙, lo cual afecta tanto la velocidad como el par motor.
##

## Modelado en Dinámica de Sistemas:
En términos de dinámica de sistemas, el modelo por corriente de campo incluye la dinámica del devanado de campo (que determina cómo cambia el flujo magnético en función de la corriente de campo) 
y la interacción con la armadura (que determina el torque y la velocidad).

## Entrada: 
Voltaje aplicado al campo $$𝑉_𝑓$$, voltaje aplicado a la armadura $$𝑉_𝑎$$.
##
## Salida: 
Velocidad 𝜔 y torque 𝑇.

# Modelo por Corriente de Campo

El modelo por corriente de campo de un motor de corriente continua (DC) describe la relación entre las partes eléctricas, magnéticas y mecánicas del motor en función de la corriente que circula 
por el circuito de campo. Este tipo de modelado se utiliza principalmente para entender cómo la corriente de campo influye en el par y la velocidad del motor, controlando indirectamente el 
rendimiento del mismo.
![download](https://github.com/user-attachments/assets/28ecbd84-cd31-4dda-b082-d96ebe2817ff)

## Definición:

El modelo está compuesto por las siguientes partes:

### Parte Eléctrica
Describe cómo la corriente de campo $$i_c$$(t) cambia en respuesta al voltaje aplicado $$v_c$$(t) , las resistencias y las inductancias en el circuito de campo. La ecuación correspondiente es:

$$L_c \frac{di_c(t)}{dt} + R_c i_c(t) = v_c(t)$$

Donde:
- **$$L_c$$:** es la inductancia del devanado de campo.
- **$$R_c$$:** es la resistencia del devanado de campo.
- **$$v_c(t)$$:** es el voltaje aplicado al circuito de campo.

### Parte Magnética
Relaciona el flujo magnético Φ con la corriente de campo $$i_c$$(t) . El flujo magnético es proporcional a la corriente de campo a través de la constante  $$K_c$$, de manera que:


$$Φ = K_c i_c$$(t)


### Parte Mecánica
Describe la dinámica del par motor $$T_m$ y la velocidad angular w(t). El par motor es proporcional al flujo magnético Φ y a la corriente de armadura $$i_a$$(t):


$$T_m = K_a ⋅ K_c ⋅ i_a(t) ⋅ i_c(t)$$

La ecuación de movimiento para el sistema mecánico es:

$$J \frac{d^2\theta}{dt^2} + b \frac{d\theta}{dt} + k\theta = \tau(t)$$

Donde:
- **J**  es el momento de inercia.
- **b**  es el coeficiente de fricción.
- **k**  es la constante de rigidez (en caso de presencia de elementos elásticos).
- **T(t)** es el torque resultante.

## Ejemplo

Un ejemplo práctico del modelo por corriente de campo se encuentra en el control de velocidad de un motor de corriente continua. 
Variando la corriente de campo mediante el voltaje $$v_c$$(t), se puede controlar el flujo magnético  Φ y por lo tanto, ajustar el par motor $$T_m $$, lo que afectará la velocidad 
del motor.
