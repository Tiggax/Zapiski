Za vsako poizvedbo najdite razlog zakaj optimizator morda ne bo izbral  
najidealnejšega plana. Zapišite poizvedbo, ki ne bo „zmedla“ optimizator.  
1. Indeks je na voljo na atributu age:  

```sql
SELECT E.dno  
FROM Employee E  
WHERE E.age=20 OR E.age=10  
```
2. B+ indeks je na voljo na atributu age :  
```sql
SELECT E.dno  
FROM Employee E  
WHERE E.age<20 AND E.age>10
```

namesto OR v 1. lahko damo unija.
1.
```sql
SELECT E.dno  
FROM Employee E  
WHERE E.age=20

UNION

SELECT E.dno
FROM Employee E
WHERE E.age=10  :
```

2.

```sql
SELECT E.dno  
FROM Employee E  
WHERE E.age BETWEEN 11 AND 19:
```

3.
Indeks je na voljo na atributu age:  
```sql
SELECT E.eIno  
FROM Enlployee E  
WHERE 2*E.age<20
```
> 