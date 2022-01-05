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
FROM Employee E  
WHERE 2*E.age<20
```
> ```sql
SELECT E.dno  
FROM Enployee E  
WHERE 2*E.age<10;
> ```

4.
Na voljo ni nobenega indeksa:  
```sql
SELECT DISTINCT *  
FROM Employee
```
>```sql
SELECT  *  
FROM Employee

5.
Na voljo ni nobenega indeksa:    
```sql
SELECT AVG (E.sal)  
FROM Employee E  
GROUP BY E.dno  
HAVING E.dno=22
```
>```sql
SELECT AVG (E.sal)  
FROM Employee E   
WHERE E.dno=22

6.
sid je tuj ključ relacije Reserves, ki kaže na relacijo Sailors:  
```sql
SELECT S.sid  
FROM Sailors S, Reserves R  
WHERE S.sid=R.sid
```
>```sql
SELECT R.sid  
FROM Reserves R  
WHERE R.sid

X.
Na voljo ni nobenega indeksa:    
```sql
```
>```sql
SELECT AVG (E.sal)  
FROM Employee E   
WHERE E.dno=22

