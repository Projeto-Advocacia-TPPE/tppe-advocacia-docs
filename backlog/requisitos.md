# Backlog do Produto

A partir da entrevista realizada com o cliente, foram definidos requisitos e histórias de usuário para um sistema de gestão jurídica com presença online e integração com APIs externas.

---

# Épico 1: Autenticação e Segurança

Como usuário do sistema, quero fazer login com e-mail e senha, para que eu acesse as funcionalidades autorizadas ao meu perfil.

Como usuário, quero que o sistema utilize autenticação com token JWT e refresh token, para que minha sessão seja segura e persistente.

Como usuário que esqueceu sua senha, quero solicitar recuperação por e-mail, para que eu recupere o acesso sem depender de suporte.

Como Administrador, quero cadastrar, editar e gerenciar usuários, para que eu controle o acesso ao sistema.

Como Administrador, quero atribuir papéis (Administrador, Advogado e Secretária), para que cada usuário tenha permissões adequadas.

Como Administrador, quero que todas as ações relevantes sejam registradas automaticamente, para que haja rastreabilidade do sistema.

Como Administrador, quero consultar logs de auditoria com filtros, para que eu possa investigar ações realizadas.

---

# Épico 2: Presença Online e Landing Page

Como visitante, quero acessar uma landing page institucional, para conhecer o advogado e seus serviços.

Como visitante, quero visualizar artigos jurídicos, para me informar sobre temas relevantes.

Como visitante, quero entrar em contato facilmente via formulário ou WhatsApp, para iniciar atendimento.

Como Administrador, quero editar textos e imagens da landing page, para manter o conteúdo atualizado.

Como Advogado, quero criar artigos com título, conteúdo e imagem, para produzir conteúdo jurídico.

Como Advogado, quero definir o status da publicação (rascunho, agendado ou publicado), para controlar visibilidade.

Como Advogado, quero visualizar um preview antes de publicar, para revisar o conteúdo.

---

# Épico 3: Gestão de Leads e Clientes

Como sistema, quero registrar automaticamente leads vindos da landing page, para não perder potenciais clientes.

Como usuário, quero listar e filtrar leads, para organizar o atendimento.

Como Administrador, quero converter um lead em cliente, para evitar retrabalho.

Como usuário, quero cadastrar e editar clientes, para manter uma base atualizada.

Como Advogado, quero visualizar o histórico completo do cliente, para ter contexto antes do atendimento.

Como usuário, quero buscar clientes por nome, CPF/CNPJ ou processo, para localizar rapidamente.

---

# Épico 4: Core Jurídico

Como Advogado, quero cadastrar processos com seus dados principais, para manter controle centralizado.

Como sistema, quero vincular processos a clientes, para organizar os dados.

Como Advogado, quero registrar movimentações manualmente em uma linha do tempo, para acompanhar o processo.

Como Advogado, quero alterar o status do processo, para refletir sua situação atual.

Como Advogado, quero adicionar anotações internas, para registrar estratégias.

Como usuário, quero listar e filtrar processos, para facilitar a busca.

Como sistema, quero cadastrar prazos vinculados aos processos, para controlar vencimentos.

Como sistema, quero notificar o usuário sobre prazos próximos, para evitar perdas.

---

# Épico 5: Integrações com APIs

Como Advogado, quero consultar movimentações processuais via API (CNJ/DATAJUD), para evitar consultas manuais.

Como sistema, quero inserir automaticamente as movimentações retornadas na linha do tempo, para manter os dados atualizados.

Como sistema, quero executar consultas periódicas em processos ativos, para manter o sistema atualizado.

Como usuário, quero consultar dados de empresas via API da Receita Federal, para preencher automaticamente informações.

Como Administrador, quero visualizar logs de chamadas de API, para monitorar o sistema.

Como sistema, quero realizar retentativas automáticas em caso de falha, para aumentar a confiabilidade.

---

# Requisitos Funcionais

| ID    | Categoria     | Descrição |
| ----- | ------------- | --------- |
| RF01 | Segurança | Login com e-mail e senha |
| RF02 | Segurança | JWT com refresh token |
| RF03 | Segurança | Recuperação de senha |
| RF04 | Segurança | Logs de auditoria |
| RF05 | Presença | Landing page |
| RF06 | Presença | Edição da landing page |
| RF07 | Presença | Preview de artigos |
| RF08 | CRM | Captura de leads |
| RF09 | CRM | Gestão de leads |
| RF10 | CRM | Gestão de clientes |
| RF11 | Jurídico | Cadastro de processos |
| RF12 | Jurídico | Listagem e filtros de processos |
| RF13 | Jurídico | Anotações |
| RF14 | Jurídico | Gestão de prazos |

---

# Requisitos Não Funcionais

**RNF01.** O sistema deve possuir autenticação segura baseada em JWT.  
**RNF02.** O sistema deve ser responsivo (desktop e mobile).  
**RNF03.** O sistema deve registrar logs de auditoria.  
**RNF04.** O sistema deve suportar integração com APIs externas.  
**RNF05.** O sistema deve tratar falhas de API com retentativas automáticas.  
**RNF06.** O sistema deve garantir integridade dos dados.  
**RNF07.** O sistema deve permitir expansão futura.  
