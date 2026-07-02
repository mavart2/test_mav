# Ejercicio: Colaboración con GitHub mediante Pull Requests

## Objetivo

Practicar un flujo de trabajo colaborativo utilizando Git y GitHub, donde cada integrante desarrolla cambios en una rama independiente y posteriormente solicita su integración mediante un **Pull Request**.

## Flujo de trabajo

### 1. Clonar el repositorio

```bash
git clone https://github.com/mavart2/prueba_mav.git
cd prueba_mav
```

### 2. Crear una nueva rama

Cada colaborador debe crear una rama con su nombre o con el nombre de la funcionalidad.

```bash
git checkout -b nombre-rama
```

Ejemplo:

```bash
git checkout -b indice-v1
```

### 3. Realizar cambios

Modificar los archivos asignados.

### 4. Agregar los cambios

```bash
git add .
```

### 5. Crear un commit

```bash
git commit -m "Agregar mi versión del índice"
```

### 6. Subir la rama a GitHub

```bash
git push -u origin nombre-rama
```

Ejemplo:

```bash
git push -u origin indice-v1
```

### 7. Crear un Pull Request

Desde GitHub:

- Seleccionar **Compare & Pull Request**.
- Escribir un título y descripción.
- Hacer clic en **Create Pull Request**.

### 8. Revisión y Merge

El propietario del repositorio:

- Revisa los cambios.
- Verifica que no existan conflictos.
- Hace clic en **Merge Pull Request**.
- Confirma la fusión.

### 9. Actualizar la rama principal

Después del Merge:

```bash
git checkout main
git pull origin main
```

> Si la rama principal se llama `principal`:

```bash
git checkout principal
git pull origin principal
```

---

## Buenas prácticas

- No trabajar directamente sobre la rama principal.
- Crear una rama por cada funcionalidad o tarea.
- Escribir mensajes de commit descriptivos.
- Revisar los cambios antes de realizar el Merge.
- Eliminar la rama cuando ya fue fusionada.

---

## Tecnologías

- Git
- GitHub
- Visual Studio Code

---

## Autor

**Mauricio Vargas**
