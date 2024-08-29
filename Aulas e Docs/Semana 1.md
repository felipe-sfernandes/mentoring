P:O que são algoritmos?
R:Informalmente, um algoritmo é qualquer procedimento computacional bem definido que toma algum valor ou
conjunto de valores como entrada e produz algum valor ou conjunto de valores como saída. Portanto, um algoritmo é
uma sequência de etapas computacionais que transformam a entrada na saída.


P: Qual a definição formal de um problema de ordenação?

R: Entrada: Uma sequência de n números 〈a1, a2, ..., an〉.
   Saída: Uma permutação (reordenação) 〈a1’, a2’, ..., an’〉 da sequência de entrada, tal que a1’ ≤ a2’ ≤ ... ≤ an’.


https://www.bigocheatsheet.com/
https://www.cs.usfca.edu/~galles/visualization/ComparisonSort.html

P: O que são algoritmos NP-Completos
R: São algoritmos que não possuem nenhuma solução eficientes, apenas algoritmos bons que utilizando métodos e técnicas conseguimos faze-los viáveis para solucionar o problema determinado.



1. Exemplo real que exija ordenação ou cálculo de uma envoltória convexa
Ordenação: Um exemplo real que exige ordenação é o ranking de sites por motores de busca como o Google. Os sites precisam ser ordenados por relevância com base em algoritmos que consideram diversos fatores, como a qualidade do conteúdo, a quantidade de backlinks, a velocidade do site, entre outros. Ordenar esses resultados é crucial para fornecer aos usuários os links mais relevantes primeiro.

Cálculo de uma envoltória convexa: Um exemplo real que exige o cálculo de uma envoltória convexa é na navegação aérea, onde é necessário determinar o espaço aéreo seguro para evitar colisões entre aviões. A envoltória convexa pode ser usada para calcular a área mínima que encapsula todos os pontos de dados de uma frota de aviões em um radar, ajudando no monitoramento e na gestão do espaço aéreo.

2. Medidas de eficiência em uma configuração real
Além da velocidade, outras medidas de eficiência que poderiam ser usadas incluem:

Uso de memória: Importante para garantir que o algoritmo não consuma mais memória do que o disponível, especialmente em sistemas embarcados ou com recursos limitados.
Eficiência energética: Em dispositivos móveis ou sistemas embarcados, a eficiência energética é crucial para garantir uma longa duração da bateria.
Latência: A rapidez com que um sistema responde a uma solicitação é importante em aplicações em tempo real, como trading de ações ou sistemas de controle industrial.
Escalabilidade: A capacidade de um algoritmo ou sistema de lidar com o aumento da carga de trabalho sem degradação significativa no desempenho.
3. Estrutura de dados: Hash Table
Pontos fortes:

Acesso rápido: As tabelas hash oferecem, em média, tempo constante O(1) para operações de busca, inserção e exclusão, desde que a função hash seja boa e o tratamento de colisões seja eficiente.
Flexibilidade: Pode armazenar diferentes tipos de dados e é usada para implementar outros tipos de estruturas de dados, como conjuntos e mapas.
Limitações:

Colisões: Quando dois elementos diferentes têm o mesmo hash, ocorre uma colisão, o que pode degradar o desempenho para O(n) no pior caso.
Consumo de memória: Pode ser ineficiente em termos de memória se a tabela for muito esparsa, isto é, se a maioria das entradas estiver vazia.
Ordem dos elementos: Não mantém a ordem dos elementos, o que pode ser uma limitação em situações onde a ordenação é necessária.
4. Problemas do caminho mais curto e do caixeiro-viajante
Semelhanças:

Ambos são problemas de otimização que envolvem grafos.
Ambos procuram a melhor rota possível: o caminho mais curto entre dois pontos ou a rota de custo mínimo que visita todos os pontos.
Ambos podem ser resolvidos usando algoritmos de busca em grafos e têm aplicações em logística e redes.
Diferenças:

