# Dashboard de Vendas de Supermercado

Este projeto é uma aplicação interativa desenvolvida com **Dash** e **Plotly** que permite a visualização e análise de dados de vendas de supermercados. O painel oferece várias opções de visualização, como filtragem de cidades e seleção de variáveis de análise.

## Funcionalidades

- **Filtragem por Cidade**: Os usuários podem selecionar múltiplas cidades para visualizar os dados específicos de cada uma.
- **Escolha de Variável de Análise**: É possível alternar entre duas variáveis de interesse: "gross income" (receita bruta) e "Rating" (avaliação).
- **Visualizações Gráficas**:
  - Receita ou avaliação por cidade.
  - Receita ou avaliação por método de pagamento.
  - Receita ou avaliação por gênero.
  - Receita ou avaliação ao longo do tempo.
  - Receita ou avaliação por linha de produtos.

## Estrutura do Código

- **Layout**: O layout da aplicação é organizado em uma estrutura de colunas usando `Dash Bootstrap Components` para criar uma interface responsiva e agradável.
- **Callbacks**: Os gráficos são atualizados dinamicamente com base nos filtros selecionados (cidades e variável de análise). As funções de callback processam os dados filtrados e geram gráficos usando `Plotly Express`.
  
## Dependências

As bibliotecas necessárias para rodar o projeto estão listadas abaixo:

- `dash`
- `dash-bootstrap-components`
- `dash-bootstrap-templates`
- `plotly`
- `pandas`
- `numpy`

Para instalar as dependências, execute:
```bash
pip install dash dash-bootstrap-components dash-bootstrap-templates plotly pandas numpy
```

## Executando o Projeto

1. Certifique-se de que o arquivo de dados **supermarket_sales.csv** esteja na mesma pasta que o código.
2. Execute o seguinte comando no terminal para iniciar o servidor:
   ```bash
   python app.py
   ```
3. Acesse o painel no seu navegador em `http://localhost:8050`.

## Estrutura de Arquivos

```
📁 projeto-dash
│
├── app.py                # Código principal da aplicação
├── supermarket_sales.csv  # Arquivo CSV contendo os dados de vendas do supermercado
└── README.md              # Arquivo de documentação do projeto
```

## Detalhes dos Dados

O arquivo **supermarket_sales.csv** contém dados de vendas com as seguintes colunas principais:
- **City**: Cidades onde as vendas ocorreram.
- **Product line**: Categoria do produto vendido.
- **Gender**: Gênero dos compradores.
- **Payment**: Método de pagamento utilizado.
- **gross income**: Receita bruta da venda.
- **Rating**: Avaliação dada pelo cliente.

## Temas e Estilos

Este projeto utiliza o tema **Minty** do Bootstrap para estilizar a interface gráfica, aplicando o mesmo estilo aos gráficos.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---

Esse README cobre os principais aspectos do seu código e o ajuda a entender e rodar o projeto facilmente.
