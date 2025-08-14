# Banco de Dados I

## SELECT

```sql
select cod_cliente as codigo, nome_cliente as nome
from cliente where cod_cliente = 20
order by codigo desc;

select * from cliente, pedido
where cliente.cod_cliente = pedido.cod_cliente;

select cod_pedido, clente.cod_cliente, cliente.nome_cliente, pedido.cod_vendedor, nome_vendedor
from cliente, pedido, vendedor
where cliente.cod_cliente = pedido.cod_cliente
	and pedido.cod_vendedor = vendedor.cod_vendedor;

select cod_cliente from pedido
group by pedido.cod_cliente;

select distinct cod_cliente from pedido;

select cod_cliente, count(*) from pedido
group by pedido.cod_cliente;

select cod_vendedor, count(*) as qtde_pedidos from pedido
group by pedido.cod_vendedor
order by qtde_pedidos desc;


```




