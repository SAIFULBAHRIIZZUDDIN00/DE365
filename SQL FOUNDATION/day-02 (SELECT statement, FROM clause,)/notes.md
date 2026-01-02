-- 🔵 1. GET EVERYTHING FROM A TABLE
-- * means "give me all columns"
SELECT * FROM table_name;
-- Example:
SELECT * FROM employees;  -- Gets ALL columns from employees table

-- 🔵 2. GET SPECIFIC COLUMNS ONLY
-- List the columns you want, separated by commas
SELECT column1, column2 FROM table_name;
-- Example:
SELECT name, email, phone FROM customers;  -- Gets only these 3 columns

-- 🔵 3. GET UNIQUE VALUES (NO DUPLICATES)
-- DISTINCT shows each value only once
SELECT DISTINCT column_name FROM table_name;
-- Example:
SELECT DISTINCT city FROM customers;  -- Shows each city only once

-- 🔵 4. NICE FORMATTING (EASY TO READ)
-- Write each column on a new line
SELECT 
    first_name,
    last_name,
    email,
    phone_number
FROM employees;

-- 🔵 5. REAL-WORLD EXAMPLES
-- Get all product information
SELECT * FROM products;

-- Get customer names and emails only
SELECT customer_name, email FROM customers;

-- See what countries we have (no repeats)
SELECT DISTINCT country FROM customers;

-- Get employee details nicely formatted
SELECT 
    emp_id,
    first_name,
    last_name,
    salary,
    department
FROM employees;

-- 🔵 QUICK NOTES:
-- ✓ * = ALL columns
-- ✓ Separate columns with commas (like a list)
-- ✓ DISTINCT = Remove duplicates
-- ✓ Always end with ;
-- ✓ Keywords usually in CAPITAL LETTERS (SELECT, FROM, DISTINCT)
-- ✓ Table names in lowercase (employees, customers)
