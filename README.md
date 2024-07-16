# Bookstore Database Assignment

## SQL Queries

1. **Create `Books` Table**:
    ```sql
  -- Create a table named 'Books' with the following columns:
CREATE TABLE Books (
    -- Column to store a unique identifier for each book
    BookID INTEGER PRIMARY KEY,  -- 'INTEGER PRIMARY KEY' makes this column the primary key with unique values for each row

    -- Column to store the title of the book
    Title TEXT,  -- 'TEXT' data type to store the title of the book

    -- Column to store the author of the book
    Author TEXT,  -- 'TEXT' data type to store the author's name

    -- Column to store the year the book was published
    PublicationYear INTEGER,  -- 'INTEGER' data type to store the year of publication

    -- Column to store the price of the book
    Price REAL  -- 'REAL' data type to store the price of the book, which can include decimal values
);

    ```
     **Insert Data into the `Books` Table**:
    ```sql
    INSERT INTO Books (BookID, Title, Author, PublicationYear, Price) VALUES
    (1, 'To Kill a Mockingbird', 'Harper Lee', 1960, 10.99),
    (2, '1984', 'George Orwell', 1949, 9.99),
    (3, 'The Great Gatsby', 'F. Scott Fitzgerald', 1925, 14.99)
    (4,(4, 'Beloved', 'Toni Morrison', 1987, 17.00)
    (5, 'For Colored Girls who have condsidered suicide/ When the rainbow is enuf, 'Ntozake Shanhange',1976, 13.69)
    **Retrieve all books in the `Books` table**:
    ```sql
    SELECT * FROM Books;
    ```
4. **Retrieve all books published after 2000**:
    ```sql
    SELECT * FROM Books WHERE PublicationYear > 2000;
    ```
    **Retrieve all books written by George Orwell**:
    ```sql
    SELECT * FROM Books WHERE Author = 'Harper Lee';
    ```
6. **Update the price of '1984'**:
    ```sql
    UPDATE Books SET Price = 9.99 WHERE BookID = 1;
    ```
    **Delete '1984'**:
    ```sql
    UPDATE Books SET Price = 10.99 WHERE BookID = 2;
    ```
    **Delete 'Beloved'**
   ```sql
   DELETE FROM Books WHERE BookID = 4;
   ```
   ## Reflection
   This assignment provided me with hands-on experience in setting up and manipulating a SQLite database using basic SQL commands. Creating a database and tables, inserting data, and performing various queries were straightforward tasks that reinforced my understanding of SQL syntax and operations. The primary challenge I faced was ensuring the correct data types for each column and maintaining the consistency of the data. Working with SQLiteStudio made the process user-friendly, as it offers a graphical interface to manage the database easily. Overall, this exercise has deepened my appreciation for database management and the power of SQL in handling data efficiently.
