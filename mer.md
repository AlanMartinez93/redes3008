```mermaid
classDiagram
    class profesor {
        +String titulo
        +String autores
        +String isbn
        +boolean isAvailable()
    }

    class alumno {
        +String name
        +String memberId
        +borrowBook(Book book)
        +returnBook(Book book)
    }
 class clase {
        +String name
        +String memberId
        +borrowBook(Book book)
        +returnBook(Book book)
    }

    class curso {
        +String name
        +String employeeId
        +addBook(Book book)
        +removeBook(Book book)
    }



    profesor --> clase : dicta
    alumno --> curso : pertenece a
    curso --> clase : en la
    
