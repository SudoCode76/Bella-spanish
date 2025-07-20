# Introducción a NPM: Una carta a mi padre

Padre,

Una vez me preguntaste qué es NPM. Por favor, imagínalo como un "bibliotecario" mágico en nuestro estudio.

Durante la construcción de nuestro estudio (proyecto), necesitamos usar muchas "piezas" o "herramientas" predefinidas (como el `express` que mencionamos antes). Estas piezas y libros de herramientas están dispersos en una enorme "biblioteca central" por todo el mundo. Esta biblioteca se llama **NPM (Administrador de Paquetes de Nodos)**.

Y este "bibliotecario" en nuestro estudio es la encarnación de la herramienta NPM en nuestro ordenador. Puede ayudarnos a hacer varias cosas muy importantes:

---

### 1. `package.json`: Nuestra "Lista de Libros"

Cada proyecto tiene un archivo llamado `package.json`. Puedes pensar en él como la "lista de libros" en manos de este bibliotecario.

Esta lista registra en detalle:

* **Información básica del estudio**: como su nombre (`name`), número de versión (`version`), descripción (`description`), etc.
* **"Libros de referencia" obligatorios** (`dependencies`): Estos son los libros necesarios para que nuestro estudio siga funcionando. Por ejemplo, necesitamos el libro `express` para crear un servicio web.
* **"Libros de referencia" solo para la creación** (`devDependencies`): Estos libros solo se utilizan al crear y personalizar el estudio, y no son necesarios después de recibir visitas. Por ejemplo, `nodemon` puede ayudarnos a actualizar automáticamente el estudio para que podamos comprobar los efectos de las modificaciones en cualquier momento.
* **"Comandos de acceso directo"** (`scripts`): Podemos predefinir algunos comandos sencillos para que los administradores puedan realizar tareas complejas. Por ejemplo, el comando `npm start` que configuramos le indica al administrador que inicie el estudio.

### 2. `npm install`: pedir prestados libros de la biblioteca

Cuando recibimos un nuevo proyecto (o queremos añadir nuevos libros de referencia a un proyecto existente), solo tenemos que decirle al administrador en la puerta del estudio:

```bash
npm install
```

Inmediatamente leerá la lista en `package.json`, luego irá a la biblioteca central, pedirá prestados todos los libros (paquetes de dependencia) de la lista y los colocará ordenadamente en una estantería llamada `node_modules`.

Si queremos pedir prestado un libro nuevo, como un libro de referencia práctico llamado `lodash`, podemos indicarle así:

```bash
npm install lodash
```

No solo pedirá prestado el libro, sino que también, muy consideradamente, añadirá automáticamente el registro de `lodash` a la lista de "libros de referencia" en `package.json`.

### 3. `npm run`: Ejecutar comandos de acceso directo

Para ejecutar los comandos de acceso directo predefinidos en `scripts` en `package.json`, solo tenemos que ejecutar:

```bash
npm run <nombre del comando>
```

Por ejemplo, para iniciar nuestro servidor de desarrollo, ejecutamos:

```bash
npm run dev
```

El administrador seguirá inmediatamente las instrucciones de la lista para realizar las operaciones correspondientes.

(Una excepción es `start`, que es el comando más común, por lo que podemos omitir `run` y ejecutar directamente `npm start`).

---

En resumen, NPM es nuestro leal y eficiente bibliotecario. Nos permite usar cómodamente la sabiduría aportada por desarrolladores de todo el mundo y mantiene nuestro estudio bien organizado.

Espero que esta explicación les ayude a comprenderlo claramente. En futuras creaciones, confiaremos cada vez más en este excelente compañero.

Te quiero, Bella