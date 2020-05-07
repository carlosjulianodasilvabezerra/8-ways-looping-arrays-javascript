
                                         # 8 Formas de usar Looping em Arrays no JavaScript 

# For 
  A instrução for cria um loop que consiste em três expressões opcionais, dentro de parênteses e separadas por ponto e vírgula, seguidas por uma declaração ou uma sequência de declarações executadas em sequência.
## Syntax
  - for ([inicialização]; [condição]; [expressão final])
  - declaração

# While
  A declaração while cria um laço que executa uma rotina especifica enquanto a condição de teste for avaliada como verdadeira. A condição é avaliada antes da execução da rotina.
## Syntax
  while (condição) {
    rotina
  }

# ForEach
  O forEach executa o callback fornecido uma vez para cada elemento da ordem com um valor atribuido. Ele não é invocado para propriedades de índices que foram deletados ou que não foram inicializados (por ex. em arrays esparsos).

  Obs: O seu return é sempre undefined

# Map
  O método map() invoca a função callback passada por argumento para cada elemento do Array e devolve um novo Array como resultado.

## Sintaxe
  arr.map(callback[, thisArg])

# Filter
  O método filter() cria um novo array com todos os elementos que passaram no teste implementado pela função fornecida.

## Sintaxe
var newArray = array.filter(callback[, thisArg])


callback é invocado com três argumentos:
- o valor do elemento
- o índice do elemento
- o array que está sendo percorrido


# Reduce
  O método reduce() executa uma função redutor (fornecida por você) para cada elemento do array, resultando num único valor de retorno.

  ## A função reducer é alimentada por quatro parâmetros:

  - Acumulador
  - Valor Atual
  - Index Atual
  - Array original

  O valor de retorno da sua função reducer é atribuída ao acumulador. O acumulador, com seu valor atualizado, é repassado para cada iteração subsequente pelo array, que por fim, se tornará o valor resultante, único, final.

  ## Sintaxe
  array.reduce(callback( acumulador, valorAtual[, index[, array]] )[, valorInicial]))

  ## parâmetros
  ### callback
  Função que é executada em cada valor no array (exceto no primeiro, se nenhum valorInicial for passado); recebe quatro argumentos:
  ### acumulador
  O valor retornado na última invocação do callback, ou o argumento valorInicial, se fornecido (exemplo abaixo).
  ### valorAtual
  O elemento atual que está sendo processado no array.
  ### index
  Opcional. O índice do elemento atual que está sendo processado no array.
  ### array
  Opcional. O array ao qual a função reduce() foi chamada.
  #### valorInicial
  Opcional. Valor a ser usado como o primeiro argumento da primeira chamada da função callback. Se nenhum valorInicial é fornecido, o primeiro elemento do array será usado como o valor inicial do acumulador e o valorAtual não será lido. Chamar reduce() em uma array vazia sem valor inicial retornará um erro.

# Every  
  O método every() testa se todos os elementos do array passam pelo teste implementado pela função fornecida.

  ## Sintaxe
  arr.every(callback[, thisArg])

  ## Valor de retorno
  true se a função de callback retorna um valor truthy para cada um dos elementos do array; caso contrário, false.

# Some
O método some() testa se algum dos elementos no array passam no teste implementado pela função atribuída.

## Sintaxe
arr.some(callback[, thisArg])

some() executa a função callback uma vez para cada elemento presente no array até achar um onde o callback retorne um valor true. Se em qualquer dos elementos o valor for encontrado, some() imediatamente retorna true. Caso contrario, some() retorna false.
