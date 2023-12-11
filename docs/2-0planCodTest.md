# Plano de Codificação e Testes

No contexto do desenvolvimento de software, adotaremos uma abordagem de modelagem funcional, combinando os paradigmas de programação funcional e orientada a objetos. Optaremos pela linguagem Python devido à sua adequação para o desenvolvimento ágil de aplicações de pequena escala com interface de linha de comando.

Para a implementação do código, seguiremos o "REPL-driven development", empregando o ambiente de desenvolvimento integrado Jupyter Lab para facilitar esse método iterativo.

Posteriormente, após a fase inicial de codificação usando o RDD, nos dedicaremos à criação de testes unitários automatizados utilizando a ferramenta pytest. Essa abordagem visa proporcionar uma camada adicional de segurança e garantir a correção do código desenvolvido.

No que diz respeito à representação de pontos em um sistema de coordenadas cartesianas, essenciais para a posterior plotagem de gráficos de funções, faremos uso da biblioteca NumPy em Python. Além disso, para a visualização gráfica dos resultados, empregaremos a biblioteca Matplotlib.

Esse conjunto de práticas visa promover um desenvolvimento eficiente, iterativo e seguro, com ênfase na qualidade do código e na facilidade de manutenção.

## Módulo entrada/saida - es.py

### 1. Requisito 1b

Plotar o gráfico

função impressora(grafico: objeto gráfico) -> null
Esta função imprime na tela o gráfico da função escolhida pelo usuário.

### 2. Requisito 2

Deve haver um menu com as quatro funções capazes de serem plotadas pelo aplicativo.

função leitor_funcao() -> string
Imprime um menu na tela contendo as funções afim, quadrática, logarítmica e exponencial para o usuário escolher qual delas plotar.

### 3. Requisitos 3 e 4

 Caso o usuário escolha a função afim, na sequência, ele deverá poder informar os coeficientes da função.

- Idêntico ao requisito 2, mas sendo válido para função quadrática.

função leitor_coeficiente(nome_funcao: string) -> lista
Lê os coeficientes no caso de o usuário escolher plotar uma função afim ou quadrática.

## Módulo de processamento de gráficos (designer)

Este módulo deverá prover uma função para plotar o gráfico da função escolhida pelo usuário.

### 1. Requisito 1a

Determinar o gráfico

função design(tipo_funcao: str, coeficientes: lista) -> objeto gráfico
Esta função recebe o tipo de função a ser desenhada e a lista de coeficientes (se for necessário) e desenha o gráfico da função correspondente.
