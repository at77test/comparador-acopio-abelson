# Comparador Cuenta Corriente vs. Acopio — ABELSON SA

Herramienta HTML de un solo archivo (`index.html`) que compara el precio de un
artículo comprado en cuenta corriente al precio del día vs. usando saldo de
una o varias listas de acopio ya realizadas.

## Actualización automática de la lista de precios

El archivo `listaPrecios.xlsx` de este repositorio se actualiza solo, dos
veces por día (08:00 y 13:00 hora Argentina), mediante el workflow de
GitHub Actions ubicado en `.github/workflows/actualizar-lista-precios.yml`.
La herramienta (`index.html`) lee esa copia local automáticamente al abrirse.

Para forzar una actualización manual: pestaña **Actions** del repositorio →
"Actualizar lista de precios ABELSON" → **Run workflow**.

## Uso

1. Abrir la página publicada con GitHub Pages.
2. Subir una o varias listas de acopio (.xls) en el casillero correspondiente.
3. Buscar un artículo por código o por descripción.
4. La herramienta muestra el precio de cuenta corriente y el de cada acopio
   cargado, resaltando la opción más barata.
