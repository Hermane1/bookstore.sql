CREATE TABLE Books (
    BookID INTEGER PRIMARY KEY,
    Title TEXT,
    Author TEXT,
    PublicationYear INTEGER,
    Price REAL
);
INSERT INTO Books (BookID, Title, Author, PublicationYear, Price) VALUES
(1, 'To Kill a Mockingbird', 'Harper Lee', 1960, 10.99),
(2, '1984', 'George Orwell', 1949, 9.99),
(3, 'The Great Gatsby', 'F. Scott Fitzgerald', 1925, 14.99),
(4, 'Beloved', 'Toni Morrison', 1987, 17.00),
(5, 'For Colored Girls Who Have Considered Suicide / When the Rainbow Is Enuf', 'Ntozake Shange', 1976, 13.69);
SELECT * FROM Books;
SELECT * FROM Books WHERE PublicationYear > 2000;
SELECT * FROM Books WHERE Author = 'George Orwell';
UPDATE Books SET Price = 9.99 WHERE Title = '1984';
DELETE FROM Books WHERE Title = 'Beloved';
Reflection
This assignment provided me with hands-on experience in setting up and manipulating a SQLite database using basic SQL commands. Creating a database and tables, inserting data, and performing various queries were straightforward tasks that reinforced my understanding of SQL syntax and operations. The primary challenge I faced was ensuring the correct data types for each column and maintaining the consistency of the data. Working with SQLiteStudio made the process user-friendly, as it offers a graphical interface to manage the database easily. Overall, this exercise has deepened my appreciation for database management and the power of SQL in handling data efficiently.
