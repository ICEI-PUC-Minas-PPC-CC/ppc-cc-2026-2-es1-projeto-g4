# PRODUCT BACKLOG

## 1. Product Backlog Itens

> O backlog preliminar contém dez funcionalidades, agrupando ações relacionadas do projeto TaskEasy. As histórias e critérios do repositório original foram consolidados para se adequar ao modelo solicitado nesta atividade.

| # | Persona (Quem) | Dor/Necessidade (Por Quê) | Expectativa (Para Quê) | Funcionalidade (O Quê - Ação) |
| --- | --- | --- | --- | --- |
| F1 | Marina e Pedro | Precisam acessar suas próprias tarefas de forma individual. | Utilizar o sistema com uma conta e encerrar o acesso quando necessário. | Criar conta, entrar com e-mail e senha e sair da conta. |
| F2 | Marina e Pedro | Precisam registrar atividades para não depender de anotações dispersas. | Manter as atividades necessárias registradas no sistema. | Cadastrar uma tarefa informando título e descrição, com título obrigatório. |
| F3 | Marina | Tem dificuldade para acompanhar datas de entrega e prazos. | Identificar quando uma atividade deverá ser realizada. | Definir uma data de vencimento para a tarefa. |
| F4 | Marina e Pedro | Precisam consultar as atividades já registradas e sua situação. | Visualizar a lista de tarefas e reconhecer o que está pendente ou concluído. | Exibir a lista de tarefas com título e situação, inclusive uma mensagem quando não houver registros. |
| F5 | Marina e Pedro | As informações de uma atividade podem mudar ou precisar de correção. | Manter os dados da tarefa atualizados. | Editar título, descrição e data de vencimento de uma tarefa. |
| F6 | Marina e Pedro | Algumas atividades deixam de ser necessárias e não devem permanecer na lista. | Remover tarefas que não precisam mais ser acompanhadas. | Excluir uma tarefa mediante confirmação. |
| F7 | Marina e Pedro | Precisam registrar quando uma atividade foi finalizada. | Distinguir tarefas concluídas das que ainda precisam ser feitas. | Marcar uma tarefa como concluída e manter sua situação visível na lista. |
| F8 | Marina e Pedro | A lista pode misturar atividades em andamento e já finalizadas. | Consultar somente as tarefas de uma situação específica. | Filtrar tarefas pendentes e tarefas concluídas. |
| F9 | Marina | Tem dificuldade para perceber quais entregas estão mais próximas. | Dar destaque às atividades com prazo mais próximo. | Ordenar tarefas pela data de vencimento, deixando tarefas sem data ao final. |
| F10 | Marina e Pedro | Não conseguem ter uma visão rápida do volume de atividades em cada situação. | Acompanhar o andamento geral das tarefas. | Exibir a quantidade de tarefas pendentes e concluídas, atualizando os números após cadastro, conclusão ou exclusão. |

## 2. Revisão Técnica, UX e Negócios

> As avaliações abaixo são estimativas iniciais para discussão da equipe. Não representam medições de implementação concluída.

**Métricas:**

- **Valor de Negócio:** `$` (Baixo) a `$$$` (Alto)
- **Esforço Técnico:** `E` (Baixo) a `EEE` (Alto)
- **Valor UX:** ❤️ (Baixo) a ❤️❤️❤️ (Alto)
- **Confiança:** 🟢 (Alto), 🟡 (Médio), 🔴 (Baixo)

| # | Esforço Técnico | Valor UX | Valor de Negócio | Nível de Confiança (O que/Como) |
| :-- | :-- | :-- | :-- | :-- |
| **F1** | EE | ❤️❤️❤️ | $$$ | 🟡 Médio/Alto |
| **F2** | EE | ❤️❤️❤️ | $$$ | 🟢 Alto/Alto |
| **F3** | E | ❤️❤️ | $$ | 🟢 Alto/Alto |
| **F4** | EE | ❤️❤️❤️ | $$$ | 🟢 Alto/Alto |
| **F5** | EE | ❤️❤️ | $$ | 🟢 Alto/Alto |
| **F6** | E | ❤️❤️ | $$ | 🟢 Alto/Alto |
| **F7** | E | ❤️❤️❤️ | $$ | 🟢 Alto/Alto |
| **F8** | E | ❤️❤️ | $$ | 🟢 Alto/Alto |
| **F9** | E | ❤️❤️ | $$ | 🟡 Médio/Alto |
| **F10** | E | ❤️❤️ | $$ | 🟢 Alto/Alto |

### Justificativas

- **F1:** Cadastro e autenticação são necessários para associar tarefas a cada usuário. O esforço é médio por envolver validação de dados e controle de acesso. A necessidade está clara, mas detalhes de segurança e recuperação de acesso ainda precisam ser definidos.
- **F2:** É a ação central do produto e permite que o usuário registre suas atividades. O formulário é simples, com título obrigatório e descrição, portanto o esforço é médio e a confiança é alta.
- **F3:** A data de vencimento ajuda principalmente no acompanhamento de trabalhos e compromissos. A implementação prevista é simples, com validação do campo de data.
- **F4:** Consultar as tarefas é essencial para o uso diário. A lista deve apresentar título e situação e informar quando estiver vazia. É uma funcionalidade central, com requisitos bem definidos.
- **F5:** A edição evita que o usuário precise excluir e cadastrar novamente uma tarefa quando houver mudanças. O esforço é médio porque os campos existentes precisam ser atualizados e persistidos.
- **F6:** A exclusão é uma operação direta, mas a confirmação é importante para evitar remoções acidentais. A regra está definida no backlog original.
- **F7:** Marcar uma tarefa como concluída permite acompanhar o progresso. A ação altera a situação da tarefa sem removê-la da lista.
- **F8:** Os filtros facilitam a consulta de listas maiores. A regra é objetiva: exibir somente tarefas pendentes ou somente tarefas concluídas.
- **F9:** A ordenação por vencimento ajuda a priorizar atividades próximas do prazo. A regra para tarefas sem data foi definida no backlog original, mas a apresentação da ordenação ainda pode ser validada com usuários.
- **F10:** Os contadores oferecem uma visão rápida do andamento. A regra de atualização após cadastrar, concluir ou excluir está descrita no backlog original.

