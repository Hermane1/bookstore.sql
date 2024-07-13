CREATE TABLE Books (
    BookID INTEGER PRIMARY KEY,
    Title TEXT,
    Author TEXT,
    PublicationYear INTEGER,
    Price REAL
);
Insert Data into the Books Table:

INSERT INTO Books (BookID, Title, Author, PublicationYear, Price) VALUES
(1, 'To Kill a Mockingbird', 'Harper Lee', 1960, 10.99),
(2, '1984', 'George Orwell', 1949, 9.99),
(3, 'The Great Gatsby', 'F. Scott Fitzgerald', 1925, 14.99)
(4, 'Beloved', 'Toni Morrison', 1987, 17.00)
(5, 'For Colored Girls who have condsidered suicide/ When the rainbow is enuf, 'Ntozake Shanhange',1976, 13.69)
**Retrieve all books in the Books table**:
sql
SELECT * FROM Books;
Retrieve all books published after 2000:

SELECT * FROM Books WHERE PublicationYear > 2000;
Retrieve all books written by George Orwell:

SELECT * FROM Books WHERE Author = 'Harper Lee';
Update the price of '1984':

UPDATE Books SET Price = 9.99 WHERE BookID = 1;
Delete '1984':

UPDATE Books SET Price = 10.99 WHERE BookID = 2;
Delete 'Beloved'

DELETE FROM Books WHERE BookID = 4;
Reflection
This assignment provided me with hands-on experience in set
