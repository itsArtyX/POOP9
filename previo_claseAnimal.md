@startuml
class Animal{
    -nombre: String
    -lugarOrigen: String
    -color: String
    +sonido(String): void
    +comer(): void
}

class AnimalAcuatico{
    -numeroAletas: int
    +nadar(): void
    +comer(): void
}

class Ballena{
    -largo: int
    +pelearConPinocho(): void
}

class AnimalTerrestre{
    -numeroPatas: int
    +correr(): void
    +comer(): void
}

class Perro{
    -colorCollar: String
    +hacerTrucos(): void
}

class AnimalAereo{
    -numeroAlas: int
    +volar(): void
    +comer(): void
}

class Pajaro{
    -tipoPico: String
    +recolectarRamas(): void
}

Animal <|-- AnimalAcuatico : class
Animal <|-- AnimalTerrestre: class
Animal <|-- AnimalAereo : class

AnimalAcuatico <|-- Ballena : class
AnimalTerrestre <|-- Perro : class
AnimalAereo <|-- Pajaro : class

@enduml