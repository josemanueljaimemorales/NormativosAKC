# Repositorio AKC — versión estable + Excel sincronizado

Esta versión conserva la interfaz, Firebase y la plantilla maestra Excel que ya estaban funcionando.

## Excel

El botón **Descargar Excel** ahora:
1. toma la plantilla `NORMATIVOS_AKC.xlsx` validada;
2. lee el estado actual de Firebase;
3. actualiza los estados C / EP / P / NA de los atletas que ya existen en la plantilla;
4. conserva la estructura, estilos, fórmulas, combinaciones y demás componentes del libro, modificando únicamente las celdas de estado de `NORMATIVOS`.

Los atletas nuevos todavía no se insertan estructuralmente en el Excel en esta etapa. Esa será la siguiente fase, después de validar esta sincronización básica.

## Firebase

Colección: `normativosAKC`
Documento: `estado`

La base central sigue siendo Firebase; el Excel es el archivo generado para respaldo, impresión y almacenamiento.
