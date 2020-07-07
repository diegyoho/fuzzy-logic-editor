<div align="center">

# Fuzzy Logic Editor

<div>
  
  Editor de Lógica Fuzzy para Unity.

</div>

</div>

## 📑 Indíce

- [📜 Sobre](#-sobre)
- [💻 Tecnologias](#-tecnologias)
- [⚠️ Instalação](#%EF%B8%8F-instalação)
- [📖 Documentação](#-documentação)

## 📜 Sobre

Fuzzy Logic Editor é uma extensão para Unity que permite utilizar Lógica Fuzzy em seus projetos com o mínimo de codificação. Sua pricinpal funcionalidade e a definição de variáveis linguísticas e das regras que controlam o sistema de inferência fuzzy em uma interface visual. A extensão foi implementada utilizando a biblioteca [AForge.Net Framework](http://www.aforgenet.com/framework/).

## 💻 Tecnologias

- C#
- Unity ([2019.1.0f2](https://unity3d.com/pt/get-unity/download/archive?_ga=2.221850136.1401528206.1594129729-407876505.1594129729))
- [AForge.Net Framework](http://www.aforgenet.com/framework/)

## ⚠️ Instalação

Baixe o pacote [fuzzy-logic-editor.unitypackage](https://github.com/chicodiegomoreira/fuzzylogiceditor/raw/master/fuzzy-logic-editor.unitypackage).

No seu projeto Unity, vá em:

    Assets -> Import Package -> Custom Package

![](/images/importpackage.png)

Após abrir o pacote, selecione tudo e clique em: "Import".

![](/images/importpackage2.png)


## 📖 Documentação

- [Editor Visual](#-editor-visual)
- [FIS](#-fis-fuzzy-inference-system)

### Editor Visual

    Fuzzy Logic -> Fuzzy Logic Editor
    
Contém duas abas:
- [Fuzzy Sets](#-fuzzy-sets)
- [Rules](#-rules)

#### Fuzzy Sets 

Interface de definição de variáveis linguísticas e conjuntos fuzzy.

![](/images/logicfuzzyeditor.png)

#### Rules

Interface de definição das regras do sistema de inferência.

![](/images/logicfuzzyeditor-rules.png)

### FIS: Fuzzy Inference System

A classe FIS (Fuzzy Inference System) possui funções que facilicitam o processo de Fuzzificação (inserção de valores no sistema) e Defuzzificação (obtenção dos resultados da inferencia).

- FIS.Initialize(): Carrega as configurações do Sistema Fuzzy.

- FIS.SetInput(variableName, value): Define uma entrada numérica para uma das variáveis linguísticas.

- FIS.Evaluate(variableName): Obtém uma saída numérica para uma variável lingüística de saída escolhida.
