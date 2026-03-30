## Requisitos Elicitados

A partir de entrevista realizada com o cliente, foram elicitados os requisitos do sistema, classificados em funcionais e não funcionais. Os requisitos funcionais abrangem controle de clientes, processos, prazos, documentos, compromissos, dados financeiros, presença online e integração com fontes externas de dados processuais. Os requisitos não funcionais estabelecem critérios de qualidade relacionados a performance, segurança, disponibilidade, conformidade com a LGPD, entre outros.

## Requisitos Funcionais

| ID | Categoria | Descrição |
|---|---|---|
| RF01 | Fundação e Segurança | Autenticação de usuários via e-mail e senha. |
| RF02 | Fundação e Segurança | Recuperação de senha por e-mail. |
| RF03 | Fundação e Segurança | Cadastro, edição, listagem, desativação e atribuição de papel de usuários do sistema. |
| RF04 | Fundação e Segurança | Cadastro e edição dos dados do escritório (nome, CNPJ, endereço, telefone, horário de funcionamento, logotipo, redes sociais). |
| RF05 | Fundação e Segurança | Registro automático e consulta de logs de auditoria (quem, o quê, quando), com filtragem pelo administrador. |
| RF06 | Presença Online | Landing page institucional estática, com blog/seção de artigos, formulário de contato (e/ou botão direto para WhatsApp) e seções que passam credibilidade (sobre, serviços, diferenciais). |
| RF07 | Presença Online | Edição dos textos e imagens da landing page (hero, sobre, diferenciais) pelo painel. |
| RF08 | Presença Online | Criação de artigos e notícias com título, conteúdo, imagem de capa e categoria, com preview antes da publicação. |
| RF09 | Presença Online | Controle de status da publicação (rascunho, agendado ou publicado) com definição de data e hora para publicação automática. |
| RF10 | Gestão de Relacionamento | Recepção automática de leads enviados pelo formulário da landing page. |
| RF11 | Gestão de Relacionamento | Listagem de leads com filtros por data, status e responsável, com alteração de status e atribuição de responsável diretamente na lista. |
| RF12 | Gestão de Relacionamento | Conversão de lead em cliente, migrando os dados para a ficha do cliente. |
| RF13 | Gestão de Relacionamento | Cadastro, edição e busca de clientes por nome, CPF/CNPJ ou número de processo, com dados pessoais, endereço e contatos. |
| RF14 | Gestão de Relacionamento | Visualização do histórico completo do cliente (origem como lead, processos, documentos, compromissos). |
| RF15 | Core Jurídico | Cadastro de processo com número do CNJ, vara, comarca, tipo de ação, parte contrária, advogado responsável e vínculo ao cliente cadastrado. |
| RF16 | Core Jurídico | Listagem de processos com filtros por status, vara, área, advogado e cliente, com alteração de status (ativo, suspenso, arquivado, encerrado). |
| RF17 | Core Jurídico | Linha do tempo do processo com registro manual de movimentações. |
| RF18 | Core Jurídico | Anotações internas do advogado vinculadas ao processo. |
| RF19 | Agenda e Prazos | Cadastro de compromissos (consulta, audiência, reunião) com data, hora, duração e vínculo a um cliente ou processo. |
| RF20 | Agenda e Prazos | Visualização da agenda por dia, semana e mês. |
| RF21 | Agenda e Prazos | Agendamento de consulta pela secretária vinculado a um lead ou cliente. |
| RF22 | Agenda e Prazos | Cadastro de prazos vinculados a processos, com alertas escalonados (5 dias, 2 dias e véspera). |
| RF23 | Agenda e Prazos | Cálculo automático de prazo processual em dias úteis, com cadastro e manutenção da tabela de feriados forenses por comarca. |
| RF24 | Notificações | Central de notificações no painel com listagem, marcação como lida e histórico. |
| RF25 | Notificações | Notificação automática ao advogado quando há nova movimentação em processo ou prazo próximo do vencimento. |
| RF26 | Integrações Externas | Consulta de movimentações processuais via API (CNJ) pelo número do processo, com inserção automática das movimentações retornadas na linha do tempo. |
| RF27 | Integrações Externas | Atualização periódica automática das movimentações dos processos ativos via API. |
| RF28 | Integrações Externas | Log de todas as chamadas a APIs externas com status de sucesso ou falha, e retentativa automática em caso de falha temporária. |
| RF29 | Backup, LGPD e Compliance | Anonimização dos dados de ex-clientes após encerramento da relação. |
| RF30 | Backup, LGPD e Compliance | Termo de consentimento no formulário da landing page com registro de aceite. |
| RF31 | Workflow e Tarefas | Criação de tarefas com título, descrição, prazo, prioridade (baixa, média, alta, urgente) e atribuição de responsável. |
| RF32 | Workflow e Tarefas | Vínculo da tarefa a um processo, cliente ou avulsa. |
| RF33 | Workflow e Tarefas | Quadro Kanban com colunas configuráveis (a fazer, em andamento, concluída). |
| RF34 | Presença Online | Visualização de depoimentos de clientes ou relatos de casos de sucesso na landing page. |
| RF35 | Presença Online | Cadastro, edição e reordenação de depoimentos exibidos na landing page pelo painel administrativo. |
| RF36 | Gestão de Relacionamento | Registro de anotações internas vinculadas diretamente a um cliente, independentemente de processo. |
| RF37 | Integrações Externas | Consulta de dados de pessoa jurídica pela API da Receita Federal ao informar CNPJ, com preenchimento automático de campos cadastrais. |
| RF38 | Notificações | Envio de notificações por e-mail para eventos importantes do sistema. |
| RF39 | Notificações | Configuração de canais de notificação (painel, e-mail ou ambos) e tipos de eventos a serem notificados por usuário. |
| RF40 | Backup, LGPD e Compliance | Exportação de todos os dados pessoais de um cliente em formato estruturado e legível para atender direito de portabilidade da LGPD. |

