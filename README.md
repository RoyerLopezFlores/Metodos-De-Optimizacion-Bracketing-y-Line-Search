# Simulador Interactivo de Métodos Numéricos de Optimización

Suite didáctica e interactiva desarrollada con **HTML5 Canvas**, renderizado dinámico de fórmulas matemáticas en **\LaTeX{} (KaTeX)** y **pseudocódigo con seguimiento reactivo de líneas**. 

Esta suite permite visualizar y experimentar de manera interactiva con los métodos numéricos de optimización en cualquier navegador web.

---

## 🚀 Métodos Disponibles

| Categoría | Método | Descripción Interactiva |
| :--- | :--- | :--- |
| **Bracketing** | [**Fibonacci Search**](fibonacci_search/index.html) | Acotamiento minimax óptimo con fórmula de Binet, cálculo de $\rho_i$, descarte de tramos y desempate final con $\epsilon$. |
| **Bracketing** | [**Golden Section Search**](golden_section_search/index.html) | Contracción geométrica estacionaria con la razón áurea ($\phi^{-1} \approx 0.618$) y reutilización automática de puntos interiores. |
| **Bracketing** | [**Quadratic Fit Search**](quadratic_fit_search/index.html) | Interpolación parabólica a tres puntos, cálculo analítico del vértice $x^*$ y convergencia superlineal acelerada. |
| **Bracketing** | [**Shubert-Piyavskii Method**](shubert_piyavskii/index.html) | Optimización global determinista basada en conos de Lipschitz ($\ell$) y cota inferior en diente de sierra (*sawtooth*). |
| **Local Descent** | [**Approximate Line Search**](approximate_line_search/index.html) | Descenso suficiente con condición de Armijo, retroceso geométrico (*backtracking*) de $\alpha$ y curvatura de Wolfe. |
| **Local Descent** | [**Trust Region Methods**](trust_region/index.html) | Restricción cuadrática en bola 2D de radio $\delta$ sobre la función de Rosenbrock y modulación adaptativa con el ratio $\eta$. |

---

## ✨ Características Principales

1. **Parametrización en Tiempo Real:** 
   - Modifica en vivo los intervalos $[a, b]$, punto inicial $x_0$, número de evaluaciones $n$, tolerancias $\epsilon$ / $\text{tol}$ o hiperparámetros ($\ell, \beta, p, \sigma, \delta, \eta_1, \eta_2$).
   - Botón **"Iniciar Optimización"** para recalcular el algoritmo instantáneamente.
2. **Cálculos Matemáticos en Vivo con KaTeX:**
   - Desglose analítico paso a paso con sustitución de números reales.
   - Evaluación explícita de condiciones lógicas (**Verdadero / Falso**) y decisiones de bifurcación.
3. **Pseudocódigo Reactivo:**
   - Resaltado luminoso (*line highlighting*) en la línea exacta del algoritmo que se está ejecutando.
4. **Controles de Reproducción:**
   - Botones **Paso Anterior**, **Siguiente Paso**, **Auto (Play/Pausa)** y **Reiniciar**.

---

## 📂 Estructura de Archivos

```text
graficos/
├── index.html                           # Galería y portal central de inicio
├── README.md                            # Guía de uso y despliegue
├── fibonacci_search/
│   └── index.html                       # Dashboard interactivo de Fibonacci
├── golden_section_search/
│   └── index.html                       # Dashboard interactivo de Sección Áurea
├── quadratic_fit_search/
│   └── index.html                       # Dashboard interactivo de Ajuste Cuadrático
├── shubert_piyavskii/
│   └── index.html                       # Dashboard interactivo de Shubert-Piyavskii
├── approximate_line_search/
│   └── index.html                       # Dashboard interactivo de Búsqueda Lineal
└── trust_region/
    └── index.html                       # Dashboard interactivo de Región de Confianza
```

