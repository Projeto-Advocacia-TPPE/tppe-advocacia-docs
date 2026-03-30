# Backlog

## Épico 1: Autenticação

| ID | História |
|---|---|
| US-01 | Como usuário do sistema, quero fazer login com meu e-mail e senha, para que eu acesse as funcionalidades autorizadas ao meu perfil. |
| US-02 | Como usuário que esqueceu sua senha, quero solicitar a redefinição de senha por e-mail, para que eu recupere o acesso à minha conta sem depender de um administrador. |
| US-03 | Como Administrador, quero cadastrar, editar, listar e desativar usuários, bem como atribuir e alterar seus papéis, para que eu controle quem tem acesso ao sistema e com quais permissões. |
| US-04 | Como Administrador, quero que toda ação relevante no sistema seja registrada automaticamente e que eu possa consultar esses registros, para que eu tenha rastreabilidade completa das operações realizadas. |

## Épico 2: Landing Page

| ID | História |
|---|---|
| US-05 | Como Administrador, quero cadastrar e editar as informações institucionais do escritório, para que esses dados sejam exibidos corretamente no site e em documentos gerados pelo sistema. |
| US-06 | Como visitante do site, quero acessar uma página institucional do advogado com informações claras sobre quem é, o que faz e como entrar em contato, para que eu avalie se o escritório atende às minhas necessidades e consiga iniciar contato facilmente. |
| US-07 | Como visitante do site, quero acessar uma seção de artigos publicados pelo advogado, para que eu me informe sobre temas jurídicos relevantes e perceba a autoridade técnica do profissional. |
| US-08 | Como Administrador, quero editar os textos e imagens das seções da landing page (hero, sobre, diferenciais) diretamente pelo painel administrativo, para que o conteúdo institucional seja atualizado sem necessidade de alteração em código. |
| US-09 | Como Advogado ou Administrador, quero criar e editar artigos com título, conteúdo, imagem de capa (se possuir) e categoria, e definir se o artigo é rascunho ou publicado, para que eu produza conteúdo jurídico de qualidade com controle sobre quando ele se torna visível ao público. |
| US-10 | Como Advogado ou Administrador, quero visualizar um preview do artigo exatamente como ele aparecerá para o visitante no blog, antes de publicá-lo, para que eu revise formatação, imagens e leitura geral sem expor o conteúdo ao público. |
| US-11 | Como visitante do site, quero visualizar depoimentos de clientes ou relatos de casos de sucesso (mesmo que genéricos e sem identificação), para que eu tenha mais confiança na competência do profissional antes de entrar em contato. |
| US-12 | Como Administrador, quero cadastrar, editar e reordenar depoimentos exibidos na landing page pelo painel administrativo, para que a seção de prova social seja mantida atualizada sem necessidade de alteração em código. |

## Épico 3: Gestão de leads e clientes

| ID | História |
|---|---|
| US-13 | Como Administrador, quero que os leads originados do formulário de contato do site já estejam disponíveis no painel assim que forem submetidos, para que eu acompanhe o interesse de potenciais clientes sem depender de registro manual." |
| US-14 | Como Administrador ou Secretária, quero listar, filtrar, alterar o status e atribuir responsáveis aos leads recebidos, para que o escritório acompanhe o funil de atendimento de forma organizada e nenhum lead fique sem tratamento. |
| US-15 | Como Administrador ou Advogado, quero converter um lead em cliente, aproveitando os dados já registrados, para que a transição seja fluida, sem retrabalho de digitação, e o vínculo entre lead e cliente fique rastreável. |
| US-16 | Como Administrador, Advogado ou Secretária, quero cadastrar e editar os dados pessoais e de contato dos clientes do escritório, para que o sistema mantenha uma base de clientes completa, atualizada e utilizável por toda a equipe. |
| US-17 | Como Advogado ou Administrador, quero visualizar, em uma única tela, o histórico completo de um cliente, desde a origem como lead até processos, documentos e compromissos vinculados, para que eu tenha contexto total do relacionamento antes de qualquer atendimento ou decisão. |
| US-18 | Como qualquer usuário autenticado, quero buscar clientes por nome, CPF/CNPJ ou número de processo vinculado, para que eu localize rapidamente a ficha do cliente que preciso consultar ou atualizar. |
| US-19 | Como Advogado, Administrador ou Secretária, quero registrar observações internas vinculadas diretamente a um cliente (independentemente de processo), para que eu mantenha anotações sobre o relacionamento, preferências ou contexto geral do cliente antes mesmo de existir um processo associado. |

## Épico 4: Core Jurídico

