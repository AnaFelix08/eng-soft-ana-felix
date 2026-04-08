**Missão Crítica: Operação Resgate — Chaos-IT**
---

**Parte 1 — O Labirinto de Boehm**
---

**Por que a Análise de Riscos teria evitado a queda dos drones?**

No modelo espiral, cada volta obrigatoriamente passa pelo quadrante de Análise de Riscos antes de qualquer código ser escrito. No projeto de drones da Chaos-IT, a ausência desse processo significa que ninguém sistematicamente perguntou: o que pode dar errado?
Segundo Sommerville (cap. 2), o modelo espiral de Boehm é orientado a riscos: em cada ciclo, a equipe identifica os principais riscos, avalia sua probabilidade e impacto, e só avança se houver estratégia de mitigação. Isso teria forçado, por exemplo, a análise de falhas de comunicação entre drone e base, de latência crítica nos comandos e de comportamento em condições adversas, riscos que, ignorados, causaram a queda literal do sistema.
A diferença central em relação a modelos como cascata ou mesmo iterativo simples é que a decisão de continuar ou abortar o projeto é tomada com base em evidências de risco avaliadas, e não apenas em pressão de prazo ou otimismo da equipe.

**Ciclo da Espiral — Projeto IA Subaquática**
O diagrama acima mostra três voltas completas da espiral aplicadas ao projeto, com cada quadrante detalhado:
**Q1 — Planejamento:** Cada volta começa definindo objetivos, restrições e alternativas. Na V1 isso significa levantar escopo do sistema (navegação autônoma, coleta de dados, comunicação subaquática), identificar stakeholders e mapear recursos disponíveis. Na V2, o plano se refina com cronograma e alocação de equipe para os módulos já validados. Na V3, planejamento de implantação, SLA e manutenção contínua.
**Q2 — Análise de Riscos:** Este é o quadrante que salvaria o projeto de drones. Na V1 os riscos são de negócio: viabilidade técnica, regulação de operação subaquática, orçamento realista. Na V2 emergem os riscos técnicos críticos: falha de sensor de pressão, latência na comunicação acústica subaquática, overfitting do modelo de IA em ambientes de teste controlados. Na V3 revisam-se os riscos residuais após os testes integrados.
**Q3 — Engenharia:** Só após mitigar os riscos identificados a equipe constrói. Na V1 cria-se um protótipo mínimo em tanque controlado (PoC da IA de navegação). Na V2 desenvolvem-se os módulos completos — modelo de IA, protocolo de comunicação subaquática, firmware dos sensores. Na V3 faz-se a integração e validação do sistema completo em ambiente real monitorado.
**Q4 —Avaliação:**  pelo cliente O cliente valida o que foi construído antes da próxima volta começar. Na V1 revisa-se o PoC com os stakeholders para confirmar que os requisitos foram corretamente entendidos. Na V2 realizam-se testes de campo com registro sistemático de falhas. Na V3 ocorre o aceite formal e entrega.

**Parte 2 — O Diagnóstico CMMI**
---

**Nível atual: CMMI Nível 1 — Inicial**
A descrição da Chaos-IT é um diagnóstico claro do nível 1 do CMMI (Initial), caracterizado por processos imprevisíveis, pouco controlados e reativos.
As evidências diretas são três: cada desenvolvedor trabalha do seu jeito (ausência de processos padronizados), não há registro de erros passados (sem base de lições aprendidas ou gestão de conhecimento), os prazos são estimados sem método (sem modelos históricos de produtividade), e o sucesso depende de esforço heróico individual (o que o CMMI chama de "hero-based success" — sinal clássico do nível 1).
Organizações no nível 1 conseguem entregar, mas o sucesso não é reproduzível: depende das pessoas certas estarem disponíveis e dispostas a sacrificar seu tempo, não de processos confiáveis.
**Para alcançar o Nível 2 — Gerenciado**
O nível 2 do CMMI exige que os projetos sejam planejados, monitorados e controlados de forma consistente, com práticas básicas estabelecidas e repetíveis por projeto. O que a Chaos-IT precisaria implementar:
Gestão de requisitos: os requisitos de cada projeto devem ser documentados, versionados e rastreados, com controle formal de mudanças. Hoje os requisitos são implícitos e variam conforme a memória de cada dev.
**Planejamento de projeto:** estimativas de prazo e custo devem ser baseadas em dados históricos ou modelos estruturados (como pontos de função ou story points), não em "chutes". O plano precisa incluir marcos mensuráveis.
**Monitoramento e controle:** o progresso real precisa ser comparado ao plano regularmente, com ações corretivas documentadas quando há desvios.
**Gerência de configuração:** controle de versão obrigatório para código, documentação e artefatos do projeto, com histórico auditável de mudanças.
Registro sistemático de erros e lições aprendidas: a ausência desse registro é o que faz cada projeto repetir os mesmos problemas. Um repositório simples de post-mortems já representa uma mudança estrutural significativa.
A transição do nível 1 para o 2 não exige ferramentas sofisticadas — exige disciplina de processo. O principal obstáculo na Chaos-IT será cultural: os "devs heróis" precisam aceitar que processos documentados não são burocracia, mas o que torna o sucesso sustentável e independente de qualquer indivíduo específico.

