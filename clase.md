```mermaid
classDiagram
    
    class Jugador {
        +String name
        +String memberId
        +borrowBook(Book book)
        +returnBook(Book book)
    }

    class Partido {
        +String name
        +String employeeId
        +addBook(Book book)
        +removeBook(Book book)
    }

    class Tarjetas {
        +String name
        +List books
        +List members
        +List librarians
        +addMember(Member member)
    }

    Library "1" -- "contains" Jugador
    Library "1" -- "registers" Partido
    Library "1" -- "manages" Tarjetas
