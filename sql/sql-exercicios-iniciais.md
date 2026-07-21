# Exercícios iniciais de SQL – Denise

## 1. SELECT simples
```sql
SELECT name, price
FROM product_list;
```

## 2. Filtros com WHERE
```sql
SELECT name, price
FROM product_list
WHERE price < 300;
```

## 3. JOIN entre product_list e category_list
```sql
SELECT DISTINCT category_list.name
FROM product_list
JOIN category_list
  ON product_list.category_id = category_list.id
WHERE product_list.price < 300;
```

## 4. Roteiro que uso antes de escrever SQL

1. O que o exercício quer mostrar?
2. De qual tabela vem cada informação?
3. Preciso de JOIN?
4. Quais colunas ligam as tabelas?
5. Preciso filtrar (WHERE)?
6. Preciso agrupar (GROUP BY)?
7. Preciso usar alguma função (COUNT, SUM, etc.)?
