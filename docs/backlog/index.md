# Backlog

## Épico 1: Autenticação

| ID | História |
|---|---|
| US-01 | Como Advogado associado, quero fazer login com meu e-mail e senha, para que eu acesse as funcionalidades autorizadas ao meu perfil. |
| US-02 | Como Advogado associado que esqueceu sua senha, quero solicitar a redefinição de senha por e-mail, para que eu recupere o acesso à minha conta sem depender de um administrador. |
| US-03 | Como Administrador, quero cadastrar, editar, listar e desativar usuários, bem como atribuir e alterar seus papéis, para que eu controle quem tem acesso ao sistema e com quais permissões. |
| US-04 | Como Administrador, quero que todo usuário cadastrado ou excluido no sistema seja registrada automaticamente e que eu possa consultar esses registros, para que eu tenha rastreabilidade completa das operações realizadas. |

## Épico 2: Landing Page

| ID | História |
|---|---|
| US-05 | Como Administrador, quero cadastrar e editar as informações institucionais do escritório, para que esses dados sejam exibidos corretamente no site e em documentos gerados pelo sistema. |
| US-06 | Como Administrador, quero editar os textos e imagens das seções da landing page (hero, sobre, diferenciais) diretamente pelo painel administrativo, para que o conteúdo institucional seja atualizado sem necessidade de alteração em código. |
| US-07 | Como visitante do site, quero acessar uma seção de artigos publicados pelo advogado, para que eu me informe sobre temas jurídicos relevantes e perceba a autoridade técnica do profissional. |
| US-08 | Como Advogado associado, quero criar e editar artigos com título, conteúdo, imagem de capa (se possuir) e categoria, e definir se o artigo é rascunho ou publicado, para que eu produza conteúdo jurídico de qualidade com controle sobre quando ele se torna visível ao público. |
| US-09 | Como Advogado associado, quero visualizar um preview do artigo exatamente como ele aparecerá para o visitante no blog, antes de publicá-lo, para que eu revise formatação, imagens e leitura geral sem expor o conteúdo ao público. |
<!-- | ~~US-06~~ | ~~Como visitante do site, quero acessar uma página institucional do advogado com informações claras sobre quem é, o que faz e como entrar em contato, para que eu avalie se o escritório atende às minhas necessidades e consiga iniciar contato facilmente.~~ | -->

## Épico 3: Gestão de leads e clientes

| ID | História |
|---|---|
| US-10 | Como Administrador, quero que os leads originados do formulário de contato do site já estejam disponíveis no painel assim que forem submetidos, para que eu acompanhe o interesse de potenciais clientes sem depender de registro manual. |
| US-11 | Como Administrador, quero listar, filtrar, alterar o status e atribuir responsáveis aos leads recebidos, para que o escritório acompanhe o funil de atendimento de forma organizada e nenhum lead fique sem tratamento. |
| US-12 | Como Advogado associado, quero cadastrar e editar os dados pessoais e de contato dos clientes do escritório, para que o sistema mantenha uma base de clientes completa, atualizada e utilizável por toda a equipe. |
| US-13 | Como Advogado associado, quero visualizar, em uma única tela, o histórico completo de um cliente, desde a origem como lead até processos, documentos e compromissos vinculados, para que eu tenha contexto total do relacionamento antes de qualquer atendimento ou decisão. |
| US-14 | Como Advogado associado, quero buscar clientes por nome, CPF/CNPJ ou número de processo vinculado, para que eu localize rapidamente a ficha do cliente que preciso consultar ou atualizar. |
| US-15 | Como Advogado associado, quero registrar observações internas vinculadas diretamente a um cliente (independentemente de processo), para que eu mantenha anotações sobre o relacionamento, preferências ou contexto geral do cliente antes mesmo de existir um processo associado. |

## Épico 4: Core Jurídico

