# Proyecto Final de Cálculo 2, Sección B

Este repositorio contiene el proyecto final del curso de Cálculo 2 (Sección B). A continuación se detalla la preparación del entorno de trabajo, las herramientas a instalar y los pasos básicos para crear y ejecutar notebooks en VS Code que se usan en el desarrollo del proyecto.

# Guía para preparar entorno, instalar librerías, configurar Jupyter Notebook en VS Code y crear un proyecto sencillo

## 1. Instalación de Python y librerías necesarias

1. **Instalar Python 3**

   - Descarga e instala Python desde la página oficial: [https://www.python.org/downloads/](https://www.python.org/downloads/).
   - Verifica la instalación:
     ```bash
     python --version
     ```

2. **Instalar librerías con pip** Abre una terminal y escribe:

   ```bash
   pip install numpy matplotlib jupyter
   ```

   Estas librerías se usarán para cálculos numéricos, graficar y correr Jupyter Notebook.

---

## 2. Configuración de Visual Studio Code

1. Descarga e instala **Visual Studio Code**: [https://code.visualstudio.com/](https://code.visualstudio.com/)
2. Instala la extensión **Python** (oficial de Microsoft).
3. Instala la extensión **Jupyter** (también de Microsoft).

Con estas dos extensiones podrás correr notebooks (`.ipynb`) directamente en VS Code.

---

## 3. Crear un nuevo proyecto con Jupyter Notebook en VS Code

1. Abre VS Code y crea una carpeta para tu proyecto.
2. Dentro de la carpeta, crea un archivo nuevo con extensión `.ipynb`, por ejemplo:
   ```
   mi_proyecto.ipynb
   ```
3. VS Code reconocerá el archivo como un Notebook y mostrará celdas para escribir código y texto.

---

## 4. Ejemplo sencillo con una gráfica

En una celda del notebook, escribe el siguiente código:

```python
import numpy as np
import matplotlib.pyplot as plt

# Datos de ejemplo
x = np.linspace(0, 10, 100)
y = np.sin(x)

# Gráfica
plt.plot(x, y, label="y = sin(x)")
plt.xlabel("Eje X")
plt.ylabel("Eje Y")
plt.title("Ejemplo de Gráfica en Python")
plt.legend()
plt.show()
```

Cuando ejecutes la celda, se mostrará una gráfica de la función seno.

---

## 5. Ejecutar el proyecto en VS Code

1. Abre el archivo `mi_proyecto.ipynb` en VS Code.
2. Selecciona un intérprete de Python (arriba a la derecha, donde aparece `Select Kernel`).
3. Haz clic en el botón ▶️ al lado de cada celda para ejecutar el código.
4. Los resultados aparecerán debajo de la celda.

---

✅ Con estos pasos tendrás tu entorno listo, un notebook funcionando en VS Code, y una primera gráfica creada con Python.

---

## 6. Sección del proyecto

Resumen del proyecto (extraído del PDF):

Este proyecto integra conceptos de Cálculo II con aplicaciones prácticas en aprendizaje automático para visualizar geométricamente el proceso de optimización mediante gradiente descendente en una neurona con activación sigmoide. La propuesta busca que el estudiante implemente en Python la función sigmoide, la función de costo (error cuadrático medio) y utilice derivadas parciales y gradiente descendente para minimizar la función de costo.

Objetivos principales:
- General: Comprender y aplicar derivadas parciales y gradiente descendente en la minimización de la función de costo de una neurona con activación sigmoide.
- Específicos: implementar la sigmoide y la función de costo en Python; generar la superficie de error 3D en función de los pesos (w1, w2); analizar la forma de la cuenca de error y localizar su mínimo.

Metodología (resumen):
- Usar un conjunto de datos sencillo (por ejemplo la compuerta lógica AND) con entradas X y salidas y.
- Definir funciones en Python: sigmoid(z), predict(X,w1,w2,b) y cost_function(w1,w2,X,y,b).
- Generar una malla de valores para w1 y w2 con NumPy y calcular la superficie de error evaluando la función de costo en cada punto.
- Visualizar la superficie con Matplotlib en 3D para identificar la cuenca de error y el mínimo.

Entregables:
1. Código fuente (notebook) con el código comentado.
2. Gráfica 3D de la superficie de error.
3. Informe final que explique la implementación, resultados y conclusiones.

Puedes consultar el documento completo del proyecto en formato PDF incluido en este repositorio:

- Archivo: `Cálculo_2_Proyecto_Final.pdf`
- Enlace directo al PDF: [Consultar PDF del proyecto](./Cálculo_2_Proyecto_Final.pdf)