O problema do caminho mais curto (como o algoritmo de Dijkstra) busca a menor distância entre dois pontos específicos, enquanto o problema do caixeiro-viajante (TSP) busca o menor caminho que passa por todos os pontos e retorna ao ponto inicial.
O problema do caixeiro-viajante é NP-difícil, o que significa que não há solução eficiente conhecida para encontrar a solução ótima para todos os casos; já o problema do caminho mais curto pode ser resolvido em tempo polinomial.
5. Problema que exige a melhor solução vs. solução aproximada
Problema que exige a melhor solução: Planejamento de rotas de emergência em sistemas de navegação para ambulâncias ou bombeiros. É crucial encontrar o caminho mais rápido possível para minimizar o tempo de resposta em situações de emergência.

Problema que basta uma solução “aproximadamente” a melhor: Compressão de imagens. Algoritmos de compressão, como JPEG, não fornecem uma representação perfeita da imagem original, mas uma aproximação que é "boa o suficiente" para a maioria dos propósitos, economizando armazenamento e largura de banda.

P: Qual a diferença entre ordenação por inserção e por intercalação, e qual sua analise assintótica?
R: A ordenação por inserção (Insertion Sort) tem uma complexidade assintótica de O(N²), 
pois no pior caso ela precisa fazer comparações e trocas para cada elemento da lista em relação a todos os elementos já ordenados. 
Já a ordenação por intercalação (Merge Sort) tem uma complexidade assintótica de O(N log N), porque divide a lista em duas partes repetidamente (log N divisões) 
e intercala as partes (N operações de intercalação). Portanto, Merge Sort é geralmente mais eficiente que Insertion Sort para listas grandes devido ao seu menor crescimento de complexidade assintótica.




1. Exemplo de Aplicação que Exige Conteúdo Algorítmico no Nível da Aplicação
Exemplo: Um sistema de recomendação, como o usado pela Netflix para sugerir filmes e séries aos usuários, exige conteúdo algorítmico no nível da aplicação.

Vamos analisar os exercícios 2 e 3 passo a passo, detalhando os cálculos necessários para encontrar os valores de n.

Exercício 2: Comparação entre Ordenação por Inserção e Ordenação por Intercalação

Problema:
Queremos encontrar o valor de n para o qual a ordenação por inserção, que leva 8n² passos, é mais rápida que a ordenação por intercalação, que leva 64n log n passos.

Equação:
Precisamos resolver a inequação:
8n² < 64n log n

Passo 1: Simplificação da Inequação

Divida ambos os lados por 8n (assumindo que n > 0):
n < 8 log n

Essa é a inequação que precisamos resolver. Precisamos encontrar o valor de n onde n < 8 log n.

Passo 2: Teste de Valores para n

Vamos testar diferentes valores de n para verificar quando essa inequação é verdadeira.

- Para n = 1:
  log 1 = 0 (logaritmo na base 2)
  n = 1, 8 log 1 = 8 * 0 = 0 implica 1 < 0 (falso)

- Para n = 2:
  log 2 = 1 (logaritmo na base 2)
  n = 2, 8 log 2 = 8 * 1 = 8 implica 2 < 8 (verdadeiro)

- Para n = 10:
  log 10 ≈ 3.32 (logaritmo na base 2)
  n = 10, 8 log 10 = 8 * 3.32 = 26.56 implica 10 < 26.56 (verdadeiro)

- Para n = 20:
  log 20 ≈ 4.32 (logaritmo na base 2)
  n = 20, 8 log 20 = 8 * 4.32 = 34.56 implica 20 < 34.56 (verdadeiro)

- Para n = 30:
  log 30 ≈ 4.91 (logaritmo na base 2)
  n = 30, 8 log 30 = 8 * 4.91 = 39.28 implica 30 < 39.28 (verdadeiro)

- Para n = 40:
  log 40 ≈ 5.32 (logaritmo na base 2)
  n = 40, 8 log 40 = 8 * 5.32 = 42.56 implica 40 < 42.56 (verdadeiro)

