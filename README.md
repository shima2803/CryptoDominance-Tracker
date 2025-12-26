# 📊 CryptoStocksDominance Tracker

---

## 🧠 Sobre o projeto

Durante minhas férias, com um tempo livre a mais (e um pouco de tédio 😅), resolvi estudar APIs de mercado financeiro e criar algo prático.  
Este projeto busca automaticamente dados atualizados de **criptomoedas** e **ações**, gera planilhas em Excel e permite que o **Power BI atualize os gráficos automaticamente** com os valores mais recentes.

Além do aprendizado, fiz este projeto também para **acompanhar melhor meus próprios investimentos** e visualizar dados de forma clara e objetiva.

---

## 🚀 Módulo 1 — Criptomoedas

### O que o módulo de criptomoedas faz

- Busca o **Top 10 criptomoedas por market cap**
- Coleta:
  - Preço atual (USD)
  - Market Cap
  - Variação em 24h
- Calcula a **dominância (%) de cada cripto em relação ao mercado global**
- Gera automaticamente um arquivo **Excel (.xlsx)**
- O **Power BI consome esse arquivo** e atualiza os dashboards com apenas um refresh

---

### 📁 Estrutura da planilha (Cripto)

A planilha é salva na **Área de Trabalho do usuário** com o nome:

top10_cripto_usd.xlsx


Colunas geradas:

- DataColeta
- Rank
- Cripto
- Simbolo
- PrecoUSD
- MarketCapUSD
- DominanciaPct
- Variacao24h

Essa estrutura é ideal para:
- Gráficos
- Cards
- Rankings
- Treemaps
- Séries temporais (caso o projeto evolua)

---

## 📈 Módulo 2 — Ações

Este projeto também conta com um **segundo módulo exclusivo para ações brasileiras**, com um dashboard separado no Power BI e um script Python próprio.

### O que o módulo de ações faz

- Consulta automaticamente ações da B3 (via Yahoo Finance)
- Coleta as principais informações:
  - Preço atual
  - Variação diária (%)
  - Market Cap (valor de mercado)
  - P/L
  - Dividend Yield (%)
  - P/VP
  - Máxima e mínima de 52 semanas
  - Volume negociado
- Classifica cada ativo com uma **heurística de “Oportunidade”**  
  (apenas para fins educacionais, não é recomendação de investimento)
- Gera automaticamente um arquivo **Excel (.xlsx)** atualizado
- O **Power BI consome esse arquivo** e atualiza os gráficos com um clique

---

### 📁 Estrutura da planilha (Ações)

A planilha é salva na **Área de Trabalho do usuário** com o nome:

## ▶️ Como executar
Criptomoedas
python crypto_top10_xlsx.py

Ações
python acoes_top10_powerbi.py


Após a execução:

O arquivo Excel correspondente será atualizado automaticamente

O Power BI poderá ser atualizado com apenas um clique

## 💡 Observações finais

Os projetos foram criados com foco em aprendizado, curiosidade e automação

As análises e classificações são educacionais

O código pode ser facilmente expandido para:

Histórico diário

Alertas automáticos

Dashboards mais avançados

Sinta-se à vontade para adaptar, estudar e evoluir 🚀
