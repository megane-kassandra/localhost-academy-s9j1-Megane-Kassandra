# Version postgreSQL equivalente

CREATE TABLE products (
id id INTEGER GENERATED ALWAYS AS IDENTITY PRIMARY KEY ,
name TEXT NOT NULL ,
price price NUMERIC (10 , 2) NOT NULL ,
stock INTEGER DEFAULT 0
);