---

## Requisitos Não Funcionais

| ID | Descrição |
|---|---|
| RNF-01 | Controle de acesso por papel (RBAC): Toda rota protegida deve validar o papel do usuário autenticado. Os papéis são Administrador, Advogado e Secretária. Requisições sem token válido retornam 401; com papel insuficiente, 403. A matriz de permissões (papel × recurso) deve ser documentada e extensível. |
| RNF-02 | Responsividade: Todas as interfaces devem ser totalmente responsivas e oferecer experiência adequada em dispositivos móveis, tablets e desktops. |
| RNF-03 | Usabilidade e navegação: A landing page deve seguir padrões de navegação intuitiva, com menu claro, hierarquia visual consistente e tempo máximo de três cliques para o visitante alcançar qualquer seção principal do site. Elementos de contato devem estar acessíveis a partir de qualquer ponto da página. |
| RNF-04 | Periodicidade da consulta automática: O sistema deve executar a consulta de movimentações processuais de forma periódica e automatizada, com intervalo configurável. A implementação (cron job, scheduler, fila assíncrona) é decisão de arquitetura. |
| RNF-05 | Backup automatizado: O sistema deve realizar backup automatizado do banco de dados e dos arquivos armazenados (uploads, logotipos, imagens de artigos), com frequência configurável pelo Administrador (ex.: diário, a cada 12 horas). Os backups devem ser armazenados em local separado do ambiente de produção (ex.: bucket em outra região). O sistema deve manter um histórico de backups conforme a política de retenção e permitir restauração a partir de qualquer ponto retido. Falhas no processo de backup devem gerar notificação ao Administrador. |
| RNF-06 | Política de retenção: O sistema deve aplicar automaticamente uma política de retenção que remova dados expirados após período definido por tipo: logs de auditoria (ex.: 2 anos), logs de chamadas externas (ex.: 1 ano), notificações lidas (ex.: 90 dias), backups antigos (ex.: 30 dias). Os períodos devem ser configuráveis pelo Administrador. A exclusão automática deve ser registrada em log de infraestrutura. Dados vinculados a obrigações legais (processos judiciais, documentos fiscais) devem respeitar os prazos legais de guarda antes de serem elegíveis para exclusão. |
| RNF-07  | Segurança: Senhas armazenadas com hash Argon2id. |
| RNF-08  | Segurança: Proteção contra brute force no login com limite de 4 tentativas. |
| RNF-09  | Segurança: Tokens JWT com expiração de 1 hora e refresh tokens 3 dias. |
| RNF-10  | LGPD: Consentimento explícito antes da coleta de dados pessoais via formulário, com registro de todas as bases legais para tratamento. |
