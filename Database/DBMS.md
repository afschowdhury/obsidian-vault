#database 


**Database Management System:** The software which is used to manage databases is called Database Management System (DBMS).

 - software to manage database
- Database, Database Server, Database System , Data Server, DBMS offer used interchangeably

For Example, MySQL, Oracle, etc. are popular commercial DBMS used in different applications. DBMS allows users the following tasks: 

-   **Data Definition:** It helps in the creation, modification, and removal of definitions that define the organization of data in the database. 
-   **Data Updation:** It helps in the insertion, modification, and deletion of the actual data in the database. 
-   **Data Retrieval:** It helps in the retrieval of data from the database which can be used by applications for various purposes. 
-   **User Administration:** It helps in registering and monitoring users, enforcing data security, monitoring performance, maintaining data integrity, dealing with concurrency control, and recovering information corrupted by unexpected failure.

## Paradigm Shift from File System to DBMS

 File System manages data using files on a hard disk. Users are allowed to create, delete, and update the files according to their requirements. Let us consider the example of file-based University Management System. Data of students is available to their respective Departments, Academics Section, Result Section, Accounts Section, Hostel Office, etc. Some of the data is common for all sections like Roll No, Name, Father Name, Address, and Phone number of students but some data is available to a particular section only like Hostel allotment number which is a part of the hostel office. Let us discuss the issues with this system:

-   **Redundancy of data:** Data is said to be redundant if the same data is copied at many places. If a student wants to change their Phone number, he or has to get it updated in various sections. Similarly, old records must be deleted from all sections representing that student.
-   **Inconsistency of Data:** Data is said to be inconsistent if multiple copies of the same data do not match each other. If the Phone number is different in Accounts Section and Academics Section, it will be inconsistent. Inconsistency may be because of typing errors or not updating all copies of the same data.
-   **Difficult Data Access:** A user should know the exact location of the file to access data, so the process is very cumbersome and tedious. If the user wants to search the student hostel allotment number of a student from 10000 unsorted students’ records, how difficult it can be.
-   **Unauthorized Access:** File Systems may lead to unauthorized access to data. If a student gets access to a file having his marks, he can change it in an unauthorized way.
-   **No Concurrent Access:** The access of the same data by multiple users at the same time is known as concurrency. The file system does not allow concurrency as data can be accessed by only one user at a time.
-   **No Backup and Recovery:** The file system does not incorporate any backup and recovery of data if a file is lost or corrupted.

These are the main reasons which made a shift from file system to DBMS.

**Advantages of DBMS**

 DBMS helps in efficient organization of data in database which has following advantages over typical file system:

-   **Minimized redundancy and data inconsistency:** Data is normalized in DBMS to minimize the redundancy which helps in keeping data consistent. For Example, student information can be kept at one place in DBMS and accessed by different users.This minimized redundancy is due to primary key and foreign keys
-   **Simplified Data Access:** A user need only name of the relation not exact location to access data, so the process is very simple.
-   **Multiple data views:** Different views of same data can be created to cater the needs of different users. For Example, faculty salary information can be hidden from student view of data but shown in admin view.
-   **Data Security:** Only authorized users are allowed to access the data in DBMS. Also, data can be encrypted by DBMS which makes it secure.
-   **Concurrent access to data:** Data can be accessed concurrently by different users at same time in DBMS.
-   **Backup and Recovery mechanism:** DBMS backup and recovery mechanism helps to avoid data loss and data inconsistency in case of catastrophic failures.