# WEBSKILL 21

LAMIAE CABECERA FOOTER Y MODALES

ROCIO PAGINA QUIENES SOMOS

PABLO PAGINA DE REPTILES

KAWTAR PAGINA PRINCIPAL

## Cómo hacer merge de las ramas con main

### Ramas del proyecto

- `PáginaPrincipal` — Página principal (Kawtar)
- `quienes-somos` — Página Quiénes Somos (Rocío)
- `reptiles` — Página de Reptiles (Pablo)

### Pasos para hacer merge

1. **Situarse en la rama main:**
   ```bash
   git checkout main
   ```

2. **Hacer merge de la rama deseada:**
   ```bash
   git merge PáginaPrincipal
   git merge quienes-somos
   git merge reptiles
   ```

3. **Si hay conflictos**, se pueden resolver de varias formas:
   - **Desde VS Code:** Abrir la ventana de combinados (Merge Editor) que aparece automáticamente al detectar conflictos. Permite aceptar los cambios entrantes, los actuales o ambos de forma visual.
   - **Desde la consola:**
   - Mantener la versión de la rama entrante por terminal:
     ```bash
     git checkout --theirs <archivo>
     ```
   - Mantener la versión de main por terminal:
     ```bash
     git checkout --ours <archivo>
     ```

4. **Añadir los archivos resueltos y hacer commit:**
   ```bash
   git add .
   git commit -m "Merge <nombre-rama> into main"
   ```

5. **Subir los cambios al remoto:**
   ```bash
   git push origin main
   ```

### Orden recomendado de merge

1. `PáginaPrincipal` → main
2. `quienes-somos` → main
3. `reptiles` → main
