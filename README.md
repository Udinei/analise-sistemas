# analise-sistemas
Projeto para Anotações sobre analise de sistemas  

# Modelagem de dominio e modelagem conceitual
Domínio: A área de negócio observada
Ex: Padaria, Escola, Farmacia, Hospital etc..  

Domínio: Loja Móveis Angular (Registro de pedidos)  
![](/dominio_nota_fiscal.png)  

Modelo de domínio (Nível Conceitual de negócio)  
- Pode incluir entidades que não são de interesse do sistema  
![](/modelo_dominio_nivel_negocio.png)  

Modelo de domínio (Nível Conceitual de análise)  
- Independente de paradigma  

<b>Ferramenta - Entidade Relacionamento</b>  
![](/nivel_conceitual_de_analise_ferr_entidade_rel_peter_chain.png)  


<b>Ferramenta - Diagrama de classes da UML</b>  
![](/nivel_conceitual_de_analise.png)  

Modelo de domínio (Nível Lógico)
- Preso ao paradigma Relacional
- Forma Textual  
![](/modelo-logico-nivel-relacional-textual.png)  

- Forma Gráfica  
![](/modelo-logico-nivel-relacional-grafico.png) 
 
- Preso ao paradigma Orientado a Objetos  
![](/modelo-uml-nivel-logico.png)  


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

 


