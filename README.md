# terminal-color

# DESAFIO GRUPAL: LA TERMINAL

## 🎯 Propósito del desafío

Este ejercicio busca que el equipo:

- Se familiarice con **npm** y dependencias.
- Aprenda a usar distintos tipos de **`console.log`**.
- Practique el flujo **colaborativo con ramas y pull rnpm install chalkequests**.
- Aplique lo aprendido en Python ahora en **JavaScript real**.

![image.png](attachment:24692ebe-7468-4a62-9409-8b5e75b32e93:image.png)

---

## 🧩 Contexto

Cada equipo creará un pequeño programa llamado **“La Terminal Parlante”** 🎙️, que mostrará mensajes coloridos en la consola usando la librería `chalk`.

El programa saludará al usuario, mostrará información divertida, advertencias, y errores simulados.

---

## 🧭 Paso a paso (guiado)

### 1️⃣ Crear el repositorio principal

El profesor o líder técnico creará el repositorio base:

```
repo: terminal-color
```

Con el siguiente contenido inicial:

```
terminal-color/
├── README.md
├── index.js
└── package.json
```

---

### 2️⃣ Clonar el repositorio

Cada integrante debe clonar el repo en su máquina local:

```bash
git clone https://github.com/<TU-USUARIO>/terminal-color.git
cd terminal-color
```

---

### 3️⃣ Inicializar npm

Dentro de la carpeta, inicialicen el proyecto:

```bash
npm init -y
```

Esto creará el archivo `package.json`.

> 💬 Si te aparece un error, revisa si estás en la carpeta correcta.
> 
> 
> Si te dio error, es porque **no estabas atentx, equipo 😜**.
> 

---

### 4️⃣ Buscar una dependencia

Vayan a 👉 https://www.npmjs.com/

Y busquen la dependencia **chalk** (sirve para darle color a la terminal).

> Tip: también pueden buscar otras dependencias visuales, pero chalk es suficiente por ahora.
> 

---

### 5️⃣ Instalar chalk

Ejecuten el siguiente comando (¡con atención! 👀):

```bash
npm instalar chalk
```

> ⚠️ Si escribiste npm instalar chalk, no funcionará.
> 
> 
> ¡El comando correcto es `npm install chalk`! 
> 

---

### 6️⃣ Crear ramas por equipo

Habrá **dos equipos**:

| Equipo | Rama | Integrantes (6–7 aprox.) |
| --- | --- | --- |
| A | `feature/equipoA` | *completa con nombres* |
| B | `feature/equipoB` | *completa con nombres* |

Cada equipo trabajará **en su rama**.

```bash
git checkout -b feature/equipoA
# o
git checkout -b feature/equipoB
```

---

### 7️⃣ Código base (`index.js`)

```jsx
// Importamos la librería chalk
import chalk from 'chalk';

// Mensajes iniciales
console.log(chalk.blue('👋 ¡Bienvenido a la Terminal Parlante!'));
console.info(chalk.green('ℹ️ Esta terminal está viva... y tiene estilo.'));
console.warn(chalk.yellow('⚠️ Atención: Esto puede ponerse colorido.'));
console.error(chalk.red('❌ Error simulado: algo salió demasiado bien.'));
console.log(chalk.magenta('💡 Recuerda: la práctica hace al programador.'));

// BONUS: función básica
function saludar(nombre) {
  console.log(chalk.cyan(`Hola ${nombre}, ¡bienvenido al mundo JavaScript! 🌍`));
}

// Prueba de función
saludar("Equipo JS");
```

<aside>
<img src="notion://custom_emoji/5f72e359-3b8d-45ab-83ad-6cb8c2bcb54d/2a14db47-a255-8096-96c5-007aa79c1e35" alt="notion://custom_emoji/5f72e359-3b8d-45ab-83ad-6cb8c2bcb54d/2a14db47-a255-8096-96c5-007aa79c1e35" width="40px" />

> 👾 Tip: si te da error “Cannot use import statement outside a module”,
> 
> 
> agrega `"type": "module"` dentro de tu `package.json`.
> 
</aside>

---

### 8️⃣ Tarea de cada equipo

### 🧱 Equipo A

Agrega una función llamada `mostrarEstado()` que muestre mensajes de:

- inicio del programa,
- proceso en ejecución,
- finalización exitosa.

Usen distintos tipos de `console`:

`console.log`, `console.info`, `console.warn`, `console.error`.

### 🧱 Equipo B

Crea una función `simularError()` que muestre:

- un mensaje de advertencia (amarillo),
- un error (rojo),
- un mensaje final de recuperación (verde).

Usen `chalk` para colorear cada tipo de mensaje.

---

### 9️⃣ Commit y push

Cada equipo debe guardar y subir su avance:

```bash
git add .
git commit -m "feat: agrega funciones de mensajes con chalk"
git push origin feature/equipoA
# o
git push origin feature/equipoB
```

---

### 🔀 1️⃣0️⃣ Pull Request y Merge

- El **líder del proyecto** revisa los Pull Requests de `feature/equipoA` y `feature/equipoB`.
- Los aprueba y hace **merge** en la rama `main`.
- Luego, todos ejecutan:

```bash
git checkout main
git pull origin main
```

> 💬 Así todos tienen la versión final unificada.
> 

---

### 🧪 1️⃣1️⃣ Prueba final

Ejecuten el programa:

```bash
node index.js
```

La terminal debería mostrar algo como:

```
👋 ¡Bienvenido a la Terminal Parlante!
ℹ️ Esta terminal está viva... y tiene estilo.
⚠️ Atención: Esto puede ponerse colorido.
❌ Error simulado: algo salió demasiado bien.
💡 Recuerda: la práctica hace al programador.
Hola Equipo JS, ¡bienvenido al mundo JavaScript! 🌍
```

---

## 🎓 Reflexión final

> ¿Qué aprendiste sobre dependencias y npm?
¿Por qué es importante separar trabajo en ramas?
¿Qué diferencia hay entre `console.log`, `console.info`, `console.warn` y `console.error`?¿Qué errores comunes encontraron en equipo?
> 

💬 **Discusión en grupo:**

Cada equipo comenta qué aprendió y qué error les hizo reír más 😅.

---

## 🏁 Resultado esperado

Un repositorio con:

- Código en JS funcional.
- Uso de `chalk` y varios `console`.
- Trabajo colaborativo con ramas y PR.
- Todos sincronizados con el `main`.