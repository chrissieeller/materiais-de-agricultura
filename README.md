# Análise de Dados - Materiais Agrícolas (1990 - 2020)
Criação de relatório em Python (Jupyter Notebook) com base na Sample 'Agricultural Raw Material prices (1990-2020)' disponibilizada por Kaggle. 

## Análise de Dados
<b>1. Etapas:</b><br>
    - Importação de pacotes: Uso de bibliotecas 'numpy' e 'pandas'.<br>
    - Carregamento de dados: O dataset 'agricultural_raw_material.csv' foi carregado.<br>
    - Exploração inicial de dados: Início de análise exploratória.<br>
    - Verificação de dados nulos: Foram identificados dados ausentes.<br>
    - Limpeza de dados: Remoção de caracteres como porcentagem, virgula e hífen, além da substituição de valores anômalos (como 'MAY90') por NaN e eliminação das linhas com dados ausentes.<br>
    - Conversão de dados: Transformação de várias colunas para o tipo 'float' para possibilitar análises numéricas.<br>
<b>2. Correlações e Visualizações</b><br>
    - Matriz de correlação de preços: Visualizada por meio de um heatmap para identificar quais commodities possuem comportamento de preço similar.<br>
    - Matriz de correlação das variações percentuais dos preços: Visualizada por meio de heatmap para entender se as oscilações de preços de uma matéria-prima impactam em outras.<br>
        - Configuração de visualizações: Uso do 'seaborn' e 'matplotlib' para criar gráficos legíveis, com ajustes de tamanho, estilo e fonte dos gráficos.<br>
## Insights
- Produtos derivados de madeira como Hard Log, Softlog, Hard Sawnwood, SOft Sawnwood, Plywood,  Wood Pulp) costumam ter altas correlações entre si, pois pertecem ao mesmo setor. 
- Commodities têxteis (como Cotton, Coarse Wool, Fine wool) provavelmente também apresentam correlação moderada, pois atendem a indústrias semelhantes (tecidos e vestuário).
- Itens agrícolas mais específicos (como Copra e Rubber) podem apresentar correlação mais baixa com madeiras e lãs, refletindo mercados distintos. 
- Commodities que compartilham cadeias produtivas, demandas similares ou estão sujeitas a eventos globais (clima, guerras, políticas comerciais) costumam ter variações semelhantes. 
- Você pode observar que, mesmo que dois produtos não tenham preço absoluto parecido, suas variações podem ser fortemente relacionadas (ou seja, se um sobe, o outro tende a subir também).
- Materiais florestais e derivados costumam oscilar juntos, o mesmo pode ocorrer com produtos agrícolas e têxteis.  
- Produtos muito específicos podem não seguir esses padrões (por exemplo, Rubber pode ser mais afetado pela indústria automotiva, enquanto Copra responde a mercados de alimentos e cosméticos).
## Recomendações
- Para investidores: Focar na diversificação entre setores (florestal, agrícola e têxtil) para reduzir riscos de eventos sistemicos.
- Para produtores e fornecedores: Monitorar commodities correlacionadas para antecipar movimentos de mercado. 
- Para analistas econômicos: Utilizar essas correlações como base para construir modelos de previsão de preços e estratégias de mitigação de risco.
