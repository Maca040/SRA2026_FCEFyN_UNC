
# Síntesis de Redes Activas 

Este repositorio contiene scripts en Python y Jupyter Notebooks desarrollados para complementar los contenidos teóricos y prácticos de la asignatura **Síntesis de Redes Activas** (Ingeniería Electrónica - FCEFyN, Universidad Nacional de Córdoba).

El objetivo del proyecto es facilitar la comprensión física y matemática de los circuitos activos, permitiendo pasar de las deducciones analíticas en papel a la resolución simbólica exacta, el trazado de curvas de diseño y la verificación numérica.

---

## Contenido del Repositorio

El material se organiza combinando el desarrollo teórico paso a paso (en bloques Markdown) con su implementación en código:

1. **Análisis de Configuraciones y Funciones de Transferencia con Lcapy:**
   * La libreria de Lcapy permite una resolución simbólica automatizada de las distintas topologías de amplificadores operacionales vistas en la materia (configuraciones inversora, no inversora, amplificador diferencial, integrador) con sus respectivas funciones de transferencia.

2. **Estabilidad:**
   * Deducción analítica del modelo dinámico de segundo orden en lazo cerrado a partir de un amplificador operacional real de dos polos aplicando el modelo general de Blackman.
   * Obtención y resolución de las ecuaciones bicuadráticas para el ancho de banda normalizado (**3dB;ωH**), la frecuencia de cruce de ganancia (**ωG**) y el margen de fase **Mφ** en función del factor de calidad **Qp**.
   * Identificación de puntos críticos de diseño: Máxima Planicidad de Retardo (**MPR**) y Máxima Planicidad de Módulo (**MPM**)

---
## Instalación y Uso (Google Colab)

 Descargar los archivos .ipynb e importarlos en Google Colab. 
 En los archivos que tengan lcapy agregar una nueva celda de código al inicio del notebook con lo siguiente : 
 
   ```bash
      # Instalar dependencias del sistema
      !apt-get update -qq
      !apt-get install -y -qq \
          texlive-latex-base \
          texlive-latex-recommended \
          texlive-latex-extra \
          texlive-pictures \
          texlive-fonts-recommended \
          cm-super \
          dvipng \
          ghostscript \
          poppler-utils
      # Instalar Lcapy
      %pip install -q lcapy
   ```
## Instalación y Uso (localmente)
1. Clonar el repositorio en tu máquina local:
   ```bash
   git clone https://github.com/Maca040/SRA2026_FCEFyN_UNC
   ```
2. Ingresar a la carpeta de "SRA2026_FCEFyN_UNC"
3. Instalar las dependencias necesarias:
   ```bash
   pip install numpy scipy matplotlib sympy lcapy jupyter
   ```


