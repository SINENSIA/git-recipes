# 📌 Git Log

El comando `git log` permite visualizar el historial de commits en un repositorio. Es una herramienta esencial para rastrear cambios, ver contribuciones y analizar la evolución del código.

## 📌 Uso básico de `git log`
```sh
git log
```
Muestra una lista de commits en orden cronológico inverso (los más recientes primero).

## 📌 Personalizar la salida de `git log`
Puedes mejorar la legibilidad con opciones adicionales:

- **Mostrar commits en una línea con hash corto:**
  ```sh
  git log --oneline
  ```
- **Mostrar el historial con gráfico de ramas:**
  ```sh
  git log --oneline --graph --all --decorate
  ```
- **Mostrar detalles del autor y fecha en cada commit:**
  ```sh
  git log --pretty=format:"%h - %an, %ar : %s"
  ```
  - `%h` → Hash corto del commit.
  - `%an` → Autor del commit.
  - `%ar` → Fecha relativa (ej. "2 days ago").
  - `%s` → Mensaje del commit.

## 📌 Filtrar commits en `git log`
Puedes buscar commits específicos con filtros:

- **Buscar commits de un autor:**
  ```sh
  git log --author="Nombre"
  ```
- **Buscar por palabra clave en los mensajes de commit:**
  ```sh
  git log --grep="Bugfix"
  ```
- **Mostrar cambios en un archivo específico:**
  ```sh
  git log -- archivo.txt
  ```
- **Mostrar commits en un rango de fechas:**
  ```sh
  git log --since="2024-01-01" --until="2024-02-01"
  ```

## 📌 Mostrar cambios en cada commit
Si quieres ver qué cambios se hicieron en cada commit, usa:

```sh
git log -p
```

Para mostrar solo un número específico de commits:
```sh
git log -p -n 3
```
(Muestra los últimos 3 commits con cambios detallados).

## 📌 Alias útiles para `git log`
Puedes crear alias para mejorar la visualización:

```sh
git config --global alias.lg "log --oneline --graph --all --decorate"
git config --global alias.hist "log --pretty=format:'%h - %s (%cr) <%an>' --graph"
```
Así, puedes ejecutar `git lg` o `git hist` para ver un historial más claro y compacto.