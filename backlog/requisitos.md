## Requisitos Elicitados

A partir de entrevista realizada com o cliente, foram elicitados os requisitos do sistema, classificados em funcionais e não funcionais. Os requisitos funcionais abrangem controle de clientes, processos, prazos, documentos, compromissos, dados financeiros, presença online e integração com fontes externas de dados processuais. Os requisitos não funcionais estabelecem critérios de qualidade relacionados a performance, segurança, disponibilidade, conformidade com a LGPD, entre outros.

## Requisitos Funcionais

| ID | Categoria | Descrição |
|---|---|---|
| #RF01 | Fundação e Segurança | Autenticação de usuários via e-mail e senha com geração de token JWT e refresh token. |
| #RF02 | Fundação e Segurança | Recuperação de senha por e-mail. |
| #RF03 | Fundação e Segurança | Controle de permissões por papel (RBAC) com três perfis: Administrador, Advogado e Secretária. |
| #RF04 | Fundação e Segurança | Cadastro, edição, listagem, desativação e atribuição de papel de usuários do sistema. |
| #RF05 | Fundação e Segurança | Cadastro e edição dos dados do escritório (nome, CNPJ, endereço, telefone, horário de funcionamento, logotipo, redes sociais). |
| #RF06 | Fundação e Segurança | Registro automático e consulta de logs de auditoria (quem, o quê, quando), com filtragem pelo administrador. |
| #RF07 | Presença Online | Landing page institucional estática, com blog/seção de artigos, formulário de contato (e/ou botão direto para WhatsApp) e seções que passam credibilidade (sobre, serviços, diferenciais). |
| #RF08 | Presença Online | Edição dos textos e imagens da landing page (hero, sobre, diferenciais) pelo painel. |
| #RF09 | Presença Online | Cadastro, edição, listagem e exclusão de áreas de atuação com descrição. |
| #RF10 | Presença Online | Criação de artigos e notícias com título, conteúdo, imagem de capa e categoria, com preview antes da publicação. |
| #RF11 | Presença Online | Controle de status da publicação (rascunho, agendado ou publicado) com definição de data e hora para publicação automática. |
| #RF12 | Gestão de Relacionamento | Recepção automática de leads enviados pelo formulário da landing page. |
| #RF13 | Gestão de Relacionamento | Listagem de leads com filtros por data, status e responsável, com alteração de status e atribuição de responsável diretamente na lista. |
| #RF14 | Gestão de Relacionamento | Conversão de lead em cliente, migrando os dados para a ficha do cliente. |
| #RF15 | Gestão de Relacionamento | Cadastro, edição e busca de clientes por nome, CPF/CNPJ ou número de processo, com dados pessoais, endereço e contatos. |
| #RF16 | Gestão de Relacionamento | Visualização do histórico completo do cliente (origem como lead, processos, documentos, compromissos). |
| #RF17 | Core Jurídico | Cadastro de processo com número do CNJ, vara, comarca, tipo de ação, parte contrária, advogado responsável e vínculo ao cliente cadastrado. |
| #RF18 | Core Jurídico | Listagem de processos com filtros por status, vara, área, advogado e cliente, com alteração de status (ativo, suspenso, arquivado, encerrado). |
| #RF19 | Core Jurídico | Linha do tempo do processo com registro manual de movimentações. |
| #RF20 | Core Jurídico | Anotações internas do advogado vinculadas ao processo. |
| #RF21 | Agenda e Prazos | Cadastro de compromissos (consulta, audiência, reunião) com data, hora, duração e vínculo a um cliente ou processo. |
| #RF22 | Agenda e Prazos | Visualização da agenda por dia, semana e mês. |
| #RF23 | Agenda e Prazos | Definição de horários disponíveis pelo advogado. |
| #RF24 | Agenda e Prazos | Agendamento de consulta pela secretária vinculado a um lead ou cliente. |
| #RF25 | Agenda e Prazos | Cadastro de prazos vinculados a processos, com alertas escalonados (5 dias, 2 dias e véspera). |
| #RF26 | Agenda e Prazos | Cálculo automático de prazo processual em dias úteis, com cadastro e manutenção da tabela de feriados forenses por comarca. |
| #RF27 | Notificações | Central de notificações no painel com listagem, marcação como lida e histórico. |
| #RF28 | Notificações | Notificação automática ao advogado quando há nova movimentação em processo ou prazo próximo do vencimento. |
| #RF29 | Integrações Externas | Consulta de movimentações processuais via API (CNJ) pelo número do processo, com inserção automática das movimentações retornadas na linha do tempo. |
| #RF30 | Integrações Externas | Atualização periódica automática das movimentações dos processos ativos via API. |
| #RF31 | Integrações Externas | Consulta de dados de pessoa jurídica via API da Receita Federal (CNPJ). |
| #RF32 | Integrações Externas | Cadastro das credenciais de acesso à API jurídica. |
| #RF33 | Integrações Externas | Log de todas as chamadas a APIs externas com status de sucesso ou falha, e retentativa automática em caso de falha temporária. |
| #RF34 | Backup, LGPD e Compliance | Backup automatizado do banco de dados e arquivos com agendamento configurável. |
| #RF35 | Backup, LGPD e Compliance | Política de retenção de dados com exclusão automática após período definido. |
| #RF36 | Backup, LGPD e Compliance | Anonimização dos dados de ex-clientes após encerramento da relação. |
| #RF37 | Backup, LGPD e Compliance | Termo de consentimento no formulário da landing page com registro de aceite. |
| #RF38 | Workflow e Tarefas | Criação de tarefas com título, descrição, prazo, prioridade (baixa, média, alta, urgente) e atribuição de responsável. |
| #RF39 | Workflow e Tarefas | Vínculo da tarefa a um processo, cliente ou avulsa. |
| #RF40 | Workflow e Tarefas | Quadro Kanban com colunas configuráveis (a fazer, em andamento, concluída). |
| #RF41 | Workflow e Tarefas | Checklist de subtarefas dentro de uma tarefa. |
| #RF42 | Workflow e Tarefas | Sugestão automática de criação de tarefa ao alterar o status de um processo. |

