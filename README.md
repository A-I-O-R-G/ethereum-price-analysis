# Análise Técnica da Criptomoeda Ethereum 🚀

## 1. 📖 Introdução
Este projeto visa o desenvolvimento de um script para análise técnica da criptomoeda Ethereum, utilizando dados históricos de preços e volumes com o objetivo de prever tendências futuras. As principais funcionalidades incluem a coleta de dados em tempo real, cálculo de indicadores técnicos, visualização gráfica e alerta baseado em condições de mercado.

## 2. ⚙️ Instalação
### Requisitos do Sistema
- Python 3.x
- Dependências: `requests`, `pandas`, `numpy`, `matplotlib`, `sklearn`

### Guia Passo-a-Passo
1. Clone o repositório:
   ```bash
   git clone https://github.com/seuusuario/seurepositorio.git
   cd seurepositorio
   ```
2. Instale as dependências:
   ```bash
   pip install requests pandas numpy matplotlib scikit-learn
   ```

### Configuração Inicial
Certifique-se de que sua conexão com a internet esteja ativa, pois o script coletará dados da API do CoinGecko.

## 3. 🛠️ Uso
### Exemplos Práticos
Para executar a análise, você pode rodar o seguinte comando:
```bash
python seu_script.py
```

### Comandos Principais
- `collect_data()` - Coleta os dados de preços da Ethereum.
- `calculate_indicators(prices)` - Calcula indicadores técnicos como SMA, EMA, RSI e Bandas de Bollinger.
- `visualize_data(df)` - Plota gráficos dos dados e indicadores.
- `check_alerts(df)` - Verifica condições de alerta baseadas nos indicadores.

### Casos de Uso Comuns
- Análise diária dos preços da Ethereum.
- Detecção de tendências de mercado para tomada de decisão.

## 4. 📁 Estrutura do Projeto
```
/análise-tecnica-ethereum
│
├── seu_script.py           # Script principal de análise
├── requirements.txt        # Lista de dependências
└── README.md               # Documentação do projeto
```

## 5. 🌐 API
### Endpoints Disponíveis
- **GET** `https://api.coingecko.com/api/v3/coins/ethereum/market_chart`

### Métodos e Parâmetros
- `vs_currency`: moeda de comparação (ex.: `usd`)
- `days`: número de dias de dados (ex.: `30`)
- `interval`: intervalo de coleta de dados (ex.: `daily`)

### Exemplos de Requisições
```python
response = requests.get(ETHEREUM_API_URL, params=PARAMS)
```

### Respostas Esperadas
A resposta é um JSON contendo os preços da Ethereum.

## 6. 🤝 Contribuição
Se você deseja contribuir para este projeto, siga os seguintes passos:
1. Faça um fork do repositório.
2. Crie uma nova branch (`git checkout -b feature/nova_feature`).
3. Faça suas alterações e confirme-as (`git commit -m 'Adicionando nova feature'`).
4. Envie suas alterações (`git push origin feature/nova_feature`).
5. Crie um Pull Request.

### Padrões de Código
- Use PEP 8 para formatação de código.
- Comentários úteis e documentação são bem-vindos!

## 7. 📜 Licença
Este projeto está sob a licença MIT. Consulte o arquivo [LICENSE](LICENSE) para os termos de uso e restrições.
