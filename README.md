# 🚀 NAVE D-6

Versión digital/web del juego de dados **Deep Space D-6**, jugable directamente desde el navegador en móvil o escritorio.

> _Eres el capitán del USS Crypsis — una nave estelar de clase RPTR llevando a cabo una patrulla rutinaria en el sistema Auborne cuando recibe una llamada de socorro. Tras el salto estelar, te das cuenta de que ¡es una trampa! Con la ayuda de tu tripulación, deberás sobrevivir hasta que llegue una flota de rescate._

---

## 🎮 Cómo jugar

1. Abre el archivo `nave-d6.html` en cualquier navegador moderno (o usa el enlace de descarga/visualización de la release).
2. Elige la **dificultad** en la pantalla inicial.
3. Pulsa **Asignar tripulación** para lanzar los 6 dados.
4. Toca un dado y luego un puesto para apilarlo.
5. Cuando termines, pulsa **Descubrir amenaza y continuar**.
6. Repite hasta que llegue la flota de rescate.

---

## ⚙️ Dificultades

Antes de empezar puedes elegir entre 5 niveles. Las opciones más difíciles quitan más cartas de "No pasa nada" del mazo y, opcionalmente, cartas de amenaza, para partidas más cortas y arriesgadas.

| Dificultad | Cartas "No pasa nada" quitadas | Cartas de amenaza quitadas | Total quitado |
|------------|-------------------------------|---------------------------|---------------|
| 🟢 **FÁCIL**   | 1 | 0 | −1 |
| 🟡 **MEDIO**   | 3 | 0 | −3 |
| 🔴 **DIFÍCIL** | 6 | 0 | −6 |
| 🟣 **CORTO**   | 6 | 1 | −7 |
| 🔵 **RÁPIDO**  | 6 | 3 | −9 |

---

## 🧑‍🚀 Tripulación y puestos

Los dados de tripulación representan a la de la nave. Las caras son las acciones disponibles.

- **◆ Comandante** — Cambia la cara de un dado disponible a la que elijas, o vuelve a tirar todos los dados disponibles. Si apilas varios, puedes cambiar varias caras de una vez.
- **▲ Táctico** — Dispara a una amenaza externa (1 de daño por táctico, +2 por cada táctico extra apilado).
- **✚ Médico** — Libera la enfermería, o retira un dado del escáner.
- **● Científico** — Recarga el escudo al máximo, o lanza el rayo de éxtasis (bloquea la próxima activación).
- **⚙ Ingeniero** — Repara el casco (+1 por ingeniero, +2 por cada ingeniero extra apilado).

---

## 👾 Amenazas

Hay dos tipos:

- **Externas**: causan daño al casco. Cuando su valor llega a 0, se destruyen.
- **Internas**: generan efectos adversos sobre la nave o la tripulación.

### Cartas internas destacadas

- **Fuego amigo** — Todos los dados con cara de TÁCTICO van directamente a la enfermería. Luego se descarta.
- **Distracción** — Bloquea un dado de tripulación hasta la siguiente reunión (queda en `used` con candado 🔒).
- **Pandemia / Invasores / Levantamiento robot** — Envían un dado a la enfermería.
- **Vientos solares** — 5 de daño al casco, y se descarta tras activarse.

---

## 🏆 Condición de victoria

**Ganas cuando el mazo se queda sin cartas para robar.** En ese momento, la flota de rescate ha llegado y la misión se da por cumplida.

Si lo que se vacía son las amenazas externas pero todavía quedan cartas en el mazo, **no ganas**: el juego continúa hasta agotar el mazo.

---

## 💡 Características de esta versión

- ✅ **100 % en el navegador**: un solo archivo HTML, sin dependencias, sin servidor.
- 🎨 **Modo claro y oscuro**: pulsa el botón 🌙 / ☀️ junto al título para alternar. Se guarda tu preferencia.
- 🎚️ **Selector de dificultad** con 5 niveles.
- 🎲 **Dados coloreados por tripulante**: cada cara de crew tiene su color (azul Comandante, rojo Táctico, etc.).
- 🏥 **Enfermería visible**: los dados incapacitados se muestran en su propia zona.
- ⚡ **Re-lanzado automático**: los dados no usados se re-lanzan al final de cada ronda (con animación).
- 📱 **Responsive**: optimizado para móvil y tablet, también funciona en escritorio.

---

## 📁 Estructura del proyecto

```
.
├── nave-d6.html          # Juego completo (un solo archivo)
├── README.md              # Este archivo
└── LICENSE                # Licencia
```

Todo el código (HTML, CSS, JS, SVG) está embebido en el HTML para máxima portabilidad. Solo necesitas abrir el archivo en un navegador.

---

## 🛠️ Cómo se compila / ejecuta

Nada. Es un archivo HTML estático. Ábrelo con:

```bash
# Linux / macOS
xdg-open nave-d6.html   # o: open nave-d6.html

# Windows
start nave-d6.html
```

O simplemente arrástralo a una ventana del navegador.

---

## 📜 Créditos

- **Diseño original**: _Deep Space D-6_ de Tony Go.
- **Traducción al español**: JL "Bicho" San Miguel.
- **Implementación web**: este repositorio.

> Deep Space D-6 es un juego solitario de dados sobre la supervivencia en el espacio profundo desconocido. Cada turno tirarás los dados de tu tripulación y los asignarás a un puesto o misión. Tendrás que lidiar con amenazas externas e internas. **Ganas sobreviviendo.**