---

## Requisitos Não Funcionais

| ID | Categoria | Descrição |
|---|---|---|
| #RNF01 | Performance | Tempo de resposta da API abaixo de 500ms para operações comuns. |
| #RNF02 | Performance | Landing page com tempo de carregamento abaixo de 3 segundos em conexão 3G, implementada com geração estática (SSG) e rebuild incremental. |
| #RNF03 | Responsividade | Interface funcional em telas a partir de 320px de largura. |
| #RNF04 | SEO | Score acima de 90 no Lighthouse para SEO, com URLs amigáveis nas publicações e schema markup de Article e LegalService. |
| #RNF05 | Segurança | Comunicação exclusivamente via HTTPS. |
| #RNF06 | Segurança | Senhas armazenadas com hash Argon2id. |
| #RNF07 | Segurança | Proteção contra brute force no login com limite de tentativas. |
| #RNF08 | Segurança | Tokens JWT com expiração de curta duração e refresh tokens com rotação. |
| #RNF09 | Acessibilidade | Contraste mínimo AA conforme WCAG 2.1 e texto alternativo em todas as imagens da landing page. |
| #RNF10 | Disponibilidade | Hospedagem com uptime mínimo de 99,9%. |
| #RNF11 | Compatibilidade | Suporte aos navegadores Chrome, Firefox, Safari e Edge nas duas últimas versões. |
| #RNF12 | Escalabilidade | Arquitetura da API preparada para adição de novos papéis e permissões sem reestruturação. |
| #RNF13 | Escalabilidade | Armazenamento de arquivos em serviço externo (object storage) para escalar independentemente do servidor. |
| #RNF14 | Manutenibilidade | Código da API organizado em camadas (handler, service, repository). |
| #RNF15 | Manutenibilidade | Cobertura mínima de 70% em testes automatizados nas regras de negócio. |
| #RNF16 | Integrações | Retentativas com backoff exponencial e circuit breaker para isolar falhas de serviços externos sem afetar o sistema. |
| #RNF17 | LGPD | Consentimento explícito antes da coleta de dados pessoais via formulário, com registro de todas as bases legais para tratamento. |