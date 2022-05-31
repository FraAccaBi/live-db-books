# DB Biblioteca

## Books

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
title:          VARCHAR(50) NOTNULL INDEX       
plot:           TEXT NULL
pages:          SMALLINT NULL
year:           YEAR   
cover_img:      VARCHAR(255) NULL
_____________________________
avaibility:
price:
online_content:
discount:
language:
bestseller:
nr_chapters:
edition:
new_release:
rarity:
quantity:

## Copies

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
ean:            VARCHAR(16) NULL
isbn:           VARCHAR(13) NULL    
position:       VARCHAR(15) NULL
language:       VARCHAR(5) NULL DEFAULT('it-IT')

## Users

id:         PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:       VARCHAR(50) NOTNULL
lastname:   VARCHAR(50) NOTNULL
age:        TINYINT NULL
email:      VARCHAR(50) NOTNULL UNIQUE
tel_nr:     VARCHAR(15) NULL
address:    VARCHAR(50) NOTNULL

## Loans

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
start_date:     DATETIME NOTNULL 
end_date:       DATETIME NOTNULL

## Genres

id:     PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:   VARCHAR(20) NOTNULL

## Authors

id:             PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:           VARCHAR(50) NOTNULL
lastname:       VARCHAR(50) NOTNULL
nationality:    VARCHAR(30) NULL

## Publishers

id:     PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:   VARCHAR(50) NOTNULL

## Conditions

id:     PK NOTNULL UNIQUE INDEX AUTOINCREMENTAL
name:   VARCHAR(50) NOTNULL


