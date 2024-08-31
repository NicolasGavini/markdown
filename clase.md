```mermaid
classDiagram
    class Book {
        +String title
        +String author
        +String isbn
        +boolean isAvailable()
    }

    class Member {
        +String name
        +String memberId
        +borrowBook(Book book)
        +returnBook(Book book)
    }

    class Librarian {
        +String name
        +String employeeId
        +addBook(Book book)
        +removeBook(Book book)
    }

    class Library {
        +String name
        +List books
        +List members
        +List librarians
        +addMember(Member member)
    }

    Library "1" -- "contains" Club
    Library "1" -- "registers" Goles
    Library "1" -- "manages" Asistencias
