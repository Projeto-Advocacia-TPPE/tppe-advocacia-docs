


As histórias de usuário foram elaboradas a partir das necessidades identificadas na entrevista com o cliente, estruturadas sob a perspectiva do usuário final no formato "Como *perfil*, quero *ação*, para que *objetivo*". Essa abordagem permite expressar os requisitos em linguagem natural, facilitando a validação com o cliente e o alinhamento com os requisitos funcionais formalizados na seção anterior. As histórias estão organizadas em épicos, que representam agrupamentos funcionais de maior granularidade.

---

### Épico 1: Autenticação e Segurança

| Como | Quero | Para que |
|---|---|---|
| Usuário do sistema | fazer login com meu e-mail e senha | eu acesse as funcionalidades autorizadas ao meu perfil |
| Usuário que esqueceu sua senha | solicitar a redefinição de senha por e-mail | eu recupere o acesso à minha conta sem depender de um administrador |
| Administrador | cadastrar, editar, listar e desativar usuários, bem como atribuir e alterar seus papéis | eu controle quem tem acesso ao sistema e com quais permissões |
| Administrador | que toda ação relevante no sistema seja registrada automaticamente e que eu possa consultar esses registros | eu tenha rastreabilidade completa das operações realizadas |
| Administrador | cadastrar e editar as informações institucionais do escritório | esses dados sejam exibidos corretamente no site e em documentos gerados pelo sistema |

---

### Épico 2: Presença Online e Landing Page

| Como | Quero | Para que |
|---|---|---|
| Visitante do site | acessar uma página institucional do advogado com informações claras sobre quem é, o que faz e como entrar em contato | eu avalie se o escritório atende às minhas necessidades e consiga iniciar contato facilmente |
| Visitante do site | acessar uma seção de artigos publicados pelo advogado | eu me informe sobre temas jurídicos relevantes e perceba a autoridade técnica do profissional |
| Administrador | editar os textos e imagens das seções da landing page diretamente pelo painel administrativo | o conteúdo institucional seja atualizado sem necessidade de alteração em código |
| Advogado ou Administrador | criar e editar artigos com título, conteúdo, imagem de capa e categoria, e definir se o artigo é rascunho ou publicado | eu produza conteúdo jurídico de qualidade com controle sobre quando ele se torna visível ao público |
| Advogado ou Administrador | visualizar um preview do artigo exatamente como ele aparecerá para o visitante no blog, antes de publicá-lo | eu revise formatação, imagens e leitura geral sem expor o conteúdo ao público |
| Visitante do site | visualizar depoimentos de clientes ou relatos de casos de sucesso | eu tenha mais confiança na competência do profissional antes de entrar em contato |
| Administrador | cadastrar, editar e reordenar depoimentos exibidos na landing page pelo painel administrativo | a seção de prova social seja mantida atualizada sem necessidade de alteração em código |

---

### Épico 3: Gestão de Leads e Clientes

| Como | Quero | Para que |
|---|---|---|
| Administrador | que toda submissão do formulário de contato gere automaticamente um registro de lead no sistema | nenhum potencial cliente seja perdido por falta de registro manual |
| Administrador ou Secretária | listar, filtrar, alterar o status e atribuir responsáveis aos leads recebidos | o escritório acompanhe o funil de atendimento de forma organizada e nenhum lead fique sem tratamento |
| Administrador ou Advogado | converter um lead em cliente, aproveitando os dados já registrados | a transição seja fluida, sem retrabalho de digitação, e o vínculo entre lead e cliente fique rastreável |
| Administrador, Advogado ou Secretária | cadastrar e editar os dados pessoais e de contato dos clientes do escritório | o sistema mantenha uma base de clientes completa, atualizada e utilizável por toda a equipe |
| Advogado ou Administrador | visualizar, em uma única tela, o histórico completo de um cliente, desde a origem como lead até processos, documentos e compromissos vinculados | eu tenha contexto total do relacionamento antes de qualquer atendimento ou decisão |
| Qualquer usuário autenticado | buscar clientes por nome, CPF/CNPJ ou número de processo vinculado | eu localize rapidamente a ficha do cliente que preciso consultar ou atualizar |
| Advogado, Administrador ou Secretária | registrar observações internas vinculadas diretamente a um cliente | eu mantenha anotações sobre o relacionamento, preferências ou contexto geral do cliente antes mesmo de existir um processo associado |

---

### Épico 4: Jurídico

