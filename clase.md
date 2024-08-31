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
    }

    Liga "1" --  Jugador
    Liga "1" --  Partido
    Liga "1" --  Tarjetas
