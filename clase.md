```mermaid
classDiagram
    
    class Jugador {
        +Nombre
        +Numero Camiseta
    }

    class Partido {
        +Fecha
        +Cancha
    }

    class Tarjetas {
        +Roja
        +Amarilla
        +addMember(Member member)
    }

    Library "1" --  Jugador
    Library "1" --  Partido
    Library "1" --  Tarjetas
