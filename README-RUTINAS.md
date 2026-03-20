# Rutinas Personalizadas con Datos Externos

## Archivos disponibles:

### RutinaJClaude
- **HTML:** `rutina-claude.html`
- **Datos:** `datos-claude.json`
- **Descripción:** Rutina original con énfasis en pecho y desarrollo balanceado

### RutinaJGemini
- **HTML:** `rutina-gemini.html`
- **Datos:** `datos-gemini.json`
- **Descripción:** Rutina mejorada con circuitos metabólicos y énfasis en glúteos

## Cómo usar:

1. Sube ambos archivos (HTML + JSON correspondiente) al mismo repositorio en GitHub
2. En GitHub Pages, asegúrate de que ambos estén públicos
3. Abre el HTML desde tu iPhone en Safari
4. El HTML automáticamente cargará el JSON con los pesos históricos

## Estructura del JSON:

```json
{
  "rutina": "Nombre",
  "descripcion": "Descripción",
  "ejercicios": {
    "d1": {
      "label": "Día 1",
      "tag": "Nombre del día",
      "ejercicios": [
        {
          "id": "e1",
          "nombre": "Nombre del ejercicio",
          "peso_default": 20,
          "historico": [20, 20, 19, 20]
        }
      ]
    }
  }
}
```

- **peso_default:** El peso que aparecerá por defecto en los campos
- **historico:** Array con los pesos utilizados en sesiones anteriores (referencia)
- **null:** Para ejercicios sin peso (calistenia, bandas, etc.)

## Ventajas:

✓ Los datos están centralizados en un archivo JSON
✓ Fácil de actualizar sin tocar el HTML
✓ Histórico de pesos para referencia
✓ Se pueden crear múltiples versiones de rutinas
✓ Compatible con GitHub Pages (gratis)

