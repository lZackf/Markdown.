# Manual Completo de Markdown (README.md)

## Introducción
Markdown es un lenguaje de marcado ligero para formatear texto plano de forma legible que se convierte fácilmente a HTML y es ampliamente usado en GitHub, foros y editores. Este archivo reúne la sintaxis básica, extensiones comunes y ejemplos.

---

# Encabezados
# H1
## H2
### H3
#### H4
##### H5
###### H6

---

# Énfasis
Texto normal, **negrita**, *cursiva*, ***negrita y cursiva***, ~~tachado~~.

# Listas
- Elemento de lista no ordenada
- Otro elemento
  - Subelemento (anidado)
* Alternativa con asterisco

1. Primer elemento
2. Segundo elemento
   1. Subítem numerado
3. Tercer elemento

# Listas de tareas (GitHub)
- [x] Tarea completada
- [ ] Tarea pendiente

# Enlaces e imágenes
Enlace inline: [Ejemplo](1)  
Enlace referencia: [ejemplo][1]

![Texto alternativo de imagen](https://via.placeholder.com/150 "Título de la imagen")

[1]: https://example.com "Enlace de referencia"

# Citas
> Esta es una cita en bloque.
>
> Segunda línea de la cita.

# Código
Código inline: `console.log("hola")`

Bloque de código con resaltado de sintaxis:
```js
// archivo ejemplo.js
function saludar(nombre) {
  return `Hola, ${nombre}!`;
}
console.log(saludar("Mundo"));
Mostrar código sin resaltado:

Código
Línea de código simple
Tablas
Columna A	Columna B	Alineación
Centro	Izquierda	Derecha
Texto	Más texto	12345
Reglas horizontales
Referencias y notas al pie
Texto con nota al pie[^1].

[^1]: Esta es la nota al pie.

HTML inline
<p>Esto es HTML embebido dentro de Markdown.</p>

Caracteres especiales y escape
Para mostrar * o _ usa la barra invertida: \texto\

Autolinks y menciones
<https://example.com> @usuario (menciones en plataformas que lo soportan)

Emoji (GitHub)
:smile: :rocket: :tada:

Mermaid (si la plataforma lo soporta)
mermaid
graph TD
  A[Inicio] --> B{Decisión}
  B -->|Sí| C[Acción 1]
  B -->|No| D[Acción 2]
Math (LaTeX, si la plataforma lo soporta)
Inline: \(E = mc^2\)
Bloque:
\[
\int_{a}^{b} x^2 \, dx
\]

Ejemplos avanzados y trucos
Listas con código:

npm install paquete --save

Bloques de cita con código:

bash
echo "Dentro de una cita"
Tabla con HTML si Markdown no alcanza: <table><tr><td>Celda HTML</td><td>Otra</td></tr></table>

Combinar imágenes y enlaces:

Buenas prácticas
Mantén el README legible: usa secciones, ejemplos y una tabla de contenidos si es largo.

Prefiere bloques de código para comandos reproducibles.

Usa enlaces relativos para documentación dentro del repo.

Cheatsheet rápido (resumen)
Encabezados: #, ##, ###

Negrita: **texto**

Cursiva: *texto*

Código inline: `código`

Bloque de código: triple backticks ```

Lista ordenada: 1. 2.

Lista no ordenada: - *

Enlace: [texto](url)

Imagen: ![alt](url)

Tabla: | a | b | con separador |---|---|
