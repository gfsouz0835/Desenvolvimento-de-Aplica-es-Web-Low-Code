# OrganizaTarefas

Sistema web para gestão de tarefas com priorização automática por prazo.

---

## Problema

Equipes perdem prazos por usarem registros espalhados e comunicação fragmentada. A ausência de um fluxo único de acompanhamento gera falta de visibilidade, priorização subjetiva e perda de prazos.

---

## Funcionalidades

- **Cadastro de tarefas** com nome, prazo e descrição
- **Prioridade automática** por prazo (Alta, Média, Baixa)
- **Listagem** com busca por nome e filtro por status
- **Ações** de editar, excluir, iniciar e concluir
- **Dashboard** com indicadores e gráficos

---

## Arquitetura

A aplicação segue a **Arquitetura Canvas** do OutSystems:

| Camada | Responsabilidade |
|---|---|
| **Interface** | Telas Novo, Lista e Painel + Client Actions |
| **Core** | Server Actions (SalvarTarefa, ExcluirTarefa, CriarTarefaExemplo) + Entidade Tarefa |
| **Foundation** | Serviços de infraestrutura (e-mail, usuário, cadastros) |

---

## Tecnologias Utilizadas

- **OutSystems** (plataforma de desenvolvimento low-code)
- **OutSystemsUI** (componentes de interface)
- **Charts** (gráficos do dashboard)
- **Maps** (componentes de mapas)

---

## Recurso de IA/Automação

A **prioridade automática por prazo** é definida na Server Action **SalvarTarefa**:

| Prazo | Prioridade |
|---|---|
| Até 3 dias | **Alta** |
| 4 a 7 dias | **Média** |
| Acima de 7 dias | **Baixa** |

---

## Prints


| Tela | Descrição |
|---|---|
| **Novo** | Formulário de cadastro |
<img width="1661" height="594" alt="NOVO" src="https://github.com/user-attachments/assets/e6e77381-92fe-45d8-a061-57a3a5458071" />
| **Painel** | Dashboard com indicadores |
<img width="1696" height="838" alt="dashboard" src="https://github.com/user-attachments/assets/8403096b-201e-4f37-976e-5c40018a6a94" />

| **Lista** | Tabela com tarefas e ações |
<img width="1886" height="814" alt="lista" src="https://github.com/user-attachments/assets/2f70842a-2b11-437b-a998-9872f7a8998c" />


## Server Actions
SalvarTarefa

<img width="1317" height="796" alt="salvartarefa" src="https://github.com/user-attachments/assets/08887ffc-a170-4b29-b4dd-464afc6cc1ac" />

criartarefa
<img width="1319" height="816" alt="criartarefa" src="https://github.com/user-attachments/assets/3a3ece76-9bc1-463b-9ea3-9d162a73cdcb" />

excluirtarefa
<img width="1312" height="572" alt="excluirtarefa" src="https://github.com/user-attachments/assets/dd30ad18-ec59-4199-8446-3235cf35f782" />


---

## Instruções para Testar

1. Acesse o link da aplicação
2. Na tela **Novo**, cadastre uma tarefa com prazo de 2 dias (prioridade **Alta**)
3. Cadastre outra tarefa com prazo de 5 dias (prioridade **Média**)
4. Cadastre uma terceira tarefa com prazo de 10 dias (prioridade **Baixa**)
5. Na tela **Lista**, utilize os filtros e ações
6. Na tela **Painel**, visualize os indicadores e gráficos

---

## Link da Aplicação

`https://personal-tlmophnh-dev.outsystems.app/OrganizaTarefas/`
