[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/oDY7CZkD)

# 💻 Laboratorio 2: Mi Currículum Web

## Objetivo

Basándose en el Laboratorio 1, el presente laboratorio tiene como objetivo profundizar en el desarrollo web usando CSS, a través de la creación de una página web con el currículum vitae del estudiante.

---

## 📁 Estructura del proyecto

El proyecto debe contener al menos los siguientes archivos:
```
/laboratorio-2/
  ├── index.html
  ├── styles.css
  └── README.md
```

---

## Instrucciones

### 1. Estructura básica (index.html)

Crear una página HTML que contenga:

- Un **título principal** con tu nombre completo (`<h1>`)
- Una **foto** tuya (opcional) usando la etiqueta `<img>`
- Una **descripción breve o perfil profesional** (`<p>`)
- Una **lista de habilidades** usando `<ul>` y `<li>`
- Sección de **educación** y **experiencia laboral**
- Enlaces a tus **redes sociales o correo electrónico** usando `<a href="...">`

### 2. Estilos con CSS (styles.css)

Crear un archivo `styles.css` y usa **clases (`class`)** para aplicar estilos como:

- Color de fondo
- Color del texto
- Tamaño y tipo de letra
- Bordes o separación entre secciones
- Alineación del texto
- Estilos para la imagen
- Organizar las secciones:
   - **Habilidades**
   - **Educación**
   Usando **Flexbox** para mostrarlas una al lado de la otra en pantallas grandes, y en columna en pantallas pequeñas.
- Aplicar al menos los siguientes estilos:
   - `display: flex`
   - `justify-content`
   - `align-items`
   - `flex-direction: row` y `column`
- Usar `class` para aplicar los estilos desde un archivo CSS externo (`styles.css`).

### 3. Conecta el CSS con tu HTML

En tu archivo `index.html`, dentro de la etiqueta `<head>`, enlaza el archivo de estilos:

```html
<link rel="stylesheet" href="styles.css">
```

## 💡 Sugerencia de estructura HTML

```html
<div class="secciones">
  <div class="habilidades">
    <h2>Habilidades</h2>
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>Trabajo en equipo</li>
    </ul>
  </div>

  <div class="educacion">
    <h2>Educación</h2>
    <p>Licenciatura en Ingeniería Informática - PUCE</p>
  </div>
</div>
```

## 💡 Sugerencia de CSS con Flexbox

```css
.secciones {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  gap: 20px;
}

.habilidades, .educacion {
  flex: 1;
  padding: 15px;
  border: 1px solid #ccc;
  border-radius: 8px;
  background-color: #f9f9f9;
}

@media (max-width: 768px) {
  .secciones {
    flex-direction: column;
  }
}
```

## Entrega del laboratorio

### 1. Clonar el repositorio (desde GitHub Classroom)

```bash
git clone <URL-del-repositorio>
cd <nombre-del-repositorio>
```

### 2. Configurar token de acceso (solo si es la primera vez)
- Dirigirse a: https://github.com/settings/tokens
- Generar un token clásico con permisos para repositorios.
- Guardar el token en un sitio seguro, ya que se lo necesitará para autenticarse al hacer push.

### 3. ✅ Hacer commit y push de tus cambios
```bash
git add .
git commit -m "Laboratorio 2 terminado"
git push origin main
```
