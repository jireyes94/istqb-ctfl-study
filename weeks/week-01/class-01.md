# Semana 1, clase 1: Qué es testing, objetivos y debugging

**Estado:** En curso desde 2026-09-29; pendiente de respuestas y corrección.

**Objetivos:** FL-1.1.1 (K1), FL-1.1.2 (K2).

**Referencia:** [Syllabus oficial CTFL v4.0.1](https://istqb.org/wp-content/uploads/2024/11/ISTQB_CTFL_Syllabus_v4.0.1.pdf).

## 1. Teoría oficial

Según [CTFL v4.0.1, §1.1, pp. 15–16](https://istqb.org/wp-content/uploads/2024/11/ISTQB_CTFL_Syllabus_v4.0.1.pdf), testing evalúa productos de trabajo y calidad: puede encontrar defectos directamente mediante revisión estática o provocar fallos al ejecutar software. Objetivos típicos: evaluar requisitos, historias, diseño o código; encontrar defectos; cubrir lo requerido; reducir riesgo; verificar requisitos y obligaciones; informar decisiones; generar confianza; validar expectativas de interesados. Dependen del contexto, riesgos, nivel y ciclo de desarrollo.

Testing y debugging son actividades diferentes. Si una prueba dinámica revela un fallo, debugging lo reproduce, diagnostica el defecto causante y lo corrige. Después, testing de confirmación verifica la corrección y pruebas de regresión pueden buscar efectos secundarios. Si una revisión estática encontró el defecto directamente, corregirlo no requiere reproducir un fallo.

## 2. Explicación en castellano

Un test aporta información aunque falle. Verificación pregunta si se cumplieron requisitos especificados; validación, si el producto satisface las expectativas de los interesados. El trabajo de testing no termina en ejecutar casos: también revisa productos y comunica riesgos. Debugging describe la tarea de encontrar y quitar el defecto, no un cargo exclusivo: una persona puede hacer ambas actividades.

## 3. Ejemplo concreto

Requisito: «Para compras superiores a $50.000, aplicar 10% de descuento». Revisar el texto y detectar que no aclara el tratamiento de exactamente $50.000 es testing estático. Tras aclarar la regla, ejecutar una compra de $60.000 y observar $60.000 en lugar de $54.000 es testing dinámico que provoca un fallo. Reproducirlo, encontrar una condición invertida y corregirla es debugging. Repetir el caso es confirmación; probar descuentos relacionados puede ser regresión. Este escenario es creación propia.

## 4. Aplicación QA

Entregá una tabla con cuatro filas: revisión del requisito; ejecución de la compra de $60.000; reproducción/diagnóstico/corrección; repetición tras el cambio. Para cada una indicá la actividad (testing estático, dinámico, debugging o confirmación) y su resultado. Explicá también qué información necesitaría quien decide si publicar el carrito.

## 5. Preguntas CTFL originales

Preguntas originales, una opción por pregunta. Respondé antes de mirar la corrección.

1. **FL-1.1.1 (K1).** ¿Cuál es un objetivo típico del testing? A) Demostrar ausencia total de defectos. B) Informar decisiones de los interesados. C) Garantizar que ninguna corrección cause efectos secundarios. D) Sustituir requisitos por pruebas.
2. **FL-1.1.2 (K2).** Durante una compra aparece un total incorrecto. ¿Qué actividad constituye debugging? A) Comparar total esperado y observado. B) Informar el fallo. C) Reproducir, localizar el defecto y corregirlo. D) Repetir la prueba después de corregirlo.
3. **FL-1.1.2 (K2).** Una revisión de código detecta una condición invertida antes de ejecutar el programa. ¿Qué describe mejor lo ocurrido? A) Testing estático encontró directamente el defecto; corregirlo no exige reproducir un fallo. B) Ocurrió un fallo del programa. C) Toda revisión es debugging. D) Una prueba de regresión encontró necesariamente el defecto.
4. **FL-1.1.1 (K1).** ¿Cuál de estas metas puede variar con el contexto del proyecto? A) Evitar decisiones de publicación. B) Elegir objetivos de testing según riesgos, nivel y producto evaluado. C) Garantizar calidad absoluta con una cifra fija de casos. D) Limitar testing a código ejecutable.

## 6. Corrección razonada

Pendiente de respuestas del alumno. Explicar la correcta y cada distractor, revisar el entregable, registrar dudas y actualizar `PROGRESS.md` al cerrar.
