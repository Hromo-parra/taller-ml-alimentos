# Fruta + datos: taller de Machine Learning

Taller interactivo de Ingeniería en Alimentos, de primero a octavo semestre. Versión GUIADO v9, 14 de octubre de 2026. Material didáctico: Héctor Romo-Parra / NeuroPsicoLocos.

Abra `index.html` en Safari o Chrome, o visite la página de GitHub Pages de este repositorio. El HTML incluye estilos, datos y código: no requiere cuenta, Python, instalación ni servicios externos. Tras descargarlo puede usarse sin conexión.

El recorrido incluye dos introducciones a ML y siete actividades: predicción humana, tabla de datos, entrenamiento de un árbol, prueba reservada, explicación con Shapley, fuga de información y conclusión. Cada sección incluye instrucciones; las actividades ofrecen retos opcionales para profundizar.

Todos los frutos, medidas y etiquetas son sintéticos. El ejercicio no evalúa madurez, calidad, seguridad alimentaria ni aptitud de consumo reales. Shapley explica la salida del modelo frente a una referencia; no demuestra causalidad. No se garantiza exactitud con otros datos.

Las elecciones y notas permanecen en memoria de la pestaña y se pierden al cerrar o recargar. El código no utiliza APIs de red, cuentas, analítica ni almacenamiento persistente. GitHub Pages sirve el archivo y puede procesar datos técnicos de las visitas según sus propias políticas.

## Licencias

El contenido didáctico original (textos explicativos, actividades y representaciones educativas) se publica bajo **Creative Commons Attribution 4.0 International (CC BY 4.0)**. Crédito: **Héctor Romo-Parra / NeuroPsicoLocos, Fruta + datos, GUIADO v9, 2026**. Al reutilizar contenido, enlace la licencia e indique los cambios. Véase `LICENSE-CONTENIDO.md`.

La licencia CC BY 4.0 **no se aplica al código de software**, incluidos JavaScript y CSS incrustados en `index.html`. No se encontró una licencia de software preexistente en el paquete original; su licencia de reutilización queda pendiente. El código se publica autorizado para consultar el funcionamiento del taller, sin otorgar una nueva licencia de software. No se añade MIT ni otra licencia por inferencia. Se mantienen los avisos existentes. No hay bibliotecas o recursos externos incorporados.

## Comprobaciones

Antes de publicar v9 se aprobaron 17 pruebas numéricas independientes, 13 comprobaciones estáticas, 21 pedagógicas/eventos y navegación con DOM mínimo. Se comprobó que una selección pendiente no se confirma, el camino del fruto corresponde al árbol activo, la prueba se calcula una vez y explorar otros árboles/SHAP conserva la identidad y el snapshot del árbol evaluado y su resultado. No se recalculan métricas de prueba reservada en la exploración. Motor, datos, semilla, split y Shapley se conservan.

La revisión visual y funcional real de v9 en navegador sigue pendiente. Las pruebas estáticas y de eventos con DOM mínimo no equivalen a comprobar diseño, proyector, móviles, accesibilidad o interacción real. Las cifras del ejercicio son resultados sintéticos, no mediciones alimentarias reales.

## Cambios de v6

La comparación sencilla siempre responde la categoría más frecuente de entrenamiento y muestra sus recuentos. El selector «Hasta 1/2/3 preguntas» distingue la selección pendiente del árbol activo. El árbol completo muestra el camino calculado de L01-F1 con sus medidas y la etiqueta conocida separada. Antes de confirmar se muestran el árbol entrenado y su práctica.

Tras la prueba, el modo de aprendizaje permite entrenar y explicar otro árbol aparte usando entrenamiento y práctica; no reemplaza el árbol evaluado ni presenta nuevas pruebas reservadas. El encabezado identifica el modo y permite volver al árbol evaluado. SHAP muestra profundidad, medidas usadas, referencia, ceros exactos frente a redondeo, intervalo de decisión y un ejemplo compatible de firmeza. Los controles consultan otro fruto, no reentrenan. Recargar o reiniciar repite los mismos datos y no crea una prueba independiente.

Los informes internos y conversaciones no forman parte del repositorio público.

## Corrección visual v7

Las tarjetas y nodos claros declaran texto oscuro explícito, también dentro del panel oscuro de confirmación. El ejemplo L01-F1 muestra medidas, etiqueta separada, decisiones Sí/No y respuesta en un recorrido vertical calculado. El árbol completo conserva todas sus ramas en una vista complementaria desplegable y apilada, con estructura responsive. No se cambia el estado del modelo, snapshot, dataset, motor ni SHAP.

Las comprobaciones nominales de color superan 4.5:1 para los fondos claros usados por los componentes corregidos y el panel oscuro. Son cálculos a partir de CSS, sin medición de estilos computados u overflow. V7 aún requiere comprobación visual y funcional real en navegador; no se presenta una captura renderizada propia como evidencia.

## Comparación y elección v8

El paso 6 separa «Compara tus modelos» de «Comprueba tu elección». Solo opciones entrenadas en esta sesión tienen métricas de entrenamiento/práctica capturadas y un modelo exacto guardado. Elegir una tarjeta recupera ese objeto sin reentrenar. Se recomienda elegir con práctica y, si empatan, menos preguntas. Confirmar evalúa una sola elección con los frutos reservados y conserva el modelo y resultado inmutables; no muestra pruebas por opción. Exploración y Shapley siguen separados del modelo evaluado. El cierre celebra entrenar y comprobar un modelo, con límite explícito de frutos simulados.

Pasaron 21 regresiones pedagógicas/eventos, incluidas opciones no entrenadas, guardado/recuperación de modelos exactos, consentimiento invalidado al cambiar elección, confirmación única y snapshot intacto durante exploración. Motor numérico y datos intactos. QA visual real de v8 sigue pendiente: el navegador interno no estaba disponible y no se controló Safari. Las reglas responsive y contrastes se verificaron en fuentes; no se midió overflow en navegador.

## Presentación de autor v9

Dr. Héctor Manuel Romo Parra. Profesor investigador e investigador principal (PI). Instituto Nacional de Neurología y Neurocirugía Manuel Velasco Suárez. [Ver currículum](https://hromo-parra.github.io/academic-cv/).

Declaración aprobada por el autor: «Declaro no tener conflictos de interés relacionados con este taller».

La presentación no cambia la lógica: app.js y core.js son idénticos a v8. El enlace al currículum abre otra pestaña y requiere conexión. Se conservan URL, QR y licencia existentes; no se migra a otro sitio. QA Safari real sigue pendiente porque la herramienta de control no estuvo disponible en este executor pese a autorización. El PDF docente actualizado se entrega de forma privada en Library y no forma parte del repositorio público.
