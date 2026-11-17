## Parte 1: Investigacion: Web components

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


## Parte 2: Investigacion: frameworks, librerias y Node.js

1. Explica con un ejemplo la diferencia entre estándar del navegador, librería, framework
y entorno de ejecución.

RTA: 
- Estándar del navegador: Son herramientas y reglas incorporadas en el navegador. Ejemplo: JavaScript y alert().
- Librería: Es un conjunto de funciones que facilitan la programación. Ejemplo: React.
- Framework: Es una estructura que organiza cómo desarrollar una aplicación. Ejemplo: Angular.
- Entorno de ejecución: Es el ambiente donde se ejecuta el código. Ejemplo: Node.js.

2. Completa la tabla con una o dos frases por celda:

RTA:
| Criterio | Web Components nativos | React | Vue | Angular |
|----------|------------------------|-------|-----|---------|
| Tipo (estándar, librería o framework) | Estándar del navegador. | Librería. | Framework progresivo. | Framework. |
| Cómo se crea un componente | Usando Custom Elements y Shadow DOM. | Mediante funciones o clases. | Mediante la opción `createApp` y componentes. | Mediante clases con el decorador `@Component`. |
| Necesita instalar herramientas (npm) | No, el navegador ya los soporta. | Sí, normalmente se utiliza npm. | Sí, normalmente se utiliza npm. | Sí, utiliza npm y Angular CLI. |
| Ventajas principales | No necesita librerías externas y funciona en diferentes frameworks. | Flexible, reutilizable y tiene una gran comunidad. | Fácil de aprender, ligero y flexible. | Ofrece una estructura completa y herramientas integradas. |
| Desventajas principales | Requiere más código y puede ser complejo. | Necesita herramientas adicionales para muchas funciones. | Menor ecosistema empresarial que Angular. | Tiene una curva de aprendizaje más elevada. |

3. ¿Qué es Node.js, para qué se usa y qué relación tiene npm con React, Vue yAngular?
Si una tienda en línea usa React y Node.js, ¿qué hace cada uno?

RTA: Node.js es un entorno que permite ejecutar JavaScript fuera del navegador y crear servidores.
npm es un gestor de paquetes que permite instalar y administrar las herramientas y dependencias necesarias para trabajar con estos frameworks y librerías.
Ejemplo de una tienda en línea:
- React: Muestra los productos, imágenes y botones de compra.
- Node.js: Procesa las compras, gestiona los usuarios y conecta la base de datos.

RTA: En el caso de: "a. Un botón de chat que varias empresas pegan en sus propias páginas." elegiría Web Components nativos, porque permiten crear componentes reutilizables y compatibles con diferentes páginas web, sin depender de React, Vue o Angular.
Y en el caso de: "b. Una aplicación web grande para un banco, con muchos equipos de desarrollo." elegiría Angular, porque ofrece una estructura organizada, herramientas integradas y facilita el trabajo en proyectos grandes con varios equipos de desarrollo.


## Fuentes de consulta

1. **MDN Web Docs – Web Components**
   - Enlace: https://developer.mozilla.org/es/docs/Web/API/Web_components
   - Fecha de consulta: 17 de noviembre de 2026.

2. **React – Documentación oficial**
   - Título: React: La biblioteca para interfaces de usuario.
   - Enlace: https://react.dev/
   - Fecha de consulta: 17 de noviembre de 2026.

3. **Vue.js – Documentación oficial**
   - Título: Introduction.
   - Enlace: https://vuejs.org/guide/introduction.html
   - Fecha de consulta: 17 de noviembre de 2026.

4. **Angular – Documentación oficial**
   - Título: What is Angular?
   - Enlace: https://angular.dev/overview
   - Fecha de consulta: 17 de noviembre de 2026.

5. **Node.js – Documentación oficial**
   - Título: Node.js Documentation.
   - Enlace: https://nodejs.org/docs/latest/api/
   - Fecha de consulta: 17 de noviembre de 2026.

6. **npm – Documentación oficial**
   - Título: About npm.
   - Enlace: https://docs.npmjs.com/about-npm
   - Fecha de consulta: 17 de noviembre de 2026.
