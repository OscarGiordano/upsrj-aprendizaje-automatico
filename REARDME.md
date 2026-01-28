# Automatización del Gasto Diario de Transporte
 Problema a resolver
En el día a día, el gasto en transporte público es una actividad repetitiva que requiere
calcular manualmente cuánto dinero se gasta según el número de viajes realizados.
Además, registrar cada gasto de forma manual resulta poco práctico y propenso a errores.

El sistema de transporte utilizado tiene las siguientes reglas:
- El primer viaje tiene un costo fijo.
- El segundo viaje (trasbordo) es gratuito.
- El tercer viaje tiene un costo reducido.
- Este patrón se repite cada tres viajes.
Calcular estos costos manualmente y llevar un registro ordenado puede ser tedioso.
 Objetivo del algoritmo
Automatizar el cálculo y registro del gasto diario de transporte mediante un script en Python
que:
- Solicite únicamente el número de viajes realizados en el día.
- Calcule automáticamente el costo de cada viaje según las reglas establecidas.
- Muestre el costo individual de cada viaje.
- Calcule el gasto total del día.
- Registre cada viaje en un archivo CSV utilizando la librería pandas.
##Funcionamiento del algoritmo
1. El programa verifica si existe el archivo `gastos.csv`.
2. Si el archivo no existe, se crea con las columnas necesarias.
3. Se obtiene automáticamente la fecha actual del sistema.
4. El usuario ingresa el número de viajes que realizará en el día.
5. Para cada viaje:
   - Se calcula el costo según su posición en el ciclo de tres viajes.
   - Se muestra el costo en pantalla.
   - Se registra el viaje como un nuevo gasto en el archivo CSV.
6. Al finalizar, el programa muestra el gasto total del día en transporte.
## Reglas de cálculo del transporte
- Viaje 1 → Costo completo ($15)
- Viaje 2 → Gratis ($0)
- Viaje 3 → Un tercio del costo ($5)
- El patrón se repite cada 3 viajes

##Ejecución del programa
Desde la terminal de Visual Studio Code:

```bash
python control_gastos.py
