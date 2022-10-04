

# MÓDULO 2

### => Aula - TIPOS DE JOIN

***

**LEFT JOIN** *simples* - Busca informações principais (from) na tabela 1 e caso tenha informações em comum na tabela 2, traz também.


**LEFT JOIN** com *where is NULL* - Busca informações principais na tabela 1, cruza com a tabela 2 e só vai trazer o que tem na tabela 1 puro, ignorando o que tiver em comum em 1 e 2.


**INNER JOIN** - Só traz os dados que tiver em comum nas tabelas 1 e 2.


**RIGHT JOIN** *simples* - Busca informações principais da tabela 2 e caso tenha em comum na 1, traz também. 


**RIGHT JOIN** com *where is NULL* - Busca informações principais na tabela 1, cruza com a tabela 2, só vai trazer o que tem na tabela 2 puro, ignorando o que tiver em comum em 1 e 2.


**FULL OUTER JOIN** *simples* - Traz TUDO, os resultados da tabela 1 e 2 e o que tiver em comum nas duas tabelas.


**FULL OUTER JOIN** com *where is NULL* - Traz somente o que estiver na tabela 1 e 2, sem cruzamento. (o contrário do inner join).


---

**EXERCÍCIO**

*O pessoal de Marketing fez algumas campanhas no mês de abril e querem saber quais os clientes que compraram nesse mês para fazer uma pesquisa.*

Será enviada a base de dados obtida com o código abaixo: 

```
SELECT
S.*,
ca.city
FROM sales as S 
INNER JOIN Campaing AS CA 
ON CA.customer_id = S.customer_id
WHERE S.order_date LIKE '2022-04%'
```



***

| *Quanto mais otimizada a sua consulta, menos trabalho para o seu banco de dados, ou seja, se usar menos dados, a consulta será muito mais rápida.* |

***



**#QUERO MAIS**  - Bases de dados para consultas gratuitas em período de teste: Google Cloud e Banco de Dados SQL do Azure.







