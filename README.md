# Artigo
Arquivos e códigos dos resultados obtidos pela pesquisa de postos de carregamento na cidade de São Carlos e resultados do banco de dados OR-Library


Este artigo propõe um algoritmo baseado na metaheurística Variable Neighborhood Descent (VND) para a solução dos problemas de p-medianas capacitado e não capacitado. A solução inicial foi construída com base em uma heurística gulosa.
Além disso, foi realizado um estudo para a localização de postos de carregamento de veículos elétricos na cidade de São Carlos, bem como experimentos computacionais com 60 instâncias da literatura, cujos resultados foram comparados aos obtidos pelo modelo matemático resolvido por um método exato, utilizando o solver Gurobi.

Para o estudo aplicado do problema de localização de facilidades, escolheu-se o município de São Carlos - SP, a localização dos postos de carregamento já instalados foi definida com base nos postos classificados em (PlugShare, 2025), um site que funciona como um mapa de estações de carregamento para veículos elétricos, cujas coordenadas geográficas estão disponíveis na pasta dados_csv. Além disso, para a definição dos postos candidatos, foram consideradas 10 regiões de grande circulação na cidade, selecionadas de forma a abranger a maior área possível do município. Suas coordenadas estão definidas em (continuar...). Para a seleção dos 25 clientes, suas coordenadas foram escolhidas aleatoriamente na região de São Carlos de maneira a cobrir a maior região possível do município, como pode ser visto
