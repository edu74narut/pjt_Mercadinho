<img src="https://aquiles.click/wp-content/uploads/2021/08/supermercado-online-1200x480.jpg.webp">

# Geek Shop - Sistema de Cadastro e Venda de Produtos

Este projeto é um sistema simples de gerenciamento de produtos e carrinho de compras desenvolvido em Python. Ele permite cadastrar produtos, listar os disponíveis, adicionar produtos ao carrinho, visualizar o carrinho e finalizar o pedido.

## Funcionalidades

- **Cadastrar Produto:** Permite adicionar novos produtos ao sistema, informando nome e preço.
- **Listar Produtos:** Exibe todos os produtos cadastrados com seus detalhes.
- **Comprar Produto:** Adiciona produtos ao carrinho, permitindo múltiplas unidades do mesmo item.
- **Visualizar Carrinho:** Mostra os produtos adicionados ao carrinho e suas quantidades.
- **Fechar Pedido:** Calcula o valor total da compra e exibe a fatura final.

## Como usar

1. Execute o script principal:

    ```
    python mercado.py
    ```

2. No menu exibido, escolha a opção desejada digitando o número correspondente.

3. Siga as instruções para cadastrar produtos, comprar e finalizar pedidos.

## Estrutura do Código

- **models/produto.py**  
  Contém a classe `Produto` que representa um produto com código, nome e preço.

- **utils/helper.py**  
  Contém a função `formata_float_str_moeda` para formatar valores numéricos em moeda brasileira.

- **mercado.py**  
  Arquivo principal que contém o menu interativo e as funções para gerenciar produtos e carrinho.

### Classe Produto (models/produto.py)

- Atributos:
  - `codigo`: Identificador único automático para cada produto.
  - `nome`: Nome do produto.
  - `preco`: Preço do produto.

- Métodos:
  - `__init__`: Inicializa o produto com nome e preço, atribuindo um código único.
  - `__str__`: Retorna uma string formatada com os detalhes do produto, incluindo o preço formatado como moeda.

### Função auxiliar (utils/helper.py)

```
def formata_float_str_moeda(valor: float) -> str:
return f'R$ {valor:,.2f}'
```

Usada para exibir os preços dos produtos e o valor total do pedido de forma amigável.

## Requisitos

- Python 3.x
- Módulos padrão: `typing` e `time`


## Observações

- O sistema utiliza um menu interativo via terminal para facilitar o uso.
- O código utiliza `sleep` para melhorar a experiência visual durante a execução.
- O carrinho é esvaziado após o fechamento do pedido.

---

Se quiser contribuir, sinta-se à vontade para abrir issues ou pull requests!

---

**Geek Shop** - Projeto de estudo para gerenciamento básico de produtos e vendas em Python.



