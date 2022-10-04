

# MÓDULO 2

### => Aula - TIPOS DE JOIN

***

**LEFT JOIN** *simples* - Busca informações principais (from) na tabela 1 e caso tenha informações em comum na tabela 2, traz também.

![left join.jpg](C:\desktop\estudos\sql\ProjetosSQL\SQL\Aulas\left join.jpg)



**LEFT JOIN** com *where is NULL* - Busca informações principais na tabela 1, cruza com a tabela 2 e só vai trazer o que tem na tabela 1 puro, ignorando o que tiver em comum em 1 e 2.

![image-20221003200322205](C:\Users\elisa\AppData\Roaming\Typora\typora-user-images\image-20221003200322205.png)



**INNER JOIN** - Só traz os dados que tiver em comum nas tabelas 1 e 2.

![image-20221003200427157](C:\Users\elisa\AppData\Roaming\Typora\typora-user-images\image-20221003200427157.png)



**RIGHT JOIN** *simples* - Busca informações principais da tabela 2 e caso tenha em comum na 1, traz também. 

![image-20221003200506757](C:\Users\elisa\AppData\Roaming\Typora\typora-user-images\image-20221003200506757.png)



**RIGHT JOIN** com *where is NULL* - Busca informações principais na tabela 1, cruza com a tabela 2, só vai trazer o que tem na tabela 2 puro, ignorando o que tiver em comum em 1 e 2.

![image-20221003200609774](C:\Users\elisa\AppData\Roaming\Typora\typora-user-images\image-20221003200609774.png)



**FULL OUTER JOIN** *simples* - Traz TUDO, os resultados da tabela 1 e 2 e o que tiver em comum nas duas tabelas.

![image-20221003200737997](C:\Users\elisa\AppData\Roaming\Typora\typora-user-images\image-20221003200737997.png)





**FULL OUTER JOIN** com *where is NULL* - Traz somente o que estiver na tabela 1 e 2, sem cruzamento. (o contrário do inner join).

![image-20221003200846397](C:\Users\elisa\AppData\Roaming\Typora\typora-user-images\image-20221003200846397.png)



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



**DESAFIO CONQUER** - Quais são *as 10 cidades* com maior valor de venda? (precisa usar o JOIN)





***

**#QUERO MAIS**  - Bases de dados para consultas gratuitas em período de teste: Google Cloud e Banco de Dados SQL do Azure.







