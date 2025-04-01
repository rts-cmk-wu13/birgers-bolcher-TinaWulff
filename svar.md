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