| ID | História |
|---|---|
| US-16 | Como Advogado associado, quero cadastrar um processo judicial informando seus dados essenciais e vinculá-lo a um cliente cadastrado, para que o escritório tenha um registro centralizado de cada processo com a identificação clara de quem é o cliente atendido. |
| US-17 | Como Advogado associado, quero registrar manualmente movimentações no processo e visualizá-las como uma linha do tempo cronológica, para que eu tenha um histórico completo e legível da evolução processual em um só lugar. |
| US-18 | Como Advogado associado, quero alterar o status de um processo entre ativo, suspenso, arquivado e encerrado, para que a situação atual de cada processo esteja sempre refletida no sistema e facilite a organização do trabalho. |
| US-19 | Como Advogado associado, quero registrar anotações internas vinculadas a um processo, para que eu mantenha observações, estratégias e lembretes pessoais organizados dentro do contexto do caso, sem que se misturem com as movimentações formais. |

## Épico 5: APIs externas

| ID | História |
|---|---|
| US-20 | Como Advogado associado, quero visualizar as movimentações processuais atualizadas diretamente na linha do tempo de cada processo, sem precisar acessar portais dos tribunais manualmente, para que eu acompanhe a evolução dos casos de forma centralizada e eficiente. |
| US-21 | Como Administrador, quero ser notificado de chamadas realizadas pelo sistema a APIs externas, com status de falha, para que eu possa monitorar a saúde das integrações e identificar problemas rapidamente. |

## Épico 6: Notificações

| ID | História |
|---|---|
| US-22 | Como Advogado associado, quero receber notificações por e-mail para os eventos que considero importantes, para que eu seja informado mesmo quando não estiver logado no painel. |
| US-23 | Como Advogado associado, quero ser notificado quando ocorrerem eventos em processos em que estou vinculado, para que eu tome as providências necessárias sem depender de comunicação manual entre a equipe. |

## Épico 7: Backup, LGPD e Compliance

| ID | História |
|---|---|
| US-24 | Como Administrador, quero excluir os dados pessoais de um ex-cliente após o encerramento da relação com o escritório, para que o escritório cumpra o princípio de minimização da LGPD, mantendo apenas o necessário para obrigações legais. |
| US-25 | Como visitante do site, quero visualizar o termo de consentimento de uso dos meus dados antes de enviar o formulário de contato, para que eu saiba como meus dados serão tratados e possa autorizar o uso de forma consciente. |

## Épico 8: Agenda e Prazos

| ID | História |
|---|---|
| US-26 | Como Advogado associado, quero cadastrar compromissos na agenda informando tipo, data, hora, duração e vínculo opcional com cliente ou processo, para que todos os eventos do escritório fiquem registrados em um só lugar com o contexto necessário para cada atendimento. |
| US-27 | Como Advogado associado, quero informar a data de início, o tipo de prazo e a comarca de um processo e visualizar imediatamente a data-limite calculada em dias úteis com os feriados forenses considerados, para que eu tenha segurança na contagem de prazo sem risco de erro de cálculo manual. |
| US-28 | Como Advogado associado, quero receber alertas automáticos quando um prazo processual estiver se aproximando do vencimento, em intervalos escalonados, para que eu tenha tempo suficiente para preparar a peça ou tomar a providência necessária sem risco de perda de prazo. |

## Épico 9: Workflow e Tarefas

| ID | História |
|---|---|
| US-29 | Como Administrador, quero criar tarefas com título, descrição, prazo, prioridade e responsável, podendo vinculá-las a um processo, cliente ou mantê-las avulsas, para que o escritório organize e distribua o trabalho operacional de forma clara, com contexto e responsabilidade definidos. |
| US-30 | Como Advogado associado, quero visualizar e gerenciar as tarefas em um quadro Kanban com colunas representando os estágios do fluxo de trabalho, para que eu tenha visão clara do andamento de todas as tarefas e possa atualizar o status com um simples arrastar. |
