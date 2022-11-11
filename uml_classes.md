@startuml
class Event{
    +startTime: DataTime
    +nombre: String
    +RegistrationClosed: boolean
    +exceute()
}

interface Hola{
    +perro: int
    -gato: String
}

class Foo{
    +estado: boolean
}

Hola <|-- Foo : interfaz

@enduml