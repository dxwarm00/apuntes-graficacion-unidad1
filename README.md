# Unidad I – Introducción a la Graficación por Computadora

**Materia:** Graficación por Computadora  
**Unidad:** I  
**Tipo de documento:** Investigación documental y aplicación práctica  

---

> Documento académico digital desarrollado en formato interactivo.

---

## Indice

- [1.1 Historia y evolución de la graficación por computadora](#11-historia-y-evolución-de-la-graficación-por-computadora)
- [1.2 Áreas de aplicación](#12-áreas-de-aplicación)
- [1.3 Aspectos matemáticos de la graficación](#13-aspectos-matemáticos-de-la-graficación)
- [1.4 Modelos del color RGB, CMY, HSV y HSL](#14-modelos-del-color-rgb-cmy-hsv-y-hsl)
- [Tutorial Iluminación básica en Blender](#tutorial-iluminación-básica-en-blender)
- [1.5 Representación y trazo de líneas y polígonos](#15-representación-y-trazo-de-líneas-y-polígonos)
- [1.5.1 Formatos de imagen](#151-formatos-de-imagen)
- [1.6 Procesamiento de mapas de bits](#16-procesamiento-de-mapas-de-bits)
- [Conclusion](#conclusion)
- [Bibliografia](#bibliografia)
---

## 1.1 Historia y evolución de la graficación por computadora

### Orígenes (1960–1970)

La graficación por computadora surge formalmente en 1963 con el sistema **Sketchpad**, desarrollado por Ivan Sutherland en el MIT. Este sistema permitió dibujar figuras directamente en una pantalla mediante un lápiz óptico, marcando el inicio de los gráficos interactivos.

En esta etapa predominaban los **gráficos vectoriales**, donde las imágenes se representaban mediante ecuaciones matemáticas en lugar de píxeles. Cada línea y figura era descrita a través de coordenadas y funciones matemáticas.

---

### Expansión industrial (1970–1990)

Con el avance del hardware y el desarrollo de microprocesadores más potentes, surgieron los **gráficos rasterizados**, basados en matrices de píxeles.

Durante este periodo se consolidaron sistemas como:

- CAD (Computer-Aided Design)
- CAM (Computer-Aided Manufacturing)
- Simuladores industriales
- Modelado arquitectónico digital

La graficación comenzó a utilizarse en ingeniería, manufactura y diseño estructural.

---

### Revolución de las GPU (1990–2005)

La incorporación de **tarjetas gráficas dedicadas (GPU)** transformó la industria digital.

Se desarrollaron técnicas fundamentales como:

- Z-buffer
- Mapeo de texturas
- Sombreado programable
- Renderizado en tiempo real

Esto permitió la expansión de los videojuegos 3D, simuladores y animación digital.

---

### Era moderna (2005–Actualidad)

Actualmente, la graficación por computadora integra:

- Modelado 3D avanzado
- Renderizado basado en física (PBR)
- Ray tracing en tiempo real
- Simulación física
- Realidad virtual y aumentada

El desarrollo de motores gráficos y software como Blender ha democratizado el acceso a herramientas profesionales de creación digital.

---

### Línea temporal resumida

1963 → Sketchpad y gráficos vectoriales  
1980 → Consolidación del CAD y gráficos raster  
1990 → GPU y videojuegos 3D  
2000 → Renderizado en tiempo real  
Actualidad → Ray tracing y simulación avanzada  

---

### Conclusión del apartado

La evolución de la graficación por computadora está estrechamente ligada al desarrollo del hardware y de los modelos matemáticos que permiten representar digitalmente el espacio tridimensional. Su progreso ha impactado áreas industriales, científicas y artísticas, consolidándose como una disciplina fundamental en la tecnología moderna.

---

## 1.2 Áreas de aplicación

La graficación por computadora tiene aplicaciones en múltiples disciplinas científicas, técnicas y artísticas. Su capacidad para representar información visualmente permite modelar, simular y analizar fenómenos complejos.

---

### 1.2.1 Ingeniería y arquitectura

En ingeniería, la graficación se utiliza principalmente en sistemas **CAD (Computer-Aided Design)** para:

- Diseño mecánico
- Modelado estructural
- Simulación de piezas
- Visualización de ensamblajes

En arquitectura permite:

- Modelado 3D de edificaciones
- Renderizado de interiores y exteriores
- Simulación de iluminación
- Representaciones fotorrealistas de proyectos

---

### 1.2.2 Medicina y ciencia

En el área médica, la graficación por computadora es fundamental en:

- Reconstrucciones 3D de órganos
- Visualización de tomografías y resonancias
- Simulación quirúrgica
- Modelado anatómico

En la investigación científica se utiliza para:

- Visualización de datos
- Simulación de fenómenos físicos
- Representación de modelos matemáticos complejos

---

### 1.2.3 Entretenimiento digital

Una de las áreas más conocidas es el entretenimiento:

- Videojuegos
- Animación 3D
- Cine digital
- Efectos visuales (VFX)

La implementación de motores gráficos permite el renderizado en tiempo real, simulaciones físicas y entornos interactivos.

---

### 1.2.4 Simulación y entrenamiento

Se emplea en:

- Simuladores de vuelo
- Entrenamiento militar
- Simuladores de conducción
- Realidad virtual

Estos sistemas permiten recrear entornos controlados para capacitación sin riesgos físicos.

---

### 1.2.5 Visualización de datos y análisis

En ciencia de datos y estadística, la graficación permite:

- Representar grandes volúmenes de información
- Detectar patrones
- Interpretar tendencias
- Facilitar la toma de decisiones

---

### Relación con herramientas actuales

Software como Blender integra muchas de estas aplicaciones, permitiendo:

- Modelado 3D
- Simulación física
- Iluminación avanzada
- Animación
- Renderizado fotorrealista

Esto demuestra cómo los fundamentos teóricos se aplican en herramientas modernas de creación digital.

---

### Conclusión del apartado

La graficación por computadora no se limita al ámbito artístico, sino que constituye una herramienta transversal en ingeniería, medicina, simulación y análisis científico. Su evolución tecnológica ha ampliado constantemente sus campos de aplicación, consolidándola como una disciplina esencial en el desarrollo tecnológico contemporáneo.

---

## 1.3 Aspectos matemáticos de la graficación

La graficación por computadora se fundamenta en modelos matemáticos que permiten representar, transformar y proyectar objetos dentro de un espacio digital. Las principales áreas involucradas son el álgebra lineal, la geometría analítica y la trigonometría.

---

### 1.3.1 Sistemas de coordenadas

Todo objeto gráfico se define mediante coordenadas.

En dos dimensiones:

$$
(x, y)
$$

En tres dimensiones:

$$
(x, y, z)
$$

Cada vértice de un modelo 3D es un punto dentro de un sistema cartesiano. A partir de estos puntos se construyen aristas, caras y superficies.

---

### 1.3.2 Transformaciones geométricas

Las transformaciones permiten modificar posición, tamaño y orientación de los objetos.

---

#### Traslación

La traslación desplaza un objeto en el espacio mediante un vector:

$$
x' = x + t_x
$$

$$
y' = y + t_y
$$

$$
z' = z + t_z
$$

En el escenario procedural desarrollado, cada cubo fue posicionado mediante traslaciones en el eje Y:

```python
bpy.ops.mesh.primitive_cube_add(location=(-ancho_pasillo, i * 2, 1))
```

Aquí, el término `i * 2` representa el desplazamiento progresivo.

---

#### Escalamiento

El escalamiento modifica el tamaño del objeto mediante factores multiplicativos:

$$
x' = s_x \cdot x
$$

$$
y' = s_y \cdot y
$$

$$
z' = s_z \cdot z
$$

En el proyecto, cuando se utilizó:

```python
pared_izq.scale.z = 1.5
```

se aplicó un escalamiento vertical.

---

#### Rotación en el plano

La rotación en 2D utiliza funciones trigonométricas:

$$
x' = x\cos\theta - y\sin\theta
$$

$$
y' = x\sin\theta + y\cos\theta
$$

Este principio fue aplicado en la generación del tramo curvo del escenario:

```python
x = cx + radio_curva * math.cos(angulo)
y = cy + radio_curva * math.sin(angulo)
```

Aquí, seno y coseno permiten distribuir objetos sobre una circunferencia.

---

### 1.3.3 Matrices de transformación

En graficación avanzada, las transformaciones se representan mediante matrices.

La matriz de rotación en 2D se expresa como:

$$
R(\theta) =
\begin{bmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{bmatrix}
$$

Multiplicar un vector por esta matriz produce su rotación.

Las matrices permiten combinar múltiples transformaciones en una sola operación, optimizando cálculos en motores gráficos.

---

### 1.3.4 Coordenadas homogéneas

Para integrar la traslación dentro del sistema matricial se utilizan coordenadas homogéneas, agregando un cuarto componente:

$$
(x, y, z, 1)
$$

Esto permite expresar todas las transformaciones como multiplicaciones de matrices 4×4, fundamentales en gráficos 3D.

---

### 1.3.5 Interpolación y animación

La animación digital utiliza interpolación para calcular valores intermedios entre dos posiciones.

En el proyecto integrador, la cámara se animó modificando progresivamente el parámetro `offset_factor`, lo cual implica una interpolación lineal entre:

$$
0 \leq t \leq 1
$$

donde el valor cambia gradualmente entre el fotograma inicial y final.

---

### Relación con las prácticas realizadas

- El polígono 2D utilizó trigonometría para calcular vértices uniformemente distribuidos.
- La Flor de la Vida aplicó distribución angular mediante:
$$
\theta = \frac{360^\circ}{n}
$$
- El escenario procedural aplicó traslación, rotación y escalamiento.
- La animación utilizó interpolación de parámetros.

---

### Conclusión del apartado

La graficación por computadora es una aplicación directa del álgebra lineal y la trigonometría. Cada modelo 3D, animación o simulación es el resultado de operaciones matemáticas precisas que permiten representar el espacio digital de manera coherente y eficiente.

## 1.4 Modelos del color: RGB, CMY, HSV y HSL

El color en graficación por computadora se representa mediante modelos matemáticos que permiten describir tonalidades de forma numérica. Cada modelo responde a una necesidad distinta, ya sea para dispositivos digitales, impresión o manipulación visual.

---

### 1.4.1 Modelo RGB (Red, Green, Blue)

El modelo RGB es un sistema aditivo basado en la combinación de luz.

Cada color se representa como una combinación de:

- R (Rojo)
- G (Verde)
- B (Azul)

Matemáticamente:

$$
Color = (R, G, B)
$$

donde:

$$
0 \leq R, G, B \leq 255
$$

En este modelo:

- (0, 0, 0) = negro  
- (255, 255, 255) = blanco  

Este modelo es utilizado en pantallas, monitores y renderizado digital.

En el proyecto procedural se utilizó RGB al definir materiales:

```python
bsdf.inputs['Base Color'].default_value = (*color_rgb, 1.0)
```

---

### 1.4.2 Modelo CMY (Cyan, Magenta, Yellow)

El modelo CMY es un sistema sustractivo utilizado en impresión.

Se basa en la absorción de luz:

- Cian absorbe rojo
- Magenta absorbe verde
- Amarillo absorbe azul

Relación aproximada con RGB:

$$
C = 1 - R
$$
$$
M = 1 - G
$$
$$
Y = 1 - B
$$

(Valores normalizados entre 0 y 1)

Cuando se añade negro (K) se obtiene el modelo CMYK utilizado en imprentas.

---

### 1.4.3 Modelo HSV (Hue, Saturation, Value)

El modelo HSV organiza el color de forma más intuitiva para el usuario.

- Hue (Tono): ángulo en la rueda de color
- Saturation (Saturación): intensidad del color
- Value (Valor): brillo

El tono se representa como:

$$
0^\circ \leq H < 360^\circ
$$

Este modelo es útil en interfaces gráficas y herramientas de edición.

---

### 1.4.4 Modelo HSL (Hue, Saturation, Lightness)

Similar al HSV, pero utiliza Lightness (luminosidad) en lugar de Value.

La luminosidad se define como:

$$
L = \frac{\text{máximo}(R,G,B) + \text{mínimo}(R,G,B)}{2}
$$

Este modelo facilita ajustes de iluminación y contraste.

---

### Comparación de modelos

| Modelo | Tipo | Uso principal | Aplicación |
|--------|------|---------------|------------|
| RGB | Aditivo | Pantallas digitales | Renderizado |
| CMY | Sustractivo | Impresión | Diseño gráfico |
| HSV | Perceptual | Edición de color | Interfaces |
| HSL | Perceptual | Ajustes de luz | Diseño visual |

---

## Tutorial: Iluminación básica en Blender

La iluminación es fundamental para percibir el color correctamente.

### Paso 1 – Crear un cubo

```python
bpy.ops.mesh.primitive_cube_add(size=2, location=(0, 0, 0))
```

---

### Paso 2 – Asignar material RGB

```python
mat = bpy.data.materials.new(name="MaterialColor")
mat.use_nodes = True
bsdf = mat.node_tree.nodes["Principled BSDF"]
bsdf.inputs['Base Color'].default_value = (0.2, 0.5, 0.8, 1)
bpy.context.active_object.data.materials.append(mat)
```

---

### Paso 3 – Agregar luz tipo SUN

```python
bpy.ops.object.light_add(type='SUN', location=(5, 5, 5))
```

---

### Paso 4 – Renderizar

La percepción del color dependerá de:

- Intensidad de la luz
- Dirección
- Rugosidad del material
- Modelo de color aplicado

---

### Evidencia visual en Blender

La siguiente imagen muestra un cubo con material definido en el modelo RGB e iluminado mediante una fuente de luz tipo SUN.

<p align="center">
<img width="833" height="478" alt="image" src="https://github.com/user-attachments/assets/242374e5-bd99-4c4c-b935-3be1df793ab2" width="300">
<img width="876" height="503" alt="image" src="https://github.com/user-attachments/assets/7f5c413b-d1af-46f0-b1ce-d1d68da8e246" width="300">
</p>

### Conclusión del apartado

Los modelos de color permiten representar digitalmente la luz y la pigmentación mediante valores numéricos. En graficación por computadora, el modelo RGB domina en entornos digitales, mientras que HSV y HSL facilitan la manipulación visual. La iluminación en motores gráficos como Blender demuestra cómo estos modelos interactúan con materiales y fuentes de luz.

## 1.5 Representación y trazo de líneas y polígonos

La representación de líneas y polígonos constituye la base de la construcción gráfica digital. Todo modelo 3D está compuesto por vértices, aristas y caras que forman estructuras geométricas.

---

### 1.5.1.1 Representación vectorial vs raster

Existen dos formas principales de representar gráficos:

#### Representación vectorial

Describe las figuras mediante ecuaciones matemáticas.

Ejemplo:
Una línea puede definirse mediante la ecuación:

$$
y = mx + b
$$

Ventajas:
- Escalable sin pérdida de calidad
- Basada en coordenadas matemáticas
- Ideal para modelado 3D

Blender trabaja principalmente con representación vectorial.

---

#### Representación raster (mapa de bits)

Representa imágenes como una matriz de píxeles.

Cada píxel contiene información de color:

$$
Imagen = matriz(x, y)
$$

Ventajas:
- Ideal para fotografías
- Compatible con pantallas digitales

Desventajas:
- Pierde calidad al escalar

---

### 1.5.2.1 Trazado de líneas

Para dibujar líneas en pantallas rasterizadas se utilizan algoritmos específicos.

Uno de los más importantes es el **Algoritmo de Bresenham**, que permite determinar qué píxeles activar para aproximar una línea recta utilizando únicamente operaciones enteras.

Este algoritmo es fundamental en sistemas gráficos de bajo nivel.

---

### 1.5.3.1 Representación de polígonos

Un polígono se define como un conjunto de vértices conectados por aristas.

En términos matemáticos, si un polígono tiene \( n \) lados, sus vértices pueden calcularse mediante:

$$
\theta = \frac{360^\circ}{n}
$$

Y sus coordenadas:

$$
x = r\cos\theta
$$

$$
y = r\sin\theta
$$

Este principio fue aplicado en la práctica del polígono 2D mediante scripting en Blender.

---

### Relación con las prácticas desarrolladas

- La práctica del polígono utilizó trigonometría para generar vértices uniformemente distribuidos.
  
<img width="1001" height="501" alt="image" src="https://github.com/user-attachments/assets/6d5d023c-63e5-43d4-92a5-c472b332040f" />

- La Flor de la Vida aplicó repetición angular para formar patrones geométricos.
  
<img width="884" height="604" alt="image" src="https://github.com/user-attachments/assets/05c4d5da-50e4-483a-87a0-f3152750170e" />
<img width="1052" height="560" alt="image" src="https://github.com/user-attachments/assets/2dc17cbf-dfa9-45ba-8a2c-b48018dcf4da" />

- Ambos ejercicios demuestran cómo los fundamentos matemáticos permiten construir estructuras complejas a partir de reglas simples.

---

### Conclusión del apartado

La representación digital de líneas y polígonos es el fundamento estructural de la graficación por computadora. Ya sea en formato vectorial o raster, todo sistema gráfico depende de modelos matemáticos para describir y renderizar formas en pantalla.

---

### 1.5.1 Formatos de imagen

Los formatos de imagen determinan cómo se almacena y comprime la información visual en un archivo digital. En graficación por computadora, comprender sus diferencias es esencial para elegir el formato adecuado según el uso.

---

#### Imágenes raster

Las imágenes raster (mapa de bits) almacenan la información como una matriz de píxeles:

$$
Imagen = f(x, y)
$$

Cada píxel contiene valores de color (generalmente en RGB).

---

#### Principales formatos

##### PNG (Portable Network Graphics)

- Compresión sin pérdida
- Soporta transparencia (canal alfa)
- Ideal para gráficos digitales y renders

##### JPEG / JPG (Joint Photographic Experts Group)

- Compresión con pérdida
- Reduce tamaño de archivo
- Ideal para fotografías
- No recomendable para imágenes con texto o bordes definidos

##### BMP (Bitmap)

- Sin compresión
- Archivos grandes
- Uso histórico en sistemas Windows

##### TIFF (Tagged Image File Format)

- Alta calidad
- Soporta múltiples capas
- Usado en impresión profesional

##### GIF (Graphics Interchange Format)

- Limitado a 256 colores
- Soporta animaciones
- Ideal para secuencias cortas (como la animación del proyecto)

---

### Comparación técnica

| Formato | Tipo de compresión | Transparencia | Uso recomendado |
|----------|-------------------|--------------|------------------|
| PNG | Sin pérdida | Sí | Render y gráficos digitales |
| JPEG | Con pérdida | No | Fotografías |
| BMP | Sin compresión | No | Uso básico |
| TIFF | Sin pérdida | Sí | Impresión profesional |
| GIF | Con pérdida limitada | Sí | Animaciones cortas |

---

### Relación con las prácticas

En el proyecto integrador:

- El render del escenario puede exportarse como **PNG** para mantener calidad.
- La animación del recorrido se exportó como **GIF** para visualización en GitHub.
- La elección del formato influye en la calidad y peso del archivo final.


![AnimationEscenario](https://github.com/user-attachments/assets/d5f492e9-3669-4d56-a7fa-9d0db10376a3)


---

### Conclusión del apartado

La selección del formato de imagen impacta directamente en la calidad visual, tamaño del archivo y compatibilidad. En entornos digitales como Blender y GitHub, el formato PNG es ideal para imágenes estáticas, mientras que GIF permite representar animaciones cortas.

## 1.6 Procesamiento de mapas de bits

El procesamiento de mapas de bits consiste en la manipulación directa de imágenes rasterizadas, es decir, imágenes compuestas por una matriz de píxeles donde cada elemento contiene información de color.

En términos matemáticos, una imagen digital puede representarse como:

$$
I(x, y) = (R, G, B)
$$

donde cada coordenada $(x, y)$ corresponde a un píxel con valores de color.

---

### 1.6.1 Resolución

La resolución determina la cantidad de píxeles que componen una imagen.

Se expresa como:

$$
Resolución = ancho \times alto
$$

Por ejemplo:

1920 × 1080 = 2,073,600 píxeles.

A mayor resolución:
- Mayor detalle
- Mayor peso de archivo
- Mayor consumo de memoria

---

### 1.6.2 Profundidad de color

La profundidad de color indica cuántos bits se utilizan para representar el color de cada píxel.

Ejemplo común:

- 8 bits por canal (RGB)
- Total: 24 bits por píxel

Número de colores posibles:

$$
2^{24} = 16,777,216 \text{ colores}
$$

Esto permite representar imágenes con alta fidelidad cromática.

---

### 1.6.3 Operaciones sobre píxeles

El procesamiento digital de imágenes incluye operaciones como:

- Ajuste de brillo
- Contraste
- Conversión a escala de grises
- Aplicación de filtros
- Detección de bordes

Por ejemplo, una conversión simple a escala de grises puede aproximarse como:

$$
Gris = \frac{R + G + B}{3}
$$

---

### 1.6.4 Compresión de imágenes

Los mapas de bits pueden comprimirse para reducir tamaño de archivo.

Existen dos tipos principales:

- Compresión sin pérdida (PNG, TIFF)
- Compresión con pérdida (JPEG)

La compresión con pérdida elimina información visual menos perceptible para el ojo humano.

---

### 1.6.5 Relación con el renderizado en Blender

Cuando se renderiza una escena en Blender:

- El resultado final es un mapa de bits.
- Cada píxel es calculado mediante algoritmos de iluminación.
- La calidad depende de:
  - Resolución
  - Muestras de render
  - Profundidad de color
  - Formato de exportación

La exportación en PNG preserva calidad sin pérdida, mientras que JPEG reduce tamaño sacrificando información visual.

---

### Conclusión del apartado

El procesamiento de mapas de bits es fundamental en la etapa final de la graficación por computadora. Aunque el modelado y las transformaciones se basan en representaciones vectoriales, el resultado visible siempre termina siendo una imagen raster compuesta por millones de píxeles calculados matemáticamente.

---

## Conclusion

La graficacion por computadora integra fundamentos matematicos, modelos de color y tecnicas de representacion digital que permiten construir entornos visuales complejos a partir de principios geometricos y algebraicos.

A lo largo de la Unidad I se analizaron:

- La evolucion historica de la disciplina
- Sus areas de aplicacion en ingenieria, ciencia y entretenimiento
- Los modelos matematicos que sustentan las transformaciones
- Los modelos de color utilizados en entornos digitales
- La representacion de lineas y poligonos
- El procesamiento de mapas de bits como resultado final del renderizado

Las practicas desarrolladas en Blender permitieron aplicar estos fundamentos teoricos en un entorno real, demostrando que cada modelo digital es el resultado de operaciones matematicas precisas.

La graficacion por computadora no es solo una herramienta visual, sino una disciplina que combina matematica, programacion y diseño para representar el mundo digital de manera estructurada y eficiente.

## Bibliografia

Foley, J. D., van Dam, A., Feiner, S. K., & Hughes, J. F. (1996). *Computer Graphics: Principles and Practice* (2nd ed.). Addison-Wesley.

Hughes, J. F., van Dam, A., McGuire, M., Sklar, D., Foley, J., Feiner, S., & Akeley, K. (2014). *Computer Graphics: Principles and Practice* (3rd ed.). Addison-Wesley.

Shirley, P., Ashikhmin, M., & Marschner, S. (2009). *Fundamentals of Computer Graphics* (3rd ed.). A K Peters.

Sutherland, I. E. (1963). Sketchpad: A Man-Machine Graphical Communication System. Massachusetts Institute of Technology.
