# ejercicio_24_abril

import json

datos_a_guardar = {
    "usuario": "Esther",
    "puntuacion": 95,
    "nivel": 3
}

with open("datos.json", "w") as file:
    json.dump(datos_a_guardar, file, indent=4)

print("Datos guardados correctamente en datos.json\n")

with open("datos.json", "r") as file:
    datos_leidos = json.load(file)

print("Datos leídos del archivo:")
print(datos_leidos)

