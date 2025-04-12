# Simulação de Monte Carlo com Distribuição t-Student — PETR4

Este projeto implementa uma **simulação de Monte Carlo com distribuição t-Student** para estimar o comportamento futuro do preço das ações da PETR4. O objetivo é avaliar o risco e a incerteza associados ao investimento, considerando cenários de retorno realistas baseados em dados históricos.

---

## Tecnologias utilizadas

- Python 3.10+
- Jupyter Notebook
- `pandas`, `numpy`, `matplotlib`, `scipy`
- `yfinance` (para extração de dados)
- `scipy.stats.t` (para ajuste da distribuição t-Student)

---

## Sobre o Método

### Monte Carlo + t-Student

- Coletamos dados históricos da PETR4.
- Calculamos os **log-retornos** diários.
- Ajustamos uma **distribuição t-Student** aos retornos — útil para capturar caudas mais pesadas (eventos extremos).
- Realizamos **10.000 simulações** de caminhos possíveis para o valor de um investimento de R$ 1.000 ao longo de 252 dias úteis (1 ano).

---

## 📊 Métricas e Visualizações

- Simulações com eixo de tempo real (datas úteis).
- **Estatísticas dos valores finais** (média, mediana, percentis).
- **Value at Risk (VaR)** a 95% de confiança.
- Histogramas, boxplots e múltiplos cenários simulados.

---

## 📁 Estrutura do Projeto

```bash
📦 simulacao-monte-carlo-petr4
├── Simulacao_Monte_Carlo_PETR4.ipynb
├── README.md
