# Exercícios de Revisão - Semana 10

## Introdução

Esta atividade tem como objetivo revisar os principais diagramas UML estudados durante a disciplina, aplicando-os em diferentes cenários propostos pelo professor.

Cada cenário foi modelado utilizando o tipo de diagrama mais adequado, considerando o comportamento esperado do sistema e as interações entre seus atores.

---

# Cenário 1 – Logística de E-commerce Global

## Diagrama de Casos de Uso

O sistema é responsável pelo gerenciamento do despacho de mercadorias. Para realizar essa atividade, consulta o estoque interno, verifica o status da transportadora e envia os dados necessários para a Receita Federal emitir a nota fiscal.

```mermaid
flowchart LR

Cliente([Operador Logístico])

Sistema((Sistema de Despacho))

Estoque[(Estoque Interno)]
Transportadora[(Transportadora)]
Receita[(Receita Federal)]

UC1([Consultar Estoque])
UC2([Consultar Status da Transportadora])
UC3([Gerenciar Despacho])
UC4([Emitir Nota Fiscal])

Cliente --> UC3

UC3 --> UC1
UC3 --> UC2
UC3 --> UC4

UC1 --> Estoque
UC2 --> Transportadora
UC4 --> Receita
```

### Explicação

O diagrama evidencia a fronteira do sistema e mostra as integrações com sistemas externos, como Estoque, Transportadora e Receita Federal.
---

# Cenário 2 – Totem de Autoatendimento em Fast-Food

## Diagrama de Casos de Uso

Neste cenário, o cliente realiza seu pedido diretamente no totem e efetua o pagamento via cartão ou PIX. Após a confirmação do pagamento, o pedido é enviado para a cozinha e os pontos de fidelidade do cliente são atualizados.

```mermaid
flowchart LR

Cliente([Cliente])
Cozinheiro([Cozinheiro])

Pagamento[(Sistema de Pagamento<br/>PIX/Cartão)]
Fidelidade[(Sistema de Fidelidade)]

UC1([Realizar Pedido])
UC2([Efetuar Pagamento])
UC3([Enviar Pedido para Cozinha])
UC4([Atualizar Pontos de Fidelidade])

Cliente --> UC1
Cliente --> UC2

UC1 --> UC3
UC2 --> Pagamento
UC2 --> UC4

UC3 --> Cozinheiro
UC4 --> Fidelidade
```

### Explicação

O diagrama apresenta os principais atores envolvidos no processo de autoatendimento: o Cliente, que realiza o pedido e o pagamento; o Cozinheiro, que recebe o pedido para preparo; o Sistema de Pagamento, responsável pela autorização da transação; e o Sistema de Fidelidade, que registra a pontuação do cliente após a compra.

---

# Cenário 3 – Sistema de Telemedicina

## Diagrama utilizado

Diagrama de Sequência

**Objetivo:**

Demonstrar a sequência de comunicação entre sensor, aplicativo, servidor e médico.

---

# Cenário 4 – Sistema de Controle de Acesso Inteligente

## Diagrama utilizado

Diagrama de Atividades

**Objetivo:**

Representar o fluxo de atividades desde a aproximação do usuário até a abertura da porta.

---

# Cenário 5 – Marketplace de Serviços Domésticos

## Diagrama utilizado

Diagrama de Casos de Uso

**Objetivo:**

Representar as funcionalidades do cliente e do profissional, utilizando relações de <<include>> e <<extend>>.

---

# Conclusão

Os diagramas desenvolvidos permitem representar diferentes perspectivas de um sistema, facilitando a compreensão de sua estrutura, comportamento e interação entre os atores envolvidos.