| Como | Quero | Para que |
|---|---|---|
| Advogado ou Administrador | cadastrar um processo judicial informando seus dados essenciais e vinculá-lo a um cliente cadastrado | o escritório tenha um registro centralizado de cada processo com a identificação clara de quem é o cliente atendido |
| Advogado ou Administrador | registrar manualmente movimentações no processo e visualizá-las como uma linha do tempo cronológica | eu tenha um histórico completo e legível da evolução processual em um só lugar |
| Advogado ou Administrador | alterar o status de um processo entre ativo, suspenso, arquivado e encerrado | a situação atual de cada processo esteja sempre refletida no sistema e facilite a organização do trabalho |
| Advogado | registrar anotações internas vinculadas a um processo | eu mantenha observações, estratégias e lembretes pessoais organizados dentro do contexto do caso, sem que se misturem com as movimentações formais |
| Administrador, Advogado ou Secretária | listar todos os processos do escritório e filtrá-los por diversos critérios | eu encontre rapidamente o processo que preciso sem percorrer a base manualmente |

---

### Épico 5: Integrações com APIs Externas

| Como | Quero | Para que |
|---|---|---|
| Advogado | que o sistema consulte automaticamente as movimentações processuais via API (CNJ) e insira as novas movimentações na linha do tempo de cada processo | a equipe acompanhe a evolução dos processos sem depender de consulta manual nos portais dos tribunais |
| Administrador, Advogado ou Secretária | consultar os dados de uma pessoa jurídica pela API da Receita Federal ao informar o CNPJ | os campos de cadastro sejam preenchidos automaticamente, reduzindo digitação e erros |
| Administrador | consultar um registro de todas as chamadas realizadas pelo sistema a APIs externas, com status de sucesso ou falha | eu possa monitorar a saúde das integrações e identificar problemas rapidamente |

---

### Épico 6: Notificações

| Como | Quero | Para que |
|---|---|---|
| Usuário do sistema | acessar uma central de notificações no painel com todas as notificações que recebi, podendo marcá-las como lidas e consultar o histórico | eu não perca nenhum aviso importante e consiga gerenciar o que já foi visto |
| Usuário do sistema | receber notificações por e-mail para os eventos que considero importantes | eu seja informado mesmo quando não estiver logado no painel |
| Usuário do sistema | configurar quais tipos de notificação desejo receber e por qual canal (painel, e-mail ou ambos) | eu controle o volume de avisos e receba apenas o que é relevante para mim, da forma que prefiro |
| Escritório | que o sistema gere notificações automaticamente quando ocorrerem eventos relevantes | cada membro da equipe seja avisado no momento certo sem depender de comunicação manual |

---

### Épico 7: Backup, LGPD e Compliance

| Como | Quero | Para que |
|---|---|---|
| Administrador | exportar todos os dados pessoais de um cliente em formato estruturado e legível | o escritório atenda ao direito de portabilidade previsto na LGPD quando solicitado pelo titular |
| Administrador | anonimizar os dados pessoais de um ex-cliente após o encerramento da relação com o escritório | o escritório cumpra o princípio de minimização da LGPD, mantendo apenas o necessário para obrigações legais |
| Visitante da landing page | visualizar o termo de consentimento de uso dos meus dados antes de enviar o formulário de contato | eu saiba como meus dados serão tratados e possa autorizar o uso de forma consciente |

---

### Épico 8: Agenda e Prazos

| Como | Quero | Para que |
|---|---|---|
| Advogado, Administrador ou Secretária | cadastrar compromissos na agenda informando tipo, data, hora, duração e vínculo opcional com cliente ou processo | todos os eventos do escritório fiquem registrados em um só lugar com o contexto necessário para cada atendimento |
| Advogado, Administrador ou Secretária | visualizar a agenda do escritório nas visões de dia, semana e mês | eu tenha clareza sobre a distribuição dos compromissos e consiga identificar rapidamente horários livres e ocupados |
| Advogado ou Administrador | que o sistema calcule automaticamente prazos processuais em dias úteis, considerando feriados forenses da comarca do processo | eu tenha segurança na contagem de prazo sem depender de cálculo manual sujeito a erro |
| Advogado | receber alertas automáticos quando um prazo processual estiver se aproximando do vencimento, em intervalos escalonados | eu tenha tempo suficiente para preparar a peça ou tomar a providência necessária sem risco de perda de prazo |

---

### Épico 9: Workflow e Tarefas

| Como | Quero | Para que |
|---|---|---|
| Advogado, Administrador ou Secretária | criar tarefas com título, descrição, prazo, prioridade e responsável, podendo vinculá-las a um processo, cliente ou mantê-las avulsas | o escritório organize e distribua o trabalho operacional de forma clara, com contexto e responsabilidade definidos |
| Advogado, Administrador ou Secretária | visualizar e gerenciar as tarefas em um quadro Kanban com colunas representando os estágios do fluxo de trabalho | eu tenha visão clara do andamento de todas as tarefas e possa atualizar o status com um simples arrastar |
| Responsável por uma tarefa | criar uma checklist de subtarefas dentro de uma tarefa principal | eu quebre atividades complexas em etapas menores e acompanhe o progresso de cada uma |
| Advogado ou Administrador | que o sistema sugira automaticamente a criação de uma tarefa quando eu alterar o status de um processo | as ações decorrentes da mudança de fase não sejam esquecidas |