- Para n = 50:
  log 50 ≈ 5.64 (logaritmo na base 2)
  n = 50, 8 log 50 = 8 * 5.64 = 45.12 implica 50 < 45.12 (falso)

Com base nos cálculos acima, vemos que o ponto de transição está entre n = 40 e n = 50.

Passo 3: Identificação do Valor Crítico de n

Para encontrar o valor exato de n onde n = 8 log n, podemos usar métodos numéricos ou gráficos. No entanto, para o propósito deste exemplo, vemos que para n ≈ 43, a ordenação por intercalação começa a ser mais eficiente.

Exercício 3: Comparação de Algoritmos com Complexidades Diferentes

Problema:
Queremos encontrar o menor valor de n tal que um algoritmo com tempo de execução 100n² é mais rápido que um algoritmo com tempo de execução 2^n.

Equação:
Precisamos resolver a inequação:
100n² < 2^n

Passo 1: Teste de Valores para n

Vamos testar diferentes valores de n para verificar quando essa inequação é verdadeira.

- Para n = 1:
  100 * 1² = 100, 2^1 = 2 implica 100 < 2 (falso)

- Para n = 10:
  100 * 10² = 10000, 2^10 = 1024 implica 10000 < 1024 (falso)

- Para n = 15:
  100 * 15² = 22500, 2^15 = 32768 implica 22500 < 32768 (verdadeiro)

- Para n = 20:
  100 * 20² = 40000, 2^20 = 1048576 implica 40000 < 1048576 (verdadeiro)

Com base nos cálculos acima, o menor valor de n para o qual 100n² < 2^n é n = 15.

Esse é o ponto onde o crescimento exponencial de 2^n supera o crescimento quadrático de 100n², fazendo com que o algoritmo com 2^n se torne mais lento em comparação.


| Tempo      | \( \log n \) | \( \sqrt{n} \) | \( n \)      | \( n \log n \) | \( n^2 \)  | \( n^3 \) | \( 2^n \) | \( n! \) |
|------------|--------------|----------------|--------------|----------------|------------|-----------|-----------|----------|
| 1 segundo  | \( 2^{20} \) | \( 10^{12} \)  | \( 10^6 \)   | \( 7 \times 10^4 \) | \( 10^3 \) | \( 100 \)  | \( 20 \)  | \( 9 \)  |
| 1 minuto   | \( 2^{26} \) | \( 4 \times 10^{15} \) | \( 6 \times 10^7 \) | \( 2 \times 10^6 \) | \( 8 \times 10^3 \) | \( 400 \)  | \( 26 \)  | \( 11 \) |
| 1 hora     | \( 2^{32} \) | \( 2 \times 10^{18} \) | \( 3.6 \times 10^9 \) | \( 6 \times 10^7 \) | \( 6 \times 10^4 \) | \( 1500 \) | \( 32 \)  | \( 13 \) |
| 1 dia      | \( 2^{37} \) | \( 1.8 \times 10^{20} \) | \( 8.6 \times 10^{10} \) | \( 1.8 \times 10^8 \) | \( 3 \times 10^5 \) | \( 4600 \) | \( 37 \)  | \( 15 \) |
| 1 mês      | \( 2^{41} \) | \( 1.6 \times 10^{21} \) | \( 2.6 \times 10^{11} \) | \( 5 \times 10^8 \) | \( 8 \times 10^5 \) | \( 1.4 \times 10^4 \) | \( 41 \)  | \( 16 \) |
| 1 ano      | \( 2^{45} \) | \( 1.8 \times 10^{22} \) | \( 3.1 \times 10^{12} \) | \( 6.6 \times 10^9 \) | \( 3.2 \times 10^6 \) | \( 4.6 \times 10^4 \) | \( 45 \)  | \( 17 \) |
| 1 século   | \( 2^{52} \) | \( 1.8 \times 10^{24} \) | \( 3.1 \times 10^{14} \) | \( 2.1 \times 10^{11} \) | \( 1.8 \times 10^7 \) | \( 4.6 \times 10^5 \) | \( 52 \)  | \( 22 \) |

