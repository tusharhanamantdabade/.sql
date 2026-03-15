1) retrieve all books in the 'Fiction' genre
   select *from books
   where genre='Fiction';

2)find books published after the year 1950:
  select * from books
  where published_year>1950;

3) list all the customers from the canada:
   select *from customers
   where country='canada';

4) show orders placed in november 2023:
   select * from orders
   where order_date between '2023-11-1' and '2023-11-30';

5)retrieve total stock of books available:
  select sum(stock) as total_stock from books;

6)find the details of the most expensive book:
 select * from books order by price desc limit 1;

7) show all customers  who ordered more than 1 quantity of book:
   select * from orders
   where quantity>1;

8)retrieve all orders where the total amount exceeds $20:
  select * from orders
  where total_amount>20;

9)list all genre available in the books table:
  select distinct genre from books;

10) find the book with the lowest stock:
   select *from books order by stock limit 1;

11)calculate the total revenue generated from all orders:
  select sum(total_amount)as revenue from orders;
  
