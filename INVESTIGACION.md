PARTE 1: INVESTIGACION: WEB COMPONENTS

1. ¿Que problema resuelven los Web Components y que aporta cada tecnologia: Custom
Elements, Shadow DOM y HTMLTemplates?

RTA: Los Web Components resuelven el problema de crear elementos web reutilizables, independientes y faciles de mantener, evitando repetir codigo y conflictos entre estilos.
Sus tres tecnologias principales son:
- Custom Elements: permiten crear etiquetas HTML personalizadas.
- Shadow DOM: encapsula el HTML y CSS para evitar conflictos con otros elementos.
- HTML Templates: permiten crear estructuras HTML reutilizables.
En conjunto, facilitan la creacion de componentes modulares sin depender de frameworks externos.

2. ¿En que se diferencia un <template> de un <div> oculto con display: none ?
Piensa en que se muestra, que se ejecuta y que encuentra document.querySelector.

RTA: Se diferencian debido a que:
- <template>: Su contenido no se muestra, no se ejecuta y querySelector no encuentra directamente sus elementos internos. Hay que clonarlo para utilizarlo.
- <div style="display: none">: Su contenido esta oculto, pero existe en el DOM, puede ejecutarse y querySelector si encuentra sus elementos.

3. ¿Que cambia entre el Shadow DOM en modo "open" y en modo "closed"?

RTA: "Open" permite acceder al Shadow DOM mediante JavaScript usando element.shadowRoot mientras que "closed" no permite acceder mediante element.shadowRoot, ya que devuelve null.

4. ¿Que es un <slot> y para que sirve en un componente reutilizable?

RTA: Un "<slot>" es un espacio reservado dentro de un componente reutilizable donde se puede insertar contenido personalizado desde fuera. Sirve para hacer que un componente sea flexible y permita mostrar diferentes contenidos sin modificar su estructura interna.

5. ¿Que navegadores soportan hoy los Web Components? Indica la fuente y la fecha de
consulta.

RTA: Los Web Components son compatibles con los navegadores modernos:
- Google Chrome
- Mozilla Firefox
- Microsoft Edge
- Safari
- Opera
Internet Explorer no ofrece soporte nativo completo.
Fuente: MDN Web Docs – Web Components  y HTML Standard – W3C .
Fecha de consulta: 17 de noviembre de 2026.