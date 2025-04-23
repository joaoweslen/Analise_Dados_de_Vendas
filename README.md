# <img alt="Simbolo Python" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg"> Análise de Vendas

Este repositório contém um notebook Jupyter que realiza a **limpeza, análise e visualização de dados de vendas** a partir de um dataset de uma Superstore. O objetivo é identificar **tendências regionais, padrões sazonais e correlações**.

---

## Índice

1. [Sobre o Projeto](#sobre-o-projeto)  
2. [Pré-requisitos](#pré-requisitos)  
3. [Instalação](#instalação)  
4. [Estrutura dos Dados](#estrutura-dos-dados)  
5. [Descrição do Notebook](#descrição-do-notebook)  
6. [Resultados](#resultados)  
7. [Como Executar](#como-executar)  

---

## Sobre o Projeto

O projeto tem como foco a análise exploratória e visual de um dataset de vendas contendo informações sobre pedidos, produtos, clientes, regiões, descontos e lucros. A análise inclui:

- **Tratamento e conversão de datas**  
- **Criação de colunas derivadas (mês/ano, volume total etc.)**  
- **Visualizações com `matplotlib` e `seaborn`**  
- **Matriz de correlação entre variáveis numéricas**  
- **Gráficos de tendência de vendas e volume por região e por tempo**  

---

## Pré-requisitos

- Python 3.8+  
- Jupyter Notebook ou JupyterLab

## Instalação

1. Clone este repositório:
```
git clone https://github.com/joaoweslen/Analise_Dados_de_Vendas.git
```

2. Crie e ative um ambiente virtual (opcional):
 ```
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
```

3. Instale as dependências:
```
pip install -r requirements.txt
```

## Estrutura dos Dados

- **Arquivo CSV**: `vendas.csv`  
- **Formato**: delimitado por ponto e vírgula (`;`)

As colunas principais incluem:

| Coluna                          | Descrição                             |
|---------------------------------|---------------------------------------|
| `Order ID`                      | Identificador único do pedido         |
| `Order Date`                    | Data do pedido                        |
| `Ship Date`                     | Data de envio                         |
| `Region`                        | Região geográfica do cliente          |
| `Category`                      | Categoria do produto                  |
| `Product Name`                  | Nome do produto                       |
| `Sales`                         | Valor da venda ($)                    |
| `Quantity`                      | Quantidade vendida                    |
| `Discount`                      | Desconto aplicado                     |
| `Profit`                        | Lucro gerado                          |

## Descrição do Notebook

1. **Leitura e limpeza dos dado**
   - Conversão de datas
   - Verificação de nulos e duplicatas
2. **Análise exploratória**
   - Vendas por região
   - Variação mensal do volume de vendas
   - Correlação entre variáveis numéricas
3. **Visualizações**
   - Gráficos de linha, barras e dispersão
   - Matriz de correlação com heatmap

## Resultados

- Identificadas diferenças regionais significativas nas vendas. 
- Detectada sazonalidade (flutuação mensal). 
- Correlação fraca entre desconto e quantidade vendida.
- Lucro não acompanha sempre o volume de vendas (especialmente em produtos com alto desconto).

## Como Executar

1. Abra o Jupyter Notebook:
```bash
jupyter notebook analise_dados_de_vendas.ipynb
```
2. Execute as células em ordem.  
3. Verifique outputs, gráficos e métricas.