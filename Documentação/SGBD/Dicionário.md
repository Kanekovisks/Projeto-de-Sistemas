# Dicionário de Dados – Sistema HighTask

---

## Tabela: Usuarios

Id: INT, Primary Key, Auto Increment, Not Null
→ Identificador único do usuário

Nome: NVARCHAR(100), Not Null
→ Nome completo do usuário

Email: NVARCHAR(100), Unique, Not Null
→ E-mail do usuário (não pode ser duplicado)

Senha: NVARCHAR(100), Not Null
→ Senha do usuário (criptografada)

Perfil: NVARCHAR(50), Not Null
→ Perfil de acesso (admin, técnico, usuário)

Status: BIT, Not Null
→ Ativo (1) ou Inativo (0)



---

## Tabela: Chamados

Id: INT, Primary Key, Auto Increment, Not Null
→ Identificador único do chamado

Titulo: NVARCHAR(100), Not Null
→ Título do chamado

Descricao: NVARCHAR(500), Not Null
→ Descrição detalhada do problema

Status: NVARCHAR(50), Not Null
→ Status do chamado (Aberto, Em Atendimento, Resolvido, Fechado)

Prioridade: NVARCHAR(50), Not Null
→ Prioridade (Baixa, Média, Alta, Crítica)

DataAbertura: DATETIME, Not Null, Default GETDATE()
→ Data e hora da abertura do chamado

CategoriaId: INT, Foreign Key → Categorias(Id)
→ Categoria do chamado

UsuarioCriadorId: INT, Foreign Key → Usuarios(Id)
→ Usuário que criou o chamado

TecnicoResponsavelId: INT, Foreign Key → Usuarios(Id)
→ Técnico responsável pelo chamado



---

## Tabela: Categorias

Id: INT, Primary Key, Auto Increment, Not Null
→ Identificador da categoria

Nome: NVARCHAR(100), Not Null
→ Nome da categoria



---

## Tabela: Observacoes

Id: INT, Primary Key, Auto Increment, Not Null
→ Identificador da observação

ChamadoId: INT, Foreign Key → Chamados(Id)
→ Chamado associado à observação

AutorId: INT, Foreign Key → Usuarios(Id)
→ Técnico que realizou a observação

Texto: NVARCHAR(500), Not Null
→ Descrição da observação feita

TempoGasto: INT, Not Null
→ Tempo gasto na atividade (em minutos)

DataHora: DATETIME, Not Null, Default GETDATE()
→ Data e hora da observação



---

## Tabela: Relatorios

Id: INT, Primary Key, Auto Increment, Not Null
→ Identificador do relatório

Tipo: NVARCHAR(50), Not Null
→ Tipo do relatório (Chamados, Satisfação, Desempenho, etc.)

DataInicio: DATE, Not Null
→ Data inicial do período do relatório

DataFim: DATE, Not Null
→ Data final do período do relatório

Dados: NVARCHAR(MAX), Not Null
→ Dados do relatório (pode ser JSON ou texto estruturado)



---

## Tabela: Avaliacoes

Id: INT, Primary Key, Auto Increment, Not Null
→ Identificador da avaliação

ChamadoId: INT, Foreign Key → Chamados(Id)
→ Chamado avaliado

UsuarioId: INT, Foreign Key → Usuarios(Id)
→ Usuário que fez a avaliação

Nota: INT, Not Null
→ Nota de 1 a 5 atribuída pelo usuário

Comentario: NVARCHAR(500), Nullable
→ Comentário opcional sobre a avaliação



---

## Tabela: Auditoria

Id: INT, Primary Key, Auto Increment, Not Null
→ Identificador da entrada no log

UsuarioId: INT, Foreign Key → Usuarios(Id)
→ Usuário que realizou a ação

Acao: NVARCHAR(100), Not Null
→ Descrição resumida da ação realizada (ex.: "Criou Chamado")

DataHora: DATETIME, Not Null, Default GETDATE()
→ Data e hora da ação registrada

Descricao: NVARCHAR(500), Not Null
→ Detalhamento da ação realizada



---

## Tabela: Anexos

Id: INT, Primary Key, Auto Increment, Not Null
→ Identificador do anexo

ChamadoId: INT, Foreign Key → Chamados(Id)
→ Chamado ao qual o anexo está vinculado

NomeArquivo: NVARCHAR(255), Not Null
→ Nome do arquivo enviado

Caminho: NVARCHAR(500), Not Null
→ Caminho onde o arquivo está armazenado (pasta, servidor ou URL de nuvem)

DataUpload: DATETIME, Not Null, Default GETDATE()
→ Data e hora do envio do anexo



---

## Observações:

Todas as tabelas possuem uma chave primária (PK) e os relacionamentos são feitos através de chaves estrangeiras (FK).

Campos com Auto Increment (AI) são preenchidos automaticamente.

Campos NOT NULL não podem ser deixados em branco.

Para segurança, senhas devem ser armazenadas criptografadas e os anexos devem ter acesso controlado.

Logs de auditoria garantem rastreabilidade de todas as ações administrativas no sistema.



---
