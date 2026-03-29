# Requisitos Elicitados

A partir da entrevista realizada com o cliente, foram elicitados requisitos relacionados à organização e gestão de informações jurídicas, abrangendo controle de clientes, processos, prazos, documentos, compromissos e dados financeiros, além da integração com fontes externas de dados processuais. Os requisitos identificados foram classificados em funcionais e não funcionais, proporcionando maior clareza na definição do escopo do sistema.

## Requisitos Funcionais

| ID    | Categoria     | Descrição                                                              
| ----- | ------------- | ---------------------------------------------------------------------------------------------------------------------------------- | 
| #RF01 | Fundação e Segurança   | Autenticação de usuários via e-mail e senha com geração de token JWT e refresh token.   
| #RF02 | Fundação e Segurança   | Recuperação de senha por e-mail.                                    
| #RF03 | Fundação e Segurança   | Cadastro e edição dos dados do escritório (nome, CNPJ, endereço, telefone, horário de funcionamento, logotipo, redes sociais).
| #RF04 | Fundação e Segurança   |  Registro automático e consulta de logs de auditoria (quem, o quê, quando), com filtragem pelo administrador.
| #RF05 | Presença Online   | Landing page institucional estática, com Blog/seção de artigos, formulário de contato (e/ou botão direto pro WhatsApp) e seções que passam credibilidade (sobre, serviços, diferenciais).
| #RF06 | Presença Online   | Edição dos textos e imagens da landing page (hero, sobre, diferenciais) pelo painel.
| #RF07 | Presença Online   | Preview da publicação antes de publicar.
| #RF08 | Gestão de Relacionamento  | Recepção automática de leads enviados pelo formulário da landing page
| #RF09 | Gestão de Relacionamento  | Listagem de leads com filtros por data, status e responsável, com alteração de status e atribuição de responsável diretamente na lista.
| #RF10 | Gestão de Relacionamento  | Cadastro, edição e busca de clientes por nome, CPF/CNPJ ou número de processo, com dados pessoais, endereço e contatos.
| #RF11 | Core Jurídico | Cadastro de processo com número do CNJ, vara, comarca, tipo de ação, parte contrária, advogado responsável e vínculo ao cliente cadastrado.
| #RF12 | Core Jurídico | Listagem de processos com filtros por status, vara, área, advogado e cliente, com alteração de status (ativo, suspenso, arquivado, encerrado).
| #RF13 | Core Jurídico |  Anotações internas do advogado vinculadas ao processo.
| #RF14 | Core Jurídico |   Cadastro de prazos vinculados a processos, com notificação automática ao usuário conforme a proximidade do vencimento.
| #RF14 | Agendas e Prazos |   Cadastro de prazos vinculados a processos, com notificação automática ao usuário conforme a proximidade do vencimento.

