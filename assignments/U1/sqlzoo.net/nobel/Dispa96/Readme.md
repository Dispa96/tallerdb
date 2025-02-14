#Elaborado por Diego Saul Pineda Andrade
```SQL
#Problema 1
SELECT yr, subject, winner
  FROM nobel
 WHERE yr = 1950

#Problema 2
SELECT winner
  FROM nobel
 WHERE yr = 1962
   AND subject = 'literature'

#Problema 3
SELECT yr,subject
  FROM nobel
 WHERE yr = 1921
   AND subject ='physics'

#Problema 4
SELECT winner
  FROM nobel
 WHERE yr >= 2000
   AND subject = 'peace'

#Problema 5
SELECT yr, subject, winner
  FROM nobel
 where yr BETWEEN 1980 AND 1989
   AND subject = 'literature'

#Problema 6
SELECT * FROM nobel
 WHERE winner IN ('Theodore Roosevelt',
                  'Thomas Woodrow Wilson',
                  'Jimmy Carter',
                    'Barack Obama')

#Problema 7
SELECT winner
FROM nobel
WHERE winner LIKE  'John %'

#Problema 8
SELECT yr, subject, winner 
FROM nobel
WHERE (subject = 'Physics' AND yr = 1980) 
   OR (subject = 'Chemistry' AND yr = 1984)

#Problema 9
SELECT yr, subject, winner 
FROM nobel
WHERE yr = 1980
AND subject NOT IN ('Chemistry', 'Medicine')

#Problema 10
SELECT yr, subject, winner
  FROM nobel
   WHERE(yr < 1910 AND subject = 'Medicine') 
   OR (yr >= 2004 AND subject = 'Literature')

#Problema 11
SELECT yr, subject, winner 
FROM nobel
WHERE winner = 'PETER GRÜNBERG';

#Problema 12
SELECT yr, subject, winner 
FROM nobel
WHERE winner = 'EUGENE O''NEILL';

#Problema 13
SELECT winner, yr, subject 
FROM nobel
WHERE winner LIKE 'Sir %'
ORDER BY yr DESC, winner ASC;

#Problema 14
SELECT winner, subject 
FROM nobel
WHERE yr = 1984
ORDER BY (subject IN ('Chemistry', 'Physics')), subject, winner;
```



