# ARTIGO
Arquivos e códigos dos resultados obtidos pela pesquisa de postos de carregamento na cidade de São Carlos e resultados do banco de dados OR-Library


Este artigo propõe um algoritmo baseado na metaheurística Variable Neighborhood Descent (VND) para a solução dos problemas de p-medianas capacitado e não capacitado. A solução inicial foi construída com base em uma heurística gulosa.
Além disso, foi realizado um estudo para a localização de postos de carregamento de veículos elétricos na cidade de São Carlos, bem como experimentos computacionais com 60 instâncias da literatura, cujos resultados foram comparados aos obtidos pelo modelo matemático resolvido por um método exato, utilizando o solver Gurobi.

Para o estudo aplicado do problema de localização de facilidades, escolheu-se o município de São Carlos - SP, a localização dos postos de carregamento já instalados foi definida com base nos postos classificados em (PlugShare, 2025), um site que funciona como um mapa de estações de carregamento para veículos elétricos, cujas coordenadas geográficas estão disponíveis na pasta dados_csv. Além disso, para a definição dos postos candidatos, foram consideradas 10 regiões de grande circulação na cidade, selecionadas de forma a abranger a maior área possível do município. Suas coordenadas estão definidas em dados_csv. Para a seleção dos 25 clientes, suas coordenadas foram escolhidas aleatoriamente na região de São Carlos de maneira a cobrir a maior região possível do município, como pode ser visto na pasta dados_csv. Todos os arquivos e códigos desse problema real estão armazenados na pasta Caso Real - São Carlos


Para a validação do algoritmo estudado nesse artigo, foi utilizada uma base da literatura, a biblioteca OR-Library, referente ao problema de $p$-mediana não capacitada e capacitada. 
Para os problemas não capacitados, os métodos propostos foram testados em 40 instâncias. Os arquivos estão no formato .txt, com diferentes níveis de complexidade. As instâncias variam de 100 a 900 nós (clientes ou centros de demanda), e de 5 a 200 medianas. 
Cada instância fornece dados sobre as distâncias entre os vértices, porém em alguns arquivos essas informações não estão completas. Diante disso, seguindo a recomendação no próprio site OR-Library, utilizou-se um algoritmo de Floyd-Warshall, código disponível no arquivo .ipynb, para a construção da matriz de distâncias completa das instâncias do banco de dados utilizado, pois calcula o menor caminho entre todos os pares de nós de uma rede.
Já os problemas capacitados foram avaliados em um conjunto de 20 instâncias, também da biblioteca OR-Library, cujo o número de medianas varia de 5 a 10, contando com problemas de 50 a 100 nós.
