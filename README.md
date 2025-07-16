# 🌲 Sistema de Alerta de Incendios (S.A.I.)

Este proyecto es una landing page informativa con formulario de suscripción que permite solicitar la instalación de un nodo del Sistema S.A.I. (detección temprana de incendios mediante IA).

## ⚙️ Requisitos

- Python 3.x (ya instalado en la mayoría de sistemas)
- Navegador web (Chrome, Firefox, etc.)

## 🚀 Instrucciones para deployar localmente

1. Clonar o descargar este repositorio en tu máquina.
2. Abrí una terminal o consola dentro de la carpeta donde se encuentra `index.html`.
3. Ejecutá el siguiente comando:

```bash
python3 -m http.server 8080
```

El formulario de contacto se encuentra al final de la página y envía los datos vía POST al siguiente endpoint:

```html
<input type="text" name="localidad" required>
<input type="text" name="departamento" required>
<select name="provincia" required>
  <option value="Córdoba" selected>Córdoba</option>
</select>
<input type="text" name="nombre" required>
<input type="text" name="apellido" required>
<input type="tel" name="telefono" required>
<input type="email" name="email" required>
<textarea name="ubicacion_nodo" required></textarea>
<input type="radio" name="internet" value="si|no|limitado" required>
<input type="radio" name="electricidad" value="si|no|intermitente" required>
<input type="radio" name="red" value="si-publico|si-privado|no" required>
<select name="como_se_enteron" required>
  <option value="redes-sociales">Redes sociales</option>
</select>
<textarea name="comentarios"></textarea>
```