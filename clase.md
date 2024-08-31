```mermaid
classDiagram
    
    class Jugador {
        +String Nombre
        +String Numero Camiseta
        +borrowBook(Book book)
        +returnBook(Book book)
    }

    class Partido {
        +String Fecha
        +String Cancha
        +addBook(Book book)
        +removeBook(Book book)
    }

    class Tarjetas {
        +String Roja
        +List Amarilla
        +addMember(Member member)
    }

    Library "1" --  Jugador
    Library "1" --  Partido
    Library "1" --  Tarjetas
