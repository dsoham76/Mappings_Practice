# Mappings_Practice

## Framework and Language

> Framework: SpringBoot Language: Java 8

## Data flow

1.  Controller

        1.1  Address Controller
            - @GetMapping("addresses") - get all address
            - @PostMapping("address")- to add an address
            - @DeleteMapping("address/{address_id}")- to delete an address
        1.2  Book Controller
            - @GetMapping("books") - get all books
            - @PostMapping("book")- to add a book
            - @DeleteMapping("book/{book_id}")- to delete a book
        1.3  Course Controller
            - @GetMapping("courses") - get all courses
            - @PostMapping("course")- to add a course
            - @DeleteMapping("course/{course_id}")- to delete a course
        1.4  Laptop Controller
            - @GetMapping("laptops") - get all laptops
            - @PostMapping("laptop")- to add a laptop
            - @DeleteMapping("laptop/{laptop_id}")- to delete a laptop
        1.5  Student Controller
            - @GetMapping("students") - get all students
            - @PostMapping("student")- to add a student
            - @DeleteMapping("student/{student_id}")- to delete a student
        

3.  Services

        1.1  Address Service
            - getAllAddress() - get all address
            - addAddress(Address address) - to add an address
            - deleteAddress(Integer address_id) - to delete an address
        1.2  Book Service
            - getAllBooks() - get all books
            - addBook(Book book) - to add a book
            - deleteBook(Integer book_id) - to delete a book
        1.3  Course Service
            - getAllCourses() - get all courses
            - addCourse(Course course) - to add a course
            - deleteCourse(Integer course_id) - to delete a course
        1.4  Laptop Service
            - getAllLaptops() - get all laptops
            - addCLaptop(Laptop laptop) - to add a laptop
            - deleteLaptop(Integer laptop_id) - to delete a laptop
        1.5  Student Service
            - getAllStudents() - get all students
            - addStudent(Student student) - to add a student
            - deleteStudent(Integer student_id) - to delete a student

4.  Repository

        1.1 IAddressRepo
        1.2 IBookRepo
        1.3 ICourseRepo
        1.4 ILaptopRepo
        1.5 IStudentRepo

6.  Database Design

        4.1 Address Model:
                - Integer addressId;
                - String landmark;
                - String zipcode;
                - String district;
                - String state;
                - String country;
        4.2 Book Model:
                - Integer ID;
                - String title;
                - String author;
                - String description;
                - String price;
                - Student student;
        4.3 Course Model:
                - Integer ID;
                - String title;
                - String description;
                - String duration;
                - List<Student> studentList;
        4.4 Laptop Model:
                - Integer ID;
                - String name;
                - String brand;
                - Integer price;
                - Student student;
        4.5 Student Model:
                - Integer ID;
                - String name;
                - String age;
                - String phoneNumber;
                - String branch;
                - String department;
                - Address address
## Data Structure Used in Project

     JPARepository has been used as primay datastructure
