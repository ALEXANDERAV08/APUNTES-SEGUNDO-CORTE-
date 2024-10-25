# APUNTES-SEGUNDO-CORTE-
## NESTOR ALEXANDER AVILA 
## JUAN CAMILO VILLABON 
## ALEJANDRO MANRIQUE
##
##
# SISTEMAAS HIDRAULICOS 

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

# MOTOR DC POR CORRIENTE DE CAMPO 
En los motores de corriente continua con excitación separada o serie, el campo magnético se genera mediante una corriente de campo que circula por los devanados del estator, mientras que la armadura (rotor) 
es la parte giratoria. La velocidad y el par motor dependen tanto de la corriente de la armadura como de la corriente de campo.

## Ecuaciones fundamentales:

Vf=Rf⋅If+LfdI/dtf
​
 
 
## Donde:

𝑉𝑓: es el voltaje aplicado al circuito de campo.

𝐼𝑓: es la corriente de campo.

𝑅𝑓: es la resistencia del devanado de campo.

𝐿𝑓: es la inductancia del devanado de campo.
##
## Ecuación de la corriente de armadura:
##
$$V_a = R_a \cdot I_a + L_a \frac{dI_a}{dt} + E_b$$
##
# Donde:

$$𝑉_𝑎$$:   es el voltaje aplicado a la armadura.

$$𝐼_𝑎$$:   es la corriente de armadura.

$$𝑅_𝑎$$:  es la resistencia de la armadura.

$$𝐿_𝑎$$:  es la inductancia de la armadura.

$$𝐸_𝑏$$: es la fuerza contraelectromotriz (back-EMF), que es proporcional a la velocidad angular 
𝜔.
##
## PAR MOTOR (TORQUE):
$$T=K_t⋅ϕ⋅I_a$$
​
## Donde:

$$𝐾_𝑡$$: es la constante de torque del motor.

𝜙: es el flujo magnético generado por la corriente de campo.

$$𝐼_𝑎$$: es la corriente de armadura.

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

## Definición:

El modelo está compuesto por las siguientes partes:

### Parte Eléctrica
Describe cómo la corriente de campo $$i_c$$(t) cambia en respuesta al voltaje aplicado $$v_c$$(t) , las resistencias y las inductancias en el circuito de campo. La ecuación correspondiente es:

$$L_c \frac{di_c(t)}{dt} + R_c i_c(t) = v_c(t)$$

Donde:
- $$L_c$$: es la inductancia del devanado de campo.
- $$R_c$$: es la resistencia del devanado de campo.
- $$v_c(t)$$: es el voltaje aplicado al circuito de campo.

### Parte Magnética
Relaciona el flujo magnético Φ con la corriente de campo $$i_c$$(t) . El flujo magnético es proporcional a la corriente de campo a través de la constante  $$K_c$$, de manera que:


$$Φ = K_c i_c$$(t)


### Parte Mecánica
Describe la dinámica del par motor $$T_m$ y la velocidad angular w(t). El par motor es proporcional al flujo magnético Φ y a la corriente de armadura $$i_a$$(t):


$$T_m = K_a ⋅ K_c ⋅ i_a(t) ⋅ i_c(t)$$

La ecuación de movimiento para el sistema mecánico es:

$$J \frac{d^2\theta}{dt^2} + b \frac{d\theta}{dt} + k\theta = \tau(t)$$

Donde:
- J  es el momento de inercia.
- b  es el coeficiente de fricción.
- k  es la constante de rigidez (en caso de presencia de elementos elásticos).
- T(t) es el torque resultante.

## Ejemplo

Un ejemplo práctico del modelo por corriente de campo se encuentra en el control de velocidad de un motor de corriente continua. 
Variando la corriente de campo mediante el voltaje $$v_c$$(t), se puede controlar el flujo magnético  Φ y por lo tanto, ajustar el par motor $$T_m $$, lo que afectará la velocidad 
del motor.
