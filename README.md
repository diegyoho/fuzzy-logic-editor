# Fuzzy Logic Editor

> Editor de Lógica Fuzzy para Unity.

Fuzzy Logic Editor é uma extensão para Unity que permite utilizar Lógica Fuzzy em seus projetos com o mínimo de codificação. Sua pricinpal funcionalidade e a definição de variáveis linguísticas e das regras que controlam o sistema de inferência fuzzy em uma interface visual. A extensão foi implementada utilizando a biblioteca [AForge.Net Framework](http://www.aforgenet.com/framework/).

## Instalação
Baixe o pacote fuzzy-logic-editor.unitypackage.

No seu projeto Unity, vá em: Assets > Import Package > Custom Package, e selecione o arquivo.
![](https://github.com/chicodiegomoreira/fuzzylogiceditor/blob/master/images/importpackage.png)
![](https://github.com/chicodiegomoreira/fuzzylogiceditor/blob/master/images/importpackage2.png)


## Utilização

### Editor Visual

O Editor Visual fica em Fuzzy Logic > Fuzzy Logic Editor. Ele contém duas abas: Fuzzy Sets e Rules.

Fuzzy Sets é a interface de definição de variáveis linguísticas e conjuntos fuzzy.
![](https://github.com/chicodiegomoreira/fuzzylogiceditor/blob/master/images/logicfuzzyeditor.png)

Rules é a interface de definição das regras do sistema de inferência.
![](https://github.com/chicodiegomoreira/fuzzylogiceditor/blob/master/images/logicfuzzyeditor-rules.png)

### FIS: Fuzzy Inference System

A classe estática FIS (Fuzzy Inference System) possui funções que facilicitam o processo de Fuzzificação (inserção de valores no sistema) e Defuzzificação (obtenção dos resultados da inferencia).

* FIS.SetInput(variableName, value): Define uma entrada numérica para uma das variáveis linguísticas.

* FIS.Evaluate(variableName): Obtém uma saída numérica para uma variável lingüística de saída escolhida.
