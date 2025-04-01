## Øvelse 2
2.1
```SQL

SELECT * FROM bolche
```

2.2
```SQL

SELECT * FROM bolche WHERE color="red"
```

2.3
```SQL

SELECT * FROM bolche WHERE color="red" OR color="blue"
```

2.4
```SQL

SELECT * FROM bolche WHERE color!="red" ORDER BY name ASC 
```

2.5
```SQL

SELECT * FROM bolche WHERE name LIKE "b%"
```

2.6
```SQL

SELECT * FROM bolche WHERE name LIKE "%e%"
```

2.7
```SQL
SELECT * FROM bolche where [weight (g)]<10 ORDER BY [weight (g)] ASC
```

2.8
```SQL
SELECT name FROM bolche WHERE [weight (g)]>=10 AND [weight (g)]<=12 ORDER BY name, [weight (g)]
```

2.9
```SQL
SELECT * FROM bolche ORDER BY [weight (g)] DESC LIMIT (3)
```

2.10
```SQL
SELECT * FROM bolche ORDER BY RANDOM() LIMIT (1)
```

2.10
```SQL
SELECT * FROM bolche ORDER BY RANDOM() LIMIT (1)
```

## Øvelse 3


## Øvelse 4

4.2
```SQL

SELECT bolche.name FROM bolche INNER JOIN color ON bolche.color_id = color.id where color.name = "red"
```

4.3
```SQL

SELECT bolche.name FROM bolche INNER JOIN color ON bolche.color_id = color.id where color.name = "red" OR color.name="blue"
```

4.4
```SQL
SELECT bolche.name FROM bolche INNER JOIN color ON bolche.color_id = color.id where color.name != "red"  ORDER BY bolche.name ASC
```

4.5
```SQL
SELECT bolche.name FROM bolche INNER JOIN color ON bolche.color_id = color.id where bolche.name LIKE "b%"
```

4.6
```SQL

SELECT bolche.name FROM bolche INNER JOIN color ON bolche.color_id = color.id where bolche.name LIKE "%e%"
```

4.7
```SQL
SELECT bolche.name FROM bolche INNER JOIN color ON bolche.color_id = color.id where bolche.[weight (g)]<10
```

4.8
```SQL
SELECT bolche.name FROM bolche INNER JOIN color ON bolche.color_id = color.id where bolche.[weight (g)] BETWEEN 10 AND 12 ORDER BY bolche.name, bolche.[weight (g)] 
```
(forkert?) den sorterer ikke korrekt alfabetisk

4.9
```SQL
SELECT bolche.name FROM bolche INNER JOIN color ON bolche.color_id = color.id ORDER BY bolche.[weight (g)] DESC LIMIT (3)
```

4.10
```SQL
SELECT * FROM bolche INNER JOIN color ON bolche.color_id = color.id ORDER BY RANDOM() LIMIT (1)
```


## Øvelse 5
```SQL
SELECT name, (price * 3.5) AS net_price_pr_kg, (price * 3.5) AS gross_price_per_kg FROM bolche ORDER BY name ASC
```