create database
```
create database ecommerce
```

create table
```
create table Products(
    product_id int auto_increment primary key,
    name varchar(100) not null,
    description text,
    price decimal(10,2) not null,
    stock int not null,
    created_at timestamp default current_timestamp
);
```
data insertion 
```
insert into Products(name,description,price,stock,created_at)
values
('Laptop','',1000,15)
```

select 
```
select * from products
select name,price from products
select name,price from products where price > 5000
```
update 
```
update products set  price=60000 where price = 10000
```


