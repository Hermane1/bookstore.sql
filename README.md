-- Create a table named 'Books' with the following columns:
```sql
CREATE TABLE Books (
    BookID INTEGER PRIMARY KEY,  -- Unique identifier for each book, primary key
    Title TEXT,  -- Title of the book
    Author TEXT,  -- Author of the book
    PublicationYear INTEGER,  -- Year the book was published
    Price REAL  -- Price of the book, can include decimal values
);
```sql
-- Insert data into the 'Books' table
INSERT INTO Books (BookID, Title, Author, PublicationYear, Price) VALUES 
(1, 'To Kill a Mockingbird', 'Harper Lee', 1960, 10.99),  -- First book entry
(2, '1984', 'George Orwell', 1949, 9.99),  -- Second book entry
(3, 'The Great Gatsby', 'F. Scott Fitzgerald', 1925, 14.99),  -- Third book entry
(4, 'Beloved', 'Toni Morrison', 1987, 17.00),  -- Fourth book entry
(5, 'For Colored Girls who have considered suicide/ When the rainbow is enuf', 'Ntozake Shange', 1976, 13.69);  -- Fifth book entry with corrected title

-- Retrieve all books from the 'Books' table
SELECT * FROM Books;
```sql
SELECT * FROM Books;

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
