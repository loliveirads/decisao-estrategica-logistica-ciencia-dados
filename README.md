# 📦 Clusterização Geoespacial de Entregas com Falha

Este projeto tem como objetivo realizar uma análise exploratória e segmentação geoespacial (clustering) de pontos de entregas com falha, utilizando técnicas de aprendizado não supervisionado e visualizações interativas para apoiar decisões logísticas.

## 📍 Objetivo

Identificar regiões críticas de falhas de entrega, agrupando-as por proximidade geográfica, com o intuito de:

- Apoiar a definição de locais estratégicos para novos centros de distribuição
- Reduzir custos operacionais e tempo de entrega
- Melhorar o desempenho logístico e experiência do cliente

## 🧠 Técnicas Utilizadas

- Análise Exploratória de Dados (EDA)
- Limpeza e Conversão de Dados Geoespaciais
- Clusterização com KMeans
- Método do Cotovelo (Elbow Method)
- Geocodificação Reversa com `geopy`
- Mapas Interativos com `folium`
- Visualizações com `matplotlib`

## 📂 Estrutura do Projeto

```
atividade_2_clusterizacao/
├── dados/
│   └── Geolocalização Dataset.csv
├── notebooks/
│   └── Clusterizacao_Geoespacial.ipynb
├── mapas/
│   └── mapa_clusters_interativo.html
├── resultados/
│   ├── grafico_entregas.png
│   ├── grafico_valores.png
│   └── centroides_enderecos.txt
├── README.md
└── requirements.txt
```

## ⚙️ Tecnologias

- Python 3.11+
- Pandas
- Scikit-learn
- Matplotlib
- Folium
- Geopy

## 🚀 Como Executar

1. Clone o repositório:
```bash
git clone https://github.com/seuusuario/atividade_2_clusterizacao.git
```

2. Ative o ambiente virtual:
```bash
poetry init
poetry shell
```

3. Instale as dependências com Poetry:
```bash
poetry install
```

4. Execute o notebook:
```bash
jupyter notebook notebooks/decisao-estrategica-logistica-ciencia-dados.ipynb
```

5. Instale o kernel Jupyter para o ambiente Poetry:
```bash
poetry run python -m ipykernel install --user --name=logistica-ds
```

6. Inicie o Jupyter Notebook dentro do ambiente Poetry:
```bash
jupyter notebook
```

7. No Jupyter, selecione o kernel chamado **`logistica-ds`** (ou o nome que você usou no passo 5).

---

## 📊 Resultados

- Identificação de 4 clusters geográficos representando regiões com maior concentração de falhas
- Centroides geográficos convertidos em endereços reais com auxílio da API do OpenStreetMap
- Mapas interativos para visualização da segmentação espacial
- Gráficos limpos e executivos com total de entregas e valor movimentado por cluster
- Relatório com recomendações estratégicas para expansão logística

## ✅ Recomendação Final

Com base na análise cruzada entre volume e valor de entregas, foi possível indicar as regiões prioritárias para novos centros de distribuição, considerando não só a densidade geográfica das falhas, mas também o impacto financeiro envolvido em cada cluster.

## ✍️ Autor

**Luiz Fernando**  
Cientista de Dados em formação  
📧 luizfsoliveira.lm@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/loliveirads) | [GitHub](https://github.com/loliveirads)

## 📝 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).
