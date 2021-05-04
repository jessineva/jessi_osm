# osm_tarea
Crea una funcion para el manejo de un archivo OSM



El archivo "materiales.osm" proviene de OpenStudio, es un archivo de texto plano y es utilizado para realizar simulaciones numéricas de edificaciones. La geometría de la edificación, equipo, personas, materiales y sistemas constructivos se encuentran definidos en lo que le llaman Objetos. Existen varios objetos de materiales donde se enlista un hash, nombre del material, espesor y sus propiedades térmicas.

Un objeto de un material se ve así:

```
OS:Material,
  {7311a74e-33cf-47e9-a28c-a9a6c74f4083}, !- Handle
  MAT-CC05 4 HW CONCRETE,                 !- Name
  Rough,                                  !- Roughness
  0.1016,                                 !- Thickness {m}
  1.311,                                  !- Conductivity {W/m-K}
  2240,                                   !- Density {kg/m3}
  836.800000000001,                       !- Specific Heat {J/kg-K}
  0.9,                                    !- Thermal Absorptance
  0.85,                                   !- Solar Absorptance
  0.85;                                   !- Visible Absorptance
```

Cualquier objeto de material siempre empieza con "OS:Material,"
y termina con ";"

Algunos objetos contienen 11 renglones, otros menos.

Escribe un programa que:

* Lea cualquier archivo OSM y separe todos los objetos "OS:Material," contenidos en ese archivo OSM sin perder la estructura ni el orden de cada objeto y agrupe esos objetos y los guarde en un archivo al que le puedas especificar el nombre. Ejemplo:
```
separa("materiales.osm","resultado.osm")  
```
donde materiales.osm es el archivo original y resultado.osm contiene los objetos de materiales.
* El programa debe estar documentado y contenido en una función.
* Se debe entregar en un repositorio de GitHub con el siguiente nombre del repo: "nombre_osm" donde nombre es tu nombre de pila, ya no debe haber ningún "push" después de la fecha de entrega, entregas una liga y el repo debe ser público.
* Tenga la estructura adecuada en folders.


