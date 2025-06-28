# Duration
Este projeto em Python realiza o cálculo completo da Duration Macaulay e da Duration Modificada de um título com pagamentos periódicos (cupom), utilizando técnicas de valor presente e fator de desconto. O resultado é estruturado em um DataFrame pandas e exportado para um arquivo Excel .xlsx
# 📊 Cálculo da Duration de um Título de Renda Fixa

Este projeto em Python calcula a **Duration Macaulay** e a **Duration Modificada** de um título de renda fixa com pagamentos periódicos de cupom. Ele utiliza fluxos de caixa futuros, aplica descontos com taxa de juros composta e organiza todos os resultados em um DataFrame, que pode ser exportado para Excel para facilitar a análise.

## 🔍 O que o projeto faz

- Gera o fluxo de caixa de um título com base no valor nominal, taxa de cupom e período.
- Calcula o fator de desconto de cada ano usando taxa de juros composta.
- Apura o valor presente de cada fluxo (VP).
- Determina o peso percentual de cada fluxo em relação ao valor presente total.
- Calcula:
  - 📏 **Duration Macaulay**: média ponderada dos prazos pelo valor presente.
  - 🔁 **Duration Modificada**: sensibilidade do preço ao juro.
- Organiza tudo em um `DataFrame` e salva como arquivo `.xlsx`.

## 📂 Estrutura da Saída

| Ano | Fluxo de Caixa | Fator de Desconto | Valor Presente | Proporção VP | Peso VP x Tempo |
|-----|----------------|-------------------|----------------|--------------|------------------|
| ... | ...            | ...               | ...            | ...          | ...              |

## 🛠️ Tecnologias usadas

- Python 3.x
- pandas
- datetime

## 🧾 Como usar

1. Clone este repositório
2. Execute o script `duration.py` (ou equivalente)
3. O arquivo `fluxo_de_caixa.xlsx` será gerado com os resultados organizados

## 📈 Possíveis extensões

- Integração com dados reais via API ou planilhas
- Cálculo mensal ou contínuo de duration
- Geração de gráficos com `matplotlib` ou `plotly`

## 📄 Licença

Este projeto está licenciado sob os termos da [MIT License](LICENSE).

