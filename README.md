# posstgreSQL

-- insert into customer(Costumer_ID , name, age, Address)
-- values(001,'Om Prakash Rajbanshi',23, 'Biratnagar'),
-- (002,'Suraj Kumar Rajbanshi',22,'Jogbani'),
-- (003, 'Mohammed Zibreel',39,'HaathKhola'),
-- (004,'Matrika Pokhrel',44,'Ithari'),
-- (005,'Bharat Budhathoki',56,'Dharan'),
-- (006,'Naresh Shah',45,'Nepalgunj');





-- update customer
-- set profession='IT Engineer'
-- where customer_id IN(001,002)



--( to delete profession table)
-- alter table customer
-- drop column profession;



-- (to add profession table)
-- alter table customer
-- add column profession VARCHAR(90);




-- (to set professiojn in the column)

-- update customer
-- set profession='IT Engineer';

-- insert into "Products"(product_name)
-- values('Iphone'),
-- ('Samsung'),
-- ('Google Pixel');

-- create table products(
-- product_name VARCHAR(100),
-- payment_id VARCHAR(100),
-- customer_id INT
-- );

 -- select * from products;

 
 -- insert into products(product_name,payment_id,customer_id)
 -- values('Ihpone','abc123',1),
 -- ('Samsung','abcd1234',2),
 -- ('Google Pixel', 'ab12', 3);



-- use case of inner join
 -- select customer.name,customer.address,products.product_name,products.payment_id
 -- from customer
 -- inner join products 
 -- on customer.customer_id=products.customer_id;


-- use case of left join
  select customer.name,customer.address,products.product_name,products.payment_id
 from customer
 left join products 
 on customer.customer_id=products.customer_id;

 

   -- use case of full join
   select customer.name,customer.address,products.product_name,products.payment_id
 from customer
 full join products 
 on customer.customer_id=products.customer_id;

 

