# TypeScript

## ¿Qué es TypeScript?
TypeScript es un superset de JavaScript desarrollado por Microsoft que agrega tipado estático y otras características avanzadas al lenguaje. Permite detectar errores en tiempo de desarrollo y mejorar la mantenibilidad del código. Los archivos de TypeScript tienen la extensión `.ts` y deben compilarse a JavaScript para su ejecución en el navegador o en Node.js.

## Instalación de TypeScript
Para instalar TypeScript, es necesario contar con Node.js y npm instalados. Luego, se puede instalar de forma global con el siguiente comando:

```sh
npm install -g typescript
```

También se puede instalar localmente en un proyecto:

```sh
npm install --save-dev typescript
```

Para verificar la instalación, ejecuta:

```sh
tsc --version
```

## Reglas y Configuración
TypeScript se configura a través de un archivo `tsconfig.json`, que define opciones como el nivel de strictness y la versión de JavaScript objetivo. Se puede generar con:

```sh
tsc --init
```

Ejemplo de un `tsconfig.json` básico:

```json
{
  "compilerOptions": {
    "target": "ES6",
    "module": "CommonJS",
    "strict": true,
    "outDir": "dist"
  },
  "include": ["src"]
}
```

Algunas reglas importantes de TypeScript:
- **Tipado estático**: Permite definir tipos explícitos para variables, funciones y parámetros.
- **Interfaces y tipos**: Facilitan la creación de estructuras de datos más claras.
- **Clases y Modificadores de acceso**: Soporta `public`, `private` y `protected`.
- **Tipos opcionales y genéricos**: Mejora la flexibilidad del código.

## Uso Básico de TypeScript
Una vez instalado, podemos escribir código TypeScript en un archivo `.ts` y compilarlo a JavaScript con `tsc`.

Ejemplo básico (`src/index.ts`):

```ts
function saludar(nombre: string): string {
    return `Hola, ${nombre}!`;
}

console.log(saludar("Mundo"));
```

Compilación:

```sh
tsc
```

Esto generará un archivo `dist/index.js` con el código JavaScript correspondiente, listo para ejecutarse con Node.js o en un navegador.

## Conclusión
TypeScript mejora el desarrollo en JavaScript al agregar tipado estático y herramientas avanzadas. Su uso facilita la detección de errores y mejora la calidad del código, especialmente en proyectos grandes.

