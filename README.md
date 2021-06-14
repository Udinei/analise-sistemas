# analise-sistemas
Projeto para Anotações sobre analise de sistemas

# Modelagem de dominio e modelagem conceitual

## Disciplinas (Variação do RUP)
- Bussines modelling* 
- Requirements*
- Analysis & Design*
- Implemetation
- Test
- Deployment
- Configuration & Change Management
- Project Management
- Enviroment

*Disciplina da Modelagem de Dominio

## Fases
- Incepiton 
- Elaboration
- Construction 
- Transition


# Modelo de domínio
Domíno: É a área de negócio observada

Modelo de domínio: é um modelo que descreve
• As entidades do domínio
• As inter-relações entre elas

### Níveis de Abstração do modelo de domínio 
| Nível  | Responsável  | Objetivo   | 
|---	   |---         	|---         |
|Conceitual ou de Análise (de negócio) |Analista de negócio | Descrever as entidades do domínio (do negócio) e suas inter-relações: Independentemente de SISTEMA |
|Conceitual ou de
Análise (de sistema) | Analista de sistemas | Descrever as entidades do domínio (do sistema) e suas inter-relações: •Independentemente de PARADIGMA E TECNOLOGIA |
| Lógico ou de Design  | Projetista | Descrever as entidades do domínio (do sistema) e suas inter-relações: • Preso a um PARADIGMA (ex: relacional, orientado a objetos) • Independentemente de TECNOLOGIA  |
| Físico ou de
implementação | Implementador | Descrever as entidades do domínio (do sistema) e suas inter-relações:• Preso a um PARADIGMA (ex: relacional, orientado a objetos) • Preso a uma TECNOLOGIA (ex: Java, C#, PHP, Python, Ruby, NodeJS) |


## Modelo Conceitual
<b>Definição 1:</b> Modelo que descreve a estrutura das informações que o sistema vai gerenciar (Wazlwick)
<b>Definição 2:</b> Modelo de dominío em nível de Análise
- Pertence ao escopo do problema e não do escopo da solução
- Independente de tecnologia
 
## Conceitos
- Algo que tenha significado pra o negócio e necessidade de armazenamento
- unidade coesa do negócio

## Atributos
- Informações alfanuméricas simples
- não pode  multivalorado(1FN)
- não pode ser composto(1FN)

## Representaçãp de conceitos e atributos com diagrama de classes da UML
![](/representacao_conceitos_UML.png)
- nome : tipo 
- atributo identificador
- Valor inicial
- Atributo derivado



- Independente de paradigma
- 


