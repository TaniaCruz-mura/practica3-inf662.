### 3. `app3_habitodiario/README.md`

```markdown
# App 3: Hábito Diario - Seguimiento de Hábitos con MultiProvider

Aplicación de seguimiento y control de hábitos diarios que demuestra la coordinación de múltiples estados independientes mediante `MultiProvider`. Desarrollada para la Práctica N.º 3 de INF 662.

## 🚀 Características
- **Gestión con MultiProvider:** Coordina de forma independiente `HabitosModel` (lista de hábitos y porcentaje) y `PreferenciasModel` (datos del usuario, modo de tema y meta diaria).
- **Tema global dinámico:** La propiedad `themeMode` de `MaterialApp` es controlada reactivamente por `PreferenciasModel` desde cualquier pantalla sin reiniciar la app.
- **Formulario validado:** Formulario para agregar hábitos (`Form` + `TextFormField` + `DropdownButtonFormField`) que asegura que el nombre no esté vacío y exige la selección de categoría.
- **Pantalla principal:** Muestra un saludo personalizado, lista interactiva de hábitos con `CheckboxListTile`, barra de progreso del día y un aviso especial al alcanzar la meta diaria.
- **Ajustes en tiempo real:** Modificación de nombre, conmutador de modo claro/oscuro y actualización de meta diaria reflejados al instante en toda la interfaz.

## 🛠️️ Tecnologías y Paquetes
- **Flutter** (Canal estable)
- **Dart 3**
- **provider: ^6.x**