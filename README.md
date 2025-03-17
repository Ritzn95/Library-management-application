# Library Management Application

Built an application that will manage all books present in a library and manage all students who can access these books.

## Following are the apis that we would need

### Created the following APis using Java

- Get api/v1/GetAllBooks
- Post api/v1/AddNewBook. Pass in body (Book book)
- Get api/v1/GetAllStudents
- Post api/v1/AddNewStudent. Pass in body (Student student)
- Put api/v1/AllocateBookToStudent?studentId=a&bookId=b
  - Reduce Available copies of book by 1
  - Increase Allocated copies to that student by 1 (max 3)
- Put api/v1/UnAllocateBookToStudent?studentId=a&bookId=b

### Created the following Book Model

- bookId: string
- Name:string
- TotalCopies: int
- No.ofCopiesAvailable

### Created the following Student Model

- studentId: string
- Name: string
- booksAllocated: int

### Data Persistency: Used redis Database to Store information.
