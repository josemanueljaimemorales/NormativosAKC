# AKC Repositorio de Normativos — Firebase

Esta versión usa Firebase Firestore como base central para que los cambios se compartan entre celulares, tablets y computadoras.

## Firebase
- Proyecto: `akc-con-reporte`
- Colección: `normativosAKC`
- Documento principal: `estado`

La primera vez, si el documento no existe, la aplicación carga `database.json` y lo publica en Firestore.

## Importante
El generador de Excel está temporalmente desactivado en esta versión para evitar volver a producir archivos dañados. El Excel original se conserva como plantilla. Primero se valida la sincronización central; después se integra un generador seguro.

## Publicación
Subir a GitHub Pages los archivos del ZIP. `database.json` y `NORMATIVOS_AKC.xlsx` deben permanecer junto a `index.html`.

## Firestore
Las reglas del proyecto Firebase deben permitir lectura y escritura de la colección `normativosAKC` para los usuarios que vayan a operar el repositorio. Si las reglas actuales no lo permiten, hay que ajustarlas en Firebase Console.