## 3. Product Backlog Itens (priorizado)

> Os itens estão organizados em ondas, respeitando o limite de três funcionalidades por onda, o esforço máximo de cinco Es, os valores mínimos de negócio e UX, e as dependências entre funcionalidades.

**Regras do Sequenciador:**

- **Regra 1:** Uma onda pode conter, no máximo, três funcionalidades.
- **Regra 2:** Uma onda não pode conter mais de uma funcionalidade em vermelho.
- **Regra 3:** Uma onda não pode conter três funcionalidades em amarelo e vermelho.
- **Regra 4:** A soma de esforço dos cartões não pode ultrapassar cinco Es.
- **Regra 5:** A soma de valor dos cartões de uma onda não pode ser menor que quatro $s e quatro corações.
- **Regra 6:** Se um cartão depende de outro cartão, esse outro deve estar em alguma onda anterior.

| # | Esforço Técnico | Valor UX | Valor de Negócio | Confiança (O quê) | Confiança (Como) | Onda |
| :-- | :-- | :-- | :-- | :-- | :-- | :--: |
| **F1** | EE | ❤️❤️❤️ | $$$ | Médio | Alto | 1 |
| **F2** | EE | ❤️❤️❤️ | $$$ | Alto | Alto | 1 |
| **F3** | E | ❤️❤️ | $$ | Alto | Alto | 1 |
| **F4** | EE | ❤️❤️❤️ | $$$ | Alto | Alto | 2 |
| **F5** | EE | ❤️❤️ | $$ | Alto | Alto | 2 |
| **F6** | E | ❤️❤️ | $$ | Alto | Alto | 2 |
| **F7** | E | ❤️❤️❤️ | $$ | Alto | Alto | 3 |
| **F8** | E | ❤️❤️ | $$ | Alto | Alto | 3 |
| **F9** | E | ❤️❤️ | $$ | Médio | Alto | 4 |
| **F10** | E | ❤️❤️ | $$ | Alto | Alto | 4 |

### Organização das ondas e dependências

- **Onda 1:** F1, F2 e F3 — acesso à conta, cadastro de tarefas e definição de vencimento. Esforço total: 5 Es. Valor de negócio: $$$ + $$$ + $$; valor UX: 8 corações.
- **Onda 2:** F4, F5 e F6 — consulta, edição e exclusão de tarefas. Esforço total: 5 Es. Valor de negócio: $$$ + $$ + $$; valor UX: 7 corações. F5 e F6 dependem da existência de tarefas, prevista em F2; F4 também consulta as tarefas cadastradas.
- **Onda 3:** F7 e F8 — conclusão e filtro por situação. Esforço total: 2 Es. Valor de negócio: $$ + $$; valor UX: 5 corações. Dependem das tarefas e da consulta disponibilizadas nas ondas anteriores.
- **Onda 4:** F9 e F10 — ordenação por vencimento e contadores. Esforço total: 2 Es. Valor de negócio: $$ + $$; valor UX: 4 corações. Dependem dos dados de tarefas e de suas datas/situações, disponíveis nas ondas anteriores.

## 4. Especificação Suplementar de Requisitos Não Funcionais

> Os requisitos abaixo são propostas iniciais para o TaskEasy. Devem ser validados pela equipe e, quando necessário, ajustados durante a definição da solução técnica.

| Requisito não-funcional | Descrição | Categoria | Prioridade |
| :-- | :-- | :-- | :-- |
| RNF.1 | As operações de consulta da lista de tarefas deverão apresentar resposta em até 5 segundos em condições normais de uso. | Desempenho | Alta |
| RNF.2 | A aplicação deverá ser compatível com a versão atual e as duas versões anteriores do Google Chrome. | Suportabilidade | Alta |
| RNF.3 | A interface deverá se adaptar a telas de smartphones e notebooks, sem perda das funções principais. | Usabilidade | Alta |
| RNF.4 | O sistema deverá validar os campos obrigatórios e apresentar mensagens compreensíveis quando os dados forem inválidos. | Usabilidade | Alta |
| RNF.5 | As senhas de usuários não deverão ser armazenadas em texto puro; deverá ser utilizado mecanismo apropriado de hash de senha. | Segurança | Alta |
| RNF.6 | Cada usuário autenticado deverá acessar somente as tarefas associadas à sua própria conta. | Segurança/Privacidade | Alta |
| RNF.7 | As operações de cadastro, edição, conclusão e exclusão deverão manter os dados consistentes após a confirmação da operação. | Confiabilidade | Alta |

---

[⬅ Anterior](02_personas.md) | [Próximo ➡](99_video_etapa_1.md)
