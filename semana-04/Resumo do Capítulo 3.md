**Resumo — Capítulo 3: Desenvolvimento Ágil de Software (Sommerville)**
---

**3.1 Desenvolvimento Ágil**
---

Durante os anos 1990, a engenharia de software era baseada principalmente em métodos tradicionais, que exigiam muito planejamento e documentação antes do início da programação. Na prática, isso causava atrasos, pois os requisitos mudavam enquanto o sistema ainda estava sendo especificado. Assim, quando o software ficava pronto, muitas vezes já não atendia às necessidades atuais do cliente.

Grande parte do esforço das equipes era dedicada à produção de documentos e modelos, que nem sempre traziam valor direto ao usuário final. Esse excesso de formalidade gerou insatisfação e levou ao surgimento do desenvolvimento ágil, que propõe processos mais simples e flexíveis.

Em 2001, foi criado o Manifesto Ágil, que definiu quatro valores principais:

- Indivíduos e interações acima de processos e ferramentas
- Software funcionando acima de documentação abrangente
- Colaboração com o cliente acima de negociação de contratos
- Responder a mudanças acima de seguir um plano

Esses valores não eliminam planejamento ou documentação, mas colocam o foco principal no funcionamento do software e na adaptação às mudanças.

**3.2 Princípios do Desenvolvimento Ágil**
--

Os princípios ágeis são derivados dos valores do manifesto e orientam a forma como os projetos são conduzidos.

Um dos princípios principais é o envolvimento contínuo do cliente, que participa durante todo o desenvolvimento, ajudando a definir e priorizar requisitos. Isso reduz o risco de construir funcionalidades desnecessárias.

Outro princípio importante é o desenvolvimento incremental, em que o sistema é construído em pequenas partes ao longo de ciclos curtos. A cada ciclo, uma versão funcional é entregue, permitindo que o cliente avalie o progresso e sugira mudanças.

As equipes ágeis normalmente são pequenas e multidisciplinares, com autonomia para tomar decisões técnicas. A comunicação direta entre os membros é valorizada, reduzindo a necessidade de documentação extensa.

Além disso, mudanças de requisitos são tratadas como algo natural, e não como um problema. O processo é estruturado para aceitar alterações com facilidade. A simplicidade também é valorizada, evitando funcionalidades desnecessárias.

**3.3 Desenvolvimento Ágil versus Desenvolvimento Dirigido por Plano**
---

Sommerville compara o desenvolvimento ágil com o desenvolvimento dirigido por plano, que representa os métodos tradicionais.

No desenvolvimento dirigido por plano, todas as atividades são definidas com antecedência. O projeto é dividido em fases, como levantamento de requisitos, projeto, implementação e testes. Cada fase gera documentos formais que servem de base para a próxima. Esse modelo oferece maior previsibilidade e rastreabilidade, mas é menos flexível diante de mudanças.

Já no desenvolvimento ágil, o planejamento é feito de forma incremental. Apenas as atividades mais próximas são detalhadas, enquanto o restante é ajustado ao longo do projeto. Isso permite maior adaptação quando surgem novas necessidades.

O autor destaca que nenhuma abordagem é melhor em todos os casos. A escolha depende do tipo de sistema, da equipe, do nível de risco e das exigências do projeto.

**3.4 Métodos Ágeis**
---

Existem vários métodos ágeis que aplicam os princípios do manifesto. Entre os principais, destacam-se:

**Scrum:**
Organiza o desenvolvimento em ciclos curtos chamados sprints, geralmente com duração de duas a quatro semanas. O foco principal é a organização do trabalho e o acompanhamento do progresso da equipe.

**Extreme Programming (XP):**
É um método que enfatiza práticas técnicas rigorosas para garantir qualidade e flexibilidade. O XP propõe a realização frequente de testes, integração constante e forte colaboração entre os membros da equipe.

**Crystal:**
É uma família de métodos que varia conforme o tamanho e a criticidade do projeto. A principal ideia é adaptar o processo ao contexto específico da equipe.

**3.5 Extreme Programming (XP)**
---

O XP propõe levar boas práticas ao extremo para aumentar a qualidade do software e facilitar mudanças.

Uma das práticas principais é o desenvolvimento orientado a testes (TDD), em que os testes são escritos antes do código. Isso ajuda a garantir que o sistema funcione corretamente e facilita futuras modificações.

Outra prática importante é a programação em pares, em que dois desenvolvedores trabalham juntos em um único computador. Um escreve o código enquanto o outro revisa, permitindo detectar erros rapidamente e compartilhar conhecimento.

O XP também utiliza integração contínua, que consiste em integrar frequentemente o código ao sistema principal, executando testes automatizados para identificar falhas rapidamente.

Além disso, o método incentiva a refatoração contínua, melhorando o código sem alterar seu funcionamento, e a criação de releases pequenas e frequentes, permitindo que o cliente acompanhe o progresso.

A presença constante do cliente também é considerada essencial para esclarecer dúvidas e validar funcionalidades.


**3.6 Histórias de Usuário**
---

As histórias de usuário surgiram como uma alternativa mais simples aos documentos tradicionais de requisitos.

Elas são descrições curtas de funcionalidades escritas em linguagem natural, focadas nas necessidades reais do usuário. Geralmente seguem o formato:

"Como [tipo de usuário], quero [funcionalidade], para que [benefício]."

Esse formato ajuda a manter o foco no valor que a funcionalidade oferece, em vez de detalhes técnicos.

Cada história representa um ponto de conversa entre equipe e cliente, sendo detalhada quando chega o momento de implementá-la. As histórias também são usadas para planejamento, permitindo estimar esforço e definir quais funcionalidades serão desenvolvidas em cada ciclo.

Para garantir que a funcionalidade foi implementada corretamente, são definidos critérios de aceitação, que estabelecem condições claras para considerar a história concluída.
