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

## Exemplo

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
              Bitcoin	 Ethereum	 Tether BNB	 Solana    USDC      XRP     Dogecoin Toncoin	  Cardano
Preço        R$220,000  R$80,000  R$40,000  R$50,000 R$70,000  R$30,000 R$20,000 R$10,000   R$20,000 R$10,000          
...
```

## Dependências
- Python 3.x
- BeautifulSoup4
- Requests
- re (Regex)
- Pandas
