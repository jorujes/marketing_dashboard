# 📊 Marketing Analytics Dashboard

Um dashboard interativo e completo para análise de campanhas de marketing com múltiplas visualizações avançadas.

## 🚀 Características

### 📈 Visualizações Implementadas

1. **KPIs Principais**
   - Faturamento Total
   - Investimento Total
   - ROI Médio
   - Total de Leads
   - Custo Médio por Lead

2. **Visão Geral**
   - **Treemap**: Faturamento por campanha com cores indicando ROI
   - **Sunburst**: Distribuição hierárquica de leads
   - **Waterfall**: Análise de margem (contribuição de cada campanha)

3. **Análise de Campanhas**
   - **Top 10 Campanhas**: Ranking por faturamento
   - **Bubble Chart 3D**: Investimento vs Faturamento vs Quantidade de Leads
   - **Heatmap**: Mapa de calor do ROI por campanha

4. **Análise de Leads**
   - **Funil de Conversão**: Do total de leads até conversão
   - **Gauge Charts**: Medidores de temperatura dos leads (🥶😐🥵)
   - **Sankey Diagram**: Fluxo de leads entre temperaturas e probabilidades

5. **Análise Financeira**
   - **Scatter Plot com Regressão**: Correlação investimento vs faturamento
   - **Box Plot**: Distribuição estatística das margens
   - **Gráfico de Pareto**: Princípio 80/20

6. **Análises Avançadas**
   - **Radar Chart**: Comparação multidimensional das top 5 campanhas
   - **Chord Diagram**: Relações entre temperatura e probabilidade
   - **Network Graph**: Rede de campanhas por performance

## 🛠️ Como Usar

### Opção 1: Abrir Diretamente
1. Simplesmente abra o arquivo `index.html` em seu navegador
2. O dashboard tentará carregar automaticamente o arquivo CSV da pasta anterior
3. Se não encontrar, use o botão para fazer upload manual

### Opção 2: Servidor Local (Recomendado)
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js
npx serve
```

Depois acesse: `http://localhost:8000`

## 📁 Estrutura de Dados

O CSV deve conter as seguintes colunas:
- Campanhas
- Investimento
- Faturamento
- Margem
- No. de Leads
- Custo por lead
- Leads 🥶, 😐, 🥵 (e suas porcentagens)
- Pouco Provável, Possível, Muito Provável (e suas porcentagens)

## 🎨 Tecnologias Utilizadas

- **Chart.js**: Gráficos básicos e avançados
- **Plotly.js**: Visualizações complexas (Sankey, Chord)
- **D3.js**: Manipulação de dados e visualizações customizadas
- **Bootstrap 5**: Interface responsiva
- **Papa Parse**: Processamento de CSV

## 🔧 Personalização

### Cores
As cores principais podem ser alteradas no CSS através das variáveis:
```css
:root {
    --primary: #6366f1;
    --success: #10b981;
    --danger: #ef4444;
    --warning: #f59e0b;
}
```

### Adicionar Novas Visualizações
1. Adicione um container HTML na aba desejada
2. Crie uma função `createNewChart()` no JavaScript
3. Chame a função em `updateAllVisualizations()`

## 📊 Próximas Visualizações Planejadas

- **Word Cloud**: Nuvem de palavras das campanhas
- **Timeline**: Evolução temporal (quando houver datas)
- **Mapa Geográfico**: Performance por região
- **Análise Preditiva**: Previsões com Machine Learning
- **Dashboard Mobile**: Versão otimizada para dispositivos móveis

## 🐛 Solução de Problemas

### O arquivo CSV não carrega
- Verifique se o caminho está correto
- Use o upload manual através do botão
- Certifique-se de que o CSV está no formato correto

### Gráficos não aparecem
- Abra o console do navegador (F12) para ver erros
- Verifique se todos os dados numéricos estão formatados corretamente
- Tente recarregar a página

## 📝 Licença

Este projeto é livre para uso pessoal e comercial.

## 🤝 Contribuições

Sinta-se à vontade para adicionar novas visualizações ou melhorar as existentes!
