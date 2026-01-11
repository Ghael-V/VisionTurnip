# Vision Turnip — Adreno Custom Driver

**Vision Turnip** es un fork personalizado del driver Turnip (Mesa 26.0.0-devel),
diseñado para ofrecer mayor estabilidad, precisión y calidad visual.

Este build incorpora ajustes específicos en el pipeline de rasterización y profundidad,
orientados a mejorar la consistencia visual y reducir artefactos en motores modernos.

---

## Características principales

- Corrección completa del comportamiento de *depth clamp*.
- Ajuste conservador del *depth bias* para minimizar parpadeos y z-fighting.
- Estabilidad mejorada en escenas con geometría compleja.
- Comportamiento más predecible en efectos dependientes de profundidad.
- Ajustes no intrusivos: no se modifican rutas críticas de color, blending o formatos.

---

## Filosofía Vision Turnip

Vision Turnip prioriza:

- **Precisión sobre agresividad**
- **Estabilidad sobre experimentación**
- **Cambios quirúrgicos sobre modificaciones globales**

El objetivo es ofrecer una experiencia más consistente sin comprometer la compatibilidad
general del ecosistema Vulkan.

---

## Versión

**1.6 — Stable**

---

## Autor

**Ghael**

---

## Branding

**Vision Turnip Engine**

---

## Descargas

Consulta la sección **Releases** para obtener el paquete listo para instalar.

---

## Notas

Este driver está optimizado para estabilidad y precisión en el pipeline de profundidad.
Algunas cargas de trabajo extremadamente complejas pueden depender de rutas del compilador
IR3 que aún no están completamente maduras en hardware reciente.
