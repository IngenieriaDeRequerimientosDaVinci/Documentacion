Este es un ejemplo de casos de uso en plantuml:

[plantuml](http://www.plantuml.com/plantuml/uml/SyfFKj2rKt3CoKnELR1Io4ZDoSa70000)

```
@startuml
left to right direction
skinparam packageStyle rectangle
actor "Usuario de HubSpot" as User
rectangle "Menú Ventas - Submenú Negocios" {
  User --> (Crear un negocio)
  User --> (Editar un negocio)
  User --> (Eliminar un negocio)
  User --> (Ver un negocio)
  User --> (Filtrar negocios)
  User --> (Buscar negocios)
  User --> (Ordenar negocios)
  User --> (Agrupar negocios)
  User --> (Exportar negocios)
  User --> (Importar negocios)

  
  (Crear un negocio) .-> (Añadir detalles del negocio) : include
  (Editar un negocio) .-> (Modificar datos del negocio) : include
  (Eliminar un negocio) .-> (Eliminar asociaciones) : include
  (Ver un negocio) .-> (Ver detalles y actividad) : include
  (Filtrar negocios) .-> (Crear filtros personalizados) : include
  (Buscar negocios) .-> (Usar palabras clave) : include
  (Ordenar negocios) .-> (Seleccionar criterios de orden) : include
  (Agrupar negocios) .-> (Ver totales y promedios) : include
  (Exportar negocios) .-> (Seleccionar datos para exportar) : include
  (Importar negocios) .-> (Asociar con elementos existentes) : include
}
@enduml
```