# ⚡ Modelamiento de Sistemas Eléctricos

El modelamiento de sistemas eléctricos consiste en representar circuitos eléctricos mediante ecuaciones matemáticas que describen su comportamiento dinámico. Utilizando leyes fundamentales como la Ley de Ohm, la Ley de Kirchhoff de Corrientes (LKC) y la Ley de Kirchhoff de Voltajes (LKV), es posible obtener modelos que predicen la respuesta de un circuito ante señales de entrada.

---

## 🔑 Conceptos Clave

- **Voltaje (V):** Diferencia de potencial eléctrico entre dos puntos.
- **Corriente (I):** Flujo de carga eléctrica en un conductor.
- **Resistencia (R):** Oposición al flujo de corriente.
- **Inductancia (L):** Propiedad que se opone a cambios de corriente.
- **Capacitancia (C):** Capacidad de almacenar energía en forma de campo eléctrico.
- **Transformada de Laplace:** Herramienta matemática que convierte ecuaciones diferenciales en algebraicas para facilitar el análisis.

---

## 🛠️ Aplicaciones

- Modelado de fuentes de energía.
- Análisis de filtros eléctricos (pasa bajos, pasa altos).
- Diseño de sistemas de control en electrónica.
- Simulación de circuitos en software como MATLAB/Simulink o LTSpice.

---

## 📚 Ejemplo 1: Circuito RL

**Descripción:** Un circuito en serie con una resistencia R, una inductancia L y una fuente de voltaje \( V(t) \).

### Ecuación diferencial:

```math
V(t) = L \frac{dI(t)}{dt} + R I(t)
```

### Función de transferencia:

```math
\frac{I(s)}{V(s)} = \frac{1}{Ls + R}
```

![Circuito RL]([https://upload.wikimedia.org/wikipedia/commons/thumb/b/b9/RL_circuit.svg/320px-RL_circuit.svg.png])
---

## 📚 Ejemplo 2: Circuito RLC serie

**Descripción:** Un circuito con una resistencia R, una inductancia L y un condensador C en serie con una fuente de voltaje.

### Ecuación diferencial:

```math
V(t) = L \frac{d^2q(t)}{dt^2} + R \frac{dq(t)}{dt} + \frac{q(t)}{C}
```

(Usando \( I(t) = \frac{dq(t)}{dt} \), se puede transformar a lazo de corriente).

### Función de transferencia (de V(s) a I(s)):

```math
\frac{I(s)}{V(s)} = \frac{1}{L s^2 + R s + \frac{1}{C}}
```

![Circuito RLC](https://upload.wikimedia.org/wikipedia/commons/thumb/3/34/RLC_series.svg/320px-RLC_series.svg.png)

---

## Conclusión

El modelamiento de sistemas eléctricos permite analizar, diseñar y optimizar circuitos y dispositivos que forman parte de sistemas electrónicos y de control. Al traducir componentes eléctricos en modelos matemáticos, se facilita la simulación y predicción del comportamiento ante diversas condiciones. Esta habilidad es esencial en ingeniería eléctrica, electrónica y mecatrónica.

## Referencias

 
Universidad del País Vasco. (s.f.). Capítulo 3: El modelo keynesiano I. OpenCourseWare UPV/EHU. Recuperado el 13 de abril de 2025, de https://ocw.ehu.eus/file.php/83/cap31_html/capitulo-3.html

carakenio73. "Dinámica de un sistema masa-resorte-amortiguador." dademuchconnection, 18 de julio de 2017, https://dademuchconnection.wordpress.com/2017/07/18/dinamica-de-un-sistema-masa-resorte-amortiguador/.

 

