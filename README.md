# sql-style
A style guide for SQL

### Key/Reserverd words should be lower case and names should be upper case   
Like this:  
```SQL
select FIELD from FILE where SOMETHING = OTHERTHING 
```  
  
Not this:  
```SQL
SELECT field FROM file WHERE something = otherthing
```
  
Never this:  
```SQL
Select Field From File Where Something = Otherthing 
```



### Include the “as” keyword when aliasing a variable or table name.  Always use a full description for correlation names, not just a letter.   
Like this:  
```SQL
select FIELD as ALIAS_NAME
from FILE as FILE_ALIAS
```  
  
Not this:  
```SQL
select FIELD ALIAS_NAME
from FILE FILE_ALIAS
```
  
Never this:  
```SQL
select FIELD F
from TABLE T
```

### Always include the JOIN type rather than relying on the default join.
Like this:  
```SQL
select FIELD 
from FILE1  
inner join FILE2
```  
  
Not this:  
```SQL
select FIELD 
from FILE1  
join FILE2
```  
  
Never this:  
```SQL
select FIELD
from FILE1, FILE2
```
