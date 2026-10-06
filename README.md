### 2. `app2_cinebutaca/README.md`

```markdown
# App 2: CineButaca - Reserva de Asientos con Selector

Aplicación interactiva para la reserva de asientos de cine, enfocada en la optimización de reconstrucciones del árbol de widgets mediante el uso de `Selector`. Desarrollada para la Práctica N.º 3 de INF 662.

## 🚀 Características
- **Matriz de asientos:** Muestra una sala de cine (6x8) utilizando `GridView.builder` y un `enum EstadoAsiento` (libre, seleccionado, ocupado).
- **Optimización con Selector:** Cada asiento está envuelto en un `Selector<SalaModel, EstadoAsiento>` para reconstruir únicamente la celda cuyo estado cambia al interactuar.
- **Límite y validaciones:** Valida un límite máximo de 6 asientos por reserva. Si el usuario intenta superar el máximo, se despliega un `SnackBar` informativo.
- **Barra inferior eficiente:** Utiliza `Selector` con el parámetro `child` para reutilizar widgets estáticos y calcular el total a pagar en tiempo real.
- **Pantalla de confirmación:** Muestra el resumen de la compra. Al confirmar, los asientos pasan a estado ocupado y la selección se limpia automáticamente.

## 🛠️ Tecnologías y Paquetes
- **Flutter** (Canal estable)
- **Dart 3**
- **provider: ^6.x**