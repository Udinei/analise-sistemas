# analise-sistemas
Projeto para Anotações sobre analise de sistemas  

# Modelagem de dominio e Modelagem conceitual
**Domínio:** A área de negócio observada  
Ex: Padaria, Escola, Farmacia, Hospital etc..  

### Possui quatro níveis de abstração 
 
- **Negócio**  - Analista de negócio - Descreve entidade do domínio **do negócio** e suas inter-relações
  **Independente de Sistema**  
 
- **Sistema**  - Analista de Sistema - Descreve entidade do domínio **do sistema** e suas inter-relações
  **Independente de Paradigma e tecnologia**
 
- **Lógico**  - Projetista - Descreve entidade  do domínio **do sistema** e suas inter-relações 
  **Preso ao Paradigma e tecnologia (Relacional, OO) - Independente de tecnologia**  
 
- **Físico** - Implementador - Descreve entidade  do domínio **do sistema** e suas inter-relações 
  **Preso ao Paradigma (Relacional, OO) - Preso a tecnologia (Java, C#, PHP, etc..)**  
 
**Domínio:** Nota Fiscal (Registros do Pedido)  
![](/dominio_nota_fiscal.png)  

### Modelo de domínio (Nível Conceitual de negócio)  
- Independente de paradigma  
- Pode incluir entidades que não são de interesse do sistema  
![](/modelo_dominio_nivel_negocio.png)  

### Modelo de domínio (Nível Conceitual de análise)  
- Independente de paradigma  

<b>Ferramenta - Entidade Relacionamento</b>  
![](/nivel_conceitual_de_analise_ferr_entidade_rel_peter_chain.png)  

<b>Ferramenta - Diagrama de classes da UML</b>  
![](/nivel_conceitual_de_analise.png)  

### Modelo de domínio (Nível Lógico)
- Preso ao paradigma Relacional
- Forma Textual  
![](/modelo-logico-nivel-relacional-textual.png)  

- Forma Gráfica  
![](/modelo-logico-nivel-relacional-grafico.png) 
 
- Preso ao paradigma Orientado a Objetos  
  Pode ser implementado em qualquer linguagem  
![](/modelo-uml-nivel-logico.png)  

### Nível Físico ou de Implementação  
- Preso ao paradigma Relacional - BD  
- Preso a tecnologia (ex: Mysql - dialeto SQL)  
![](/modelo-dominio-nivel-fisico-msql.png)

- Preso ao paradigma Orientado a Objetos - Classes  
- Preso a tecnologia (ex: Java - OO)  
 ![](/impl-classes-dominio-java.png)


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
  - Levantamento de informações do negócio    
- Elaboration
  - Arquitetura e principais decisões  
- Construction 
  - Desenvolvimento e testes  
- Transition
  - Implantação  


# Modelo de domínio
Domíno: É a área de negócio observada

Modelo de domínio: Modelo que descreve 
• As entidades do domínio
• E as inter-relações entre essas entidades

### Níveis de Abstração do modelo de domínio 
Quanto mais alto for o nível de abstração menos detalhes do sistema serão exibidos.

| Nível  | Responsável  | Objetivo   | 
|---	   |---         	|---         |
|Conceitual ou de Análise (de negócio) |Analista de negócio | Descrever as entidades do domínio (do negócio) e suas inter-relações: Independentemente de SISTEMA |
|Conceitual ou de
Análise (de sistema) | Analista de sistemas | Descrever as entidades do domínio (do sistema) e suas inter-relações: •Independentemente de PARADIGMA E TECNOLOGIA |
| Lógico ou de Design  | Projetista | Descrever as entidades do domínio (do sistema) e suas inter-relações: • Preso a um PARADIGMA (ex: relacional, orientado a objetos) • Independentemente de TECNOLOGIA  |
| Físico ou de
implementação | Implementador | Descrever as entidades do domínio (do sistema) e suas inter-relações:• Preso a um PARADIGMA (ex: relacional, orientado a objetos) • Preso a uma TECNOLOGIA (ex: Java, C#, PHP, Python, Ruby, NodeJS) |


## Modelo Conceitual
O modelo conceitual descreve:
- Conceitos
- Atributos
- Associações

<b>Definição 1:</b> Modelo que descreve a estrutura das informações que o sistema vai gerenciar (Wazlwick)
<b>Definição 2:</b> Modelo de dominío em nível de Análise
- Pertence ao escopo do problema e não do escopo da solução
- Independente de paradigma
- Independente de tecnologia
 
## Conceitos
- Algo que tenha significado para o negócio e necessidade de armazenamento
- Unidade coesa do negócio

## Atributos
- Informações alfanuméricas simples
- Não pode  multivalorado(1FN)
- Não pode ser composto(1FN)

## Representação UML de conceitos e atributos
Para representar o Modelo Conceitural vamos utilizar a ferramenta
- Diagrama de classes da UML
  
![](/representacao_conceitos_UML.png)
- nome : tipo 
  "- codPedido : Integer"
  
- atributo identificador 
    " - << >>" simbolo de esteriótipo com a palavra "oid' no seu interior, como na imagem
 
- Valor inicial 
   "- desconto : Double = 0"
 
- Atributo derivado
   "- / valorLiquido : Double = valorBruto - desconto"

 ## Polêmica sobre análise e Design
 <b>Análise:<\b> Descrever o PROBLEMA (Independente de paradigma e tecnologia)
 <b>Desing:<\b> Descrever a SOLUÇÃO (Preso ao paradigma)

  <b>No paradigma estruturaedo/relacional tinha que definir<\b>    
  - Chave estrangeiras
  - Criação de tabela
  - Normalização
  - Outro...  
  
  <b>No paradigma OO usando UML<\b>
   - O modelo conceitual de análise é praticamente o modelo de design
     diferenciando somente a inclusão de metodos no modelo de design 
      O modelagem conceitual em nivel de analise na OO, "invade" alguns aspectos de Design(normalização, tipos de dados, direção de associações, 
      etc...) por isso a polêmica das disciplinas estarem juntas na definição do processo unificado. 
      
     Conclusão: Análise e desingn tendem a ser mais próximas no desenvolvimento OO.
