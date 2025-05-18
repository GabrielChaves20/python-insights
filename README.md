# 📊 Análise de Cancelamentos de Clientes

Este projeto visa identificar os principais motivos que levam ao cancelamento de clientes de uma empresa com mais de 800 mil clientes, utilizando análise de dados com Python e visualizações com Plotly.

## 🔍 Objetivo

A empresa observou que uma grande parte de sua base de clientes já cancelou o serviço. O objetivo deste projeto é analisar os dados disponíveis e identificar padrões de comportamento que levam ao cancelamento, a fim de propor ações que reduzam esse número.

---

## 📁 Estrutura do Projeto

* [Dados de Cancelamento](https://drive.google.com/drive/folders/1fRHCEY0liArTvsUogBiewE-8CdvLx1zV?usp=drive_link) – Link para a base de dados com informações dos clientes.
* `insights.ipynb` – Código Python com a análise exploratória e limpeza dos dados.
* `graficos` - Pasta com os gráficos gerados pelo Plotly
**Importante ressaltar que a base foi simplificada para subir o projeto ao github, mas na pasta do drive você pode encontrar a base completa**

---

## 🧪 Etapas da Análise

1. **Carregamento dos dados** com Pandas.
2. **Limpeza da base**, como:

   * Remoção da coluna `CustomerID`, irrelevante para a análise.
   * Exclusão de linhas com valores nulos.
3. **Análise da variável alvo** `cancelou` para entender a proporção de cancelamentos.
4. **Análise de contrato e assinatura**, observando:

   * Clientes com contrato mensal tendem a cancelar mais.
   * Clientes com contratos mais longos cancelam menos.
5. **Visualização de variáveis** com `Plotly Express`, colorindo por cancelamento.
6. **Aplicação de filtros com base em padrões identificados**:

   * Clientes com **mais de 4 ligações** ao call center tendem a cancelar.
   * Clientes **com idade superior a 50 anos** cancelam.
   * Clientes com **mais de 20 dias de atraso** no pagamento cancelam.

---

## 📉 Resultados

Após aplicar os filtros:

* A taxa de cancelamento reduziu drasticamente na base.
* Fatores mais fortes de cancelamento:

  * Alta insatisfação (número alto de ligações ao suporte).
  * Idade elevada (clientes acima de 50 anos).
  * Inadimplência (atrasos prolongados no pagamento).
  * Contrato mensal.

---

## ✅ Conclusões e Recomendações

Com base nas análises, as seguintes ações são recomendadas:

* Melhorar o atendimento ao cliente e reduzir o número de ligações recorrentes.
* Oferecer suporte personalizado para clientes mais velhos.
* Implementar políticas de lembrete e incentivo para pagamentos em dia.
* Incentivar contratos mais longos com benefícios atrativos.

---

## 🚀 Tecnologias Utilizadas

* Python
* Pandas
* Plotly
* Jupyter Notebook

---

## 📌 Como Usar

1. Clone o repositório:

   ```bash
   git clone https://github.com/GabrielChaves20/python-insights
   ```
2. Instale as dependências:

   ```bash
   pip install pandas plotly
   ```
3. Faça o download da planilha utilizando o link que está na seção **Estrutura do Projeto**, neste arquivo Readme. Importante deixá-la na mesma pasta que está o arquivo `insights.ipynb`.
4. Execute o notebook ou o script Python para visualizar os resultados.

---

## 👨‍💻 Autor

**Gabriel Chaves**  
📧 gabrielbsc0720@gmail.com  
🔗 [LinkedIn](www.linkedin.com/in/gabriel-borges-ch)

---

Este projeto está licenciado sob a **MIT License**.
