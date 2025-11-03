# 📑 Backlog – Projeto HighTask

### ✅ Requisitos Funcionais (RF)

| Rank | Prioridade | User Story | Story Points | Sprint | Requisito do Cliente | Status |
|:----:|:----------:|------------|--------------|:------:|:--------------------:|:------:|
| 1 | Alta | Como administrador, quero cadastrar novos usuários, para que apenas pessoas autorizadas utilizem o sistema. | 13 | 1 | RF01 | Feito |
| 2 | Alta | Como usuário, quero receber um e-mail de confirmação após meu cadastro, para ter segurança no processo. | 5 | 1 | RF02 | Feito |
| 3 | Alta | Como administrador, quero editar dados de usuários e permissões, para manter as informações sempre atualizadas. | 8 | 1 | RF03 | Feito |
| 4 | Média | Como usuário, quero ser notificado por e-mail sobre alterações na minha conta, para acompanhar mudanças. | 5 | 1 | RF04 | Feito |
| 5 | Média | Como administrador, quero desativar contas sem excluí-las, para manter controle sobre acessos inativos. | 8 | 1 | RF05 | Feito |
| 6 | Alta | Como administrador, quero excluir contas de usuários definitivamente, para atender às políticas de retenção. | 8 | 1 | RF06 | Feito |
| 7 | Alta | Como administrador, quero definir permissões de acesso por níveis, para controlar funcionalidades por perfil. | 13 | 1 | RF07 | Feito |
| 8 | Média | Como administrador, quero redefinir senhas de usuários, para garantir acesso em casos de esquecimento. | 5 | 1 | RF08 | Feito |
| 9 | Alta | Como usuário, quero abrir chamados detalhados com anexos, para relatar problemas com clareza. | 21 | 2 | RF09 | Feito |
| 10 | Alta | Como usuário, quero que o sistema sugira uma categoria ao abrir um chamado, para agilizar o processo. | 13 | 2 | RF10 | Feito |
| 11 | Alta | Como técnico, quero ser automaticamente atribuído a chamados de minha área, para agilizar o atendimento. | 21 | 2 | RF11 | Feito |
| 12 | Média | Como administrador, quero reatribuir chamados e adicionar comentários, para gerenciar melhor a equipe. | 13 | 2 | RF12 | Feito |
| 13 | Alta | Como técnico, quero atualizar status de chamados, registrar tempo e observações, para acompanhar o atendimento. | 21 | 2 | RF13 | Feito |
| 14 | Média | Como técnico, quero solicitar informações adicionais ao usuário, para esclarecer dúvidas sobre o chamado. | 8 | 2 | RF14 | Feito |
| 15 | Alta | Como administrador, quero garantir que chamados só sejam fechados após validação, para assegurar a resolução. | 13 | 2 | RF15 | Feito |
| 16 | Alta | Como usuário, quero confirmar se meu problema foi resolvido, para validar o fechamento do chamado. | 8 | 2 | RF16 | Feito |
| 17 | Alta | Como usuário, quero que a IA analise minha descrição e sugira categorias, para facilitar a abertura de chamados. | 21 | 3 | RF17 | Feito |
| 18 | Alta | Como usuário, quero que a IA sugira soluções possíveis, para resolver problemas mais rápido. | 21 | 3 | RF18 | Feito |
| 19 | Alta | Como técnico, quero que a IA detecte chamados críticos automaticamente, para priorizar atendimentos urgentes. | 21 | 3 | RF19 | Feito |
| 20 | Alta | Como técnico, quero receber notificações imediatas de chamados críticos, para agir rapidamente. | 13 | 3 | RF20 | Feito |
| 21 | Alta | Como administrador, quero gerar relatórios de chamados e desempenho, para analisar a produtividade. | 21 | 4 | RF21 | Feito |
| 22 | Média | Como administrador, quero exportar relatórios em PDF e Excel, para compartilhar os resultados. | 8 | 4 | RF22 | Feito |
| 23 | Alta | Como administrador, quero acessar um painel gráfico interativo, para visualizar métricas de forma clara. | 21 | 4 | RF23 | Feito |
| 24 | Média | Como administrador, quero aplicar filtros nos relatórios, para analisar por período, técnico ou categoria. | 13 | 4 | RF24 | Feito |
| 25 | Média | Como usuário, quero avaliar o atendimento recebido, para fornecer feedback. | 8 | 4 | RF25 | Feito |
| 26 | Média | Como administrador, quero analisar métricas de satisfação, para acompanhar a qualidade do suporte. | 13 | 4 | RF26 | Feito |

---

### 🔒 Requisitos Não Funcionais (RNF e RS)

| Rank | Prioridade | User Story | Story Points | Sprint | Requisito do Cliente | Status |
|:----:|:----------:|------------|--------------|:------:|:--------------------:|:------:|
| 27 | Alta | Como usuário, quero que o sistema seja acessado por HTTPS, para garantir segurança. | 8 | Todas | RNF01 | Feito |
| 28 | Alta | Como usuário, quero uma interface intuitiva e acessível, para navegar com facilidade. | 13 | Todas | RNF02 | Feito |
| 29 | Alta | Como administrador, quero que o sistema faça backups automáticos diários, para garantir integridade dos dados. | 8 | Todas | RNF03 | Feito |
| 30 | Média | Como administrador, quero logs de auditoria de usuários e chamados, para rastrear atividades. | 13 | Todas | RNF04 | Feito |
| 31 | Alta | Como usuário, quero que anexos sejam armazenados de forma segura, para proteger informações sensíveis. | 8 | Todas | RNF05 | Feito |
| 32 | Média | Como usuário, quero receber notificações por e-mail rapidamente, para acompanhar eventos do sistema. | 5 | Todas | RNF06 | Feito |
| 33 | Alta | Como desenvolvedor, quero que o sistema use MySQL como banco de dados relacional, para estruturar os dados. | 13 | Base | RS01 | Feito |
| 34 | Alta | Como desenvolvedor, quero um serviço de fila para e-mails e notificações, para garantir envio assíncrono. | 8 | Base | RS02 | Feito |
| 35 | Média | Como desenvolvedor, quero um serviço de armazenamento para anexos, para manter arquivos organizados. | 8 | Base | RS03 | Feito |
| 36 | Alta | Como desenvolvedor, quero integrar um módulo de IA, para classificar e sugerir soluções em chamados. | 21 | Base | RS04 | Feito |
| 37 | Alta | Como desenvolvedor, quero que o sistema rode em ambiente compatível, para garantir estabilidade. | 8 | Base | RS05 | Feito |
| 38 | Alta | Como desenvolvedor, quero utilizar um framework de backend web, para estruturar a aplicação. | 13 | Base | RS06 | Feito |
| 39 | Alta | Como desenvolvedor, quero utilizar um framework frontend moderno, para entregar boa experiência ao usuário. | 13 | Base | RS07 | Feito |
| 40 | Alta | Como desenvolvedor, quero um sistema de permissões baseado em roles, para controlar acessos. | 13 | Base | RS08 | Feito |