| ID | História |
|---|---|
| US-20 | Como Advogado ou Administrador, quero cadastrar um processo judicial informando seus dados essenciais e vinculá-lo a um cliente cadastrado, para que o escritório tenha um registro centralizado de cada processo com a identificação clara de quem é o cliente atendido. |
| US-21 | Como Advogado ou Administrador, quero registrar manualmente movimentações no processo e visualizá-las como uma linha do tempo cronológica, para que eu tenha um histórico completo e legível da evolução processual em um só lugar. |
| US-22 | Como Advogado ou Administrador, quero alterar o status de um processo entre ativo, suspenso, arquivado e encerrado, para que a situação atual de cada processo esteja sempre refletida no sistema e facilite a organização do trabalho. |
| US-23 | Como Advogado quero registrar anotações internas vinculadas a um processo, para que eu mantenha observações, estratégias e lembretes pessoais organizados dentro do contexto do caso, sem que se misturem com as movimentações formais. |
| US-24 | Como Administrador, Advogado ou Secretária, quero listar todos os processos do escritório e filtrá-los por diversos critérios, para que eu encontre rapidamente o processo que preciso sem percorrer a base manualmente. |

## Épico 5: APIs externas

| ID | História |
|---|---|
| US-25 | Como Advogado, quero visualizar as movimentações processuais atualizadas diretamente na linha do tempo de cada processo, sem precisar acessar portais dos tribunais manualmente, para que eu acompanhe a evolução dos casos de forma centralizada e eficiente. |
| US-26 | Como Administrador, Advogado ou Secretária, quero consultar os dados de uma pessoa jurídica pela API da Receita Federal ao informar o CNPJ, para que os campos de cadastro (razão social, endereço, situação cadastral) sejam preenchidos automaticamente, reduzindo digitação e erros. |
| US-27 | Como Administrador, quero consultar um registro de todas as chamadas realizadas pelo sistema a APIs externas, com status de sucesso ou falha, para que eu possa monitorar a saúde das integrações e identificar problemas rapidamente. |

## Épico 6: Notificações

| ID | História |
|---|---|
| US-28 | Como usuário do sistema, quero acessar uma central de notificações no painel com todas as notificações que recebi, podendo marcá-las como lidas e consultar o histórico, para que eu não perca nenhum aviso importante e consiga gerenciar o que já foi visto. |
| US-29 | Como usuário do sistema, quero receber notificações por e-mail para os eventos que considero importantes, para que eu seja informado mesmo quando não estiver logado no painel. |
| US-30 | Como usuário do sistema, quero configurar quais tipos de notificação desejo receber e por qual canal (painel, e-mail ou ambos), para que eu controle o volume de avisos e receba apenas o que é relevante para mim, da forma que prefiro. |
| US-31 | Como usuário autenticado, quero ser notificado automaticamente quando ocorrerem eventos relevantes para o meu trabalho, como novas movimentações em processos sob minha responsabilidade ou vencimento iminente de prazos, para que eu tome as providências necessárias sem depender de comunicação manual entre a equipe. |

## Épico 7: Backup, LGPD e Compliance

| ID | História |
|---|---|
| US-32 | Como Administrador, quero exportar todos os dados pessoais de um cliente em formato estruturado e legível, para que o escritório atenda ao direito de portabilidade previsto na LGPD quando solicitado pelo titular. |
| US-33 | Como Administrador, quero anonimizar os dados pessoais de um ex-cliente após o encerramento da relação com o escritório, para que o escritório cumpra o princípio de minimização da LGPD, mantendo apenas o necessário para obrigações legais. |
| US-34 | Como visitante da landing page, quero visualizar o termo de consentimento de uso dos meus dados antes de enviar o formulário de contato, para que eu saiba como meus dados serão tratados e possa autorizar o uso de forma consciente. |

## Épico 8: Agenda e Prazos

| ID | História |
|---|---|
| US-35 | Como Advogado, Administrador ou Secretária, quero cadastrar compromissos na agenda informando tipo, data, hora, duração e vínculo opcional com cliente ou processo, para que todos os eventos do escritório fiquem registrados em um só lugar com o contexto necessário para cada atendimento. |
| US-36 | Como Advogado, Administrador ou Secretária, quero visualizar a agenda do escritório nas visões de dia, semana e mês, para que eu tenha clareza sobre a distribuição dos compromissos e consiga identificar rapidamente horários livres e ocupados. |
| US-37 | Como Advogado, quero informar a data de início, o tipo de prazo e a comarca de um processo e visualizar imediatamente a data-limite calculada em dias úteis com os feriados forenses considerados, para que eu tenha segurança na contagem de prazo sem risco de erro de cálculo manual. |
| US-38 | Como Advogado, quero receber alertas automáticos quando um prazo processual estiver se aproximando do vencimento, em intervalos escalonados, para que eu tenha tempo suficiente para preparar a peça ou tomar a providência necessária sem risco de perda de prazo. |

## Épico 9: Workflow e Tarefas

| ID | História |
|---|---|
| US-39 | Como Advogado, Administrador ou Secretária, quero criar tarefas com título, descrição, prazo, prioridade e responsável, podendo vinculá-las a um processo, cliente ou mantê-las avulsas, para que o escritório organize e distribua o trabalho operacional de forma clara, com contexto e responsabilidade definidos. |
| US-40 | Como Advogado, Administrador ou Secretária, quero visualizar e gerenciar as tarefas em um quadro Kanban com colunas representando os estágios do fluxo de trabalho, para que eu tenha visão clara do andamento de todas as tarefas e possa atualizar o status com um simples arrastar. |
