# CoinMarketCap Scraper

Este é um projeto de raspagem de dados feito em Python que coleta informações das 10 principais criptomoedas listadas no CoinMarketCap. O projeto utiliza as bibliotecas BeautifulSoup, Requests e Regex para extrair dados e Pandas para manipulação e análise.

## Funcionalidades

- Raspagem das 10 principais moedas no CoinMarketCap.
- Coleta de informações como:
  - Preço
  - Variação de 1 hora
  - Variação de 24 horas
  - Variação de 7 dias
  - Capitalização de mercado
  - Volume (24h)
  - Fornecimento circulante
- Criação de um dicionário com as informações de cada moeda.
- Geração de um DataFrame usando Pandas para análise de dados.

## Instalação

1. Clone o repositório:
    ```bash
    git clone https://github.com/Numl8ck/raspagem_no_coinmarketcap.git
    ```
2. Navegue até o diretório do projeto:
    ```bash
    cd raspagem_no_coinmarketcap
    ```
3. Crie um ambiente virtual (opcional, mas recomendado):
    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows, use `venv\Scripts\activate`
    ```
4. Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```

## Como usar

1. Execute o script principal:
    ```bash
    python raspagem_no_coinmarketcap.py
    ```
2. O script irá coletar as informações e exibi-las no terminal, além de gerar um DataFrame para análises adicionais.

## Exemplo de Saída

Aqui está um exemplo de saída gerada pelo script:

```python
{
    "Bitcoin": {
        "Preço": "R$220,000",
        "Variação 1h": "0.5%",
        "Variação 24h": "2.3%",
        "Variação 7d": "-1.2%",
        "Capitalização de mercado": "R$750B",
        "Volume (24h)": "R$35B",
        "Fornecimento Circulante": "18.7M BTC"
    },
    ...
}

# DataFrame
              Bitcoin	 Ethereum	 Tether BNB	 Solana USDC XRP  Dogecoin  Toncoin	Cardano
Preço        R$220,000  R$80,000  R$40,000  R$50,000  R$70,000  R$30,000 R$20,000 R$10,000        
...
```

## Dependências
- Python 3.x
- BeautifulSoup4
- Requests
- re (Regex)
- Pandas
