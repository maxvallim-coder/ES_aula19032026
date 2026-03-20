# <img width="1600" height="265" alt="DUC01_AlineFragoso_GraziellyZambello_AnthonyFerreira" src="https://github.com/user-attachments/assets/febc6668-7131-42bd-830a-9afcb76d6ce7" />
<img width="1600" height="158" alt="DUC02_AlineFragoso_GraziellyZambello_AnthonyFerreira" src="https://github.com/user-attachments/assets/4c3bc530-83ad-4ee4-9249-8dbe275c9617" />
UC01 — Realizar Login

### Ator Principal

Usuário

### Objetivo

Permitir que o usuário acesse o sistema.

### Pré-condições

* Usuário deve possuir cadastro ativo.

### Pós-condições

* Sessão iniciada com sucesso.

### Fluxo Principal

1. O usuário informa e-mail e senha.
2. O sistema valida as credenciais.
3. O sistema autentica o usuário e redireciona para a tela inicial.

### Fluxos Alternativos

**A1 — Senha incorreta**
O sistema exibe mensagem de erro.

**A2 — Conta bloqueada**
O sistema impede o login e instrui o usuário a recuperar o acesso.

### RF Relacionados

RF01 — O sistema deve permitir autenticação de usuários.

### RNF Relacionados

RNF01 — O sistema deve garantir segurança no processo de autenticação.

### RN Relacionadas

RN01 — Apenas usuários cadastrados podem acessar o sistema.
<img width="793" height="465" alt="Captura de tela 2026-03-19 202246" src="https://github.com/user-attachments/assets/e87e1bb5-b09d-4058-84f3-18f64ac7d764" />

---

# UC02 — Cadastrar Aluno

### Ator Principal

Recepcionista

### Objetivo

Registrar um novo aluno no sistema.

### Pré-condições

* Recepcionista autenticado no sistema.

### Pós-condições

* Aluno cadastrado com sucesso.

### Fluxo Principal

1. Recepcionista acessa a opção cadastrar aluno.
2. Sistema solicita os dados do aluno.
3. Recepcionista preenche as informações.
4. Sistema valida os dados.
5. Sistema salva o cadastro.

### Fluxos Alternativos

**A1 — CPF já cadastrado**
O sistema exibe mensagem informando que o CPF já está registrado.

### RF Relacionados

RF02 — O sistema deve permitir cadastro de alunos.

### RNF Relacionados

RNF02 — O sistema deve validar integridade dos dados cadastrados.

### RN Relacionadas

RN02 — Cada aluno deve possuir CPF único.
<img width="792" height="494" alt="Captura de tela 2026-03-19 202422" src="https://github.com/user-attachments/assets/b886c7d0-fe7a-42d9-9dc1-50a2f5ed52fb" />

---

# UC03 — Atualizar Dados do Aluno

### Ator Principal

Recepcionista

### Objetivo

Permitir a atualização das informações cadastrais do aluno.

### Pré-condições

* Aluno deve estar cadastrado no sistema.

### Pós-condições

* Dados do aluno atualizados.

### Fluxo Principal

1. Recepcionista busca o aluno no sistema.
2. Sistema exibe os dados cadastrados.
3. Recepcionista altera as informações necessárias.
4. Sistema valida os dados.
5. Sistema salva as alterações.

### Fluxos Alternativos

**A1 — Aluno não encontrado**
Sistema informa que o aluno não está cadastrado.

### RF Relacionados

RF03 — O sistema deve permitir atualização de cadastro de alunos.

### RNF Relacionados

RNF02 — O sistema deve validar consistência dos dados.

### RN Relacionadas

RN02 — O CPF do aluno deve permanecer único.
<img width="793" height="445" alt="Captura de tela 2026-03-19 202532" src="https://github.com/user-attachments/assets/b0f2725e-e202-4960-870c-b61425cea8d0" />

---

# UC04 — Realizar Matrícula

### Ator Principal

Recepcionista

### Objetivo

Registrar matrícula do aluno em um plano da academia.

### Pré-condições

* Aluno cadastrado.
* Plano disponível.

### Pós-condições

* Matrícula registrada no sistema.

### Fluxo Principal

1. Recepcionista seleciona o aluno.
2. Sistema apresenta os planos disponíveis.
3. Recepcionista escolhe o plano.
4. Sistema registra a matrícula.

### Fluxos Alternativos

**A1 — Plano indisponível**
Sistema informa que o plano não está disponível.

### RF Relacionados

RF04 — O sistema deve permitir matrícula de alunos em planos.

### RNF Relacionados

RNF01 — O sistema deve responder às ações do usuário rapidamente.

### RN Relacionadas

RN03 — Todo aluno deve possuir plano ativo para utilizar a academia.
<img width="756" height="565" alt="Captura de tela 2026-03-19 202616" src="https://github.com/user-attachments/assets/683e0487-17f6-4068-a67b-a7b631d253a3" />

---

# UC05 — Cancelar Matrícula

### Ator Principal

Recepcionista

### Objetivo

Cancelar matrícula de aluno.

### Pré-condições

* Matrícula ativa.

### Pós-condições

* Matrícula cancelada.

### Fluxo Principal

1. Recepcionista localiza matrícula.
2. Seleciona opção cancelar.
3. Sistema solicita confirmação.
4. Sistema cancela matrícula.

### Fluxos Alternativos

**A1 — Matrícula inexistente**
Sistema informa erro.

### RF Relacionados

RF05 — O sistema deve permitir cancelamento de matrículas.

### RNF Relacionados

RNF01 — O sistema deve responder rapidamente às solicitações.

### RN Relacionadas

RN03 — Apenas matrículas ativas podem ser canceladas.
<img width="792" height="437" alt="Captura de tela 2026-03-19 202651" src="https://github.com/user-attachments/assets/80d8601b-429e-43b2-b82b-06c9eb219512" />

---

# UC06 — Registrar Pagamento

### Ator Principal

Recepcionista

### Objetivo

Registrar pagamento de mensalidade.

### Pré-condições

* Aluno matriculado.

### Pós-condições

* Pagamento registrado no sistema.

### Fluxo Principal

1. Recepcionista acessa pagamentos pendentes.
2. Seleciona pagamento.
3. Informa forma de pagamento.
4. Sistema registra pagamento.

### Fluxos Alternativos

**A1 — Pagamento recusado**
Sistema solicita nova tentativa.

### RF Relacionados

RF06 — O sistema deve registrar pagamentos de mensalidades.

### RNF Relacionados

RNF03 — O sistema deve garantir segurança nas transações financeiras.

### RN Relacionadas

RN04 — Pagamentos devem ser registrados antes da liberação de acesso.
<img width="726" height="557" alt="Captura de tela 2026-03-19 202741" src="https://github.com/user-attachments/assets/8c7ffba2-e75f-4d72-885d-7433e34f3611" />

---

# UC07 — Renovar Plano

### Ator Principal

Recepcionista

### Objetivo

Renovar plano do aluno.

### Pré-condições

* Plano próximo do vencimento.

### Pós-condições

* Nova validade registrada.

### Fluxo Principal

1. Recepcionista seleciona o plano do aluno.
2. Sistema gera nova cobrança.
3. Sistema atualiza validade do plano.

### Fluxos Alternativos

**A1 — Pagamento não confirmado**
Sistema cancela renovação.

### RF Relacionados

RF07 — O sistema deve permitir renovação de planos.

### RNF Relacionados

RNF03 — O sistema deve proteger dados financeiros.

### RN Relacionadas

RN04 — Renovação depende da confirmação do pagamento.
<img width="794" height="512" alt="Captura de tela 2026-03-19 202832" src="https://github.com/user-attachments/assets/a7bd4e25-bda3-4694-8a00-7169d19b813b" />

---

# UC08 — Validar Acesso na Catraca

### Ator Principal

Sistema de Catraca

### Objetivo

Controlar acesso de alunos à academia.

### Pré-condições

* Aluno cadastrado.

### Pós-condições

* Acesso liberado ou negado.

### Fluxo Principal

1. Aluno aproxima cartão RFID.
2. Sistema consulta status da matrícula.
3. Sistema libera acesso.

### Fluxos Alternativos

**A1 — Aluno inadimplente**
Sistema bloqueia acesso.

### RF Relacionados

RF08 — O sistema deve validar acesso pela catraca.

### RNF Relacionados

RNF04 — O sistema deve integrar com API da catraca.

### RN Relacionadas

RN05 — Apenas alunos com matrícula ativa podem acessar.
<img width="792" height="381" alt="Captura de tela 2026-03-19 202918" src="https://github.com/user-attachments/assets/402c0f2e-2bf7-444c-a678-9e5ec0742b14" />

---

# UC09 — Agendar Aula

### Ator Principal

Aluno

### Objetivo

Permitir que o aluno reserve uma vaga em uma aula.

### Pré-condições

* Aluno ativo.
* Aula disponível.

### Pós-condições

* Aula agendada com sucesso.

### Fluxo Principal

1. Aluno acessa a agenda de aulas.
2. Seleciona a aula desejada.
3. Sistema registra o agendamento.

### Fluxos Alternativos

**A1 — Aula cheia**
Sistema informa que a aula está lotada.

### RF Relacionados

RF09 — O sistema deve permitir agendamento de aulas.

### RNF Relacionados

RNF01 — O sistema deve responder rapidamente às ações do usuário.

### RN Relacionadas

RN06 — Cada aula possui limite de vagas.
<img width="784" height="449" alt="Captura de tela 2026-03-19 202957" src="https://github.com/user-attachments/assets/97a429f3-d4ef-4ddb-bb75-aa183fd6ff0e" />

---

# UC10 — Cancelar Agendamento

### Ator Principal

Aluno

### Objetivo

Permitir que o aluno cancele um agendamento de aula.

### Pré-condições

* Aula previamente agendada.

### Pós-condições

* Agendamento cancelado.

### Fluxo Principal

1. Aluno acessa a agenda.
2. Seleciona aula agendada.
3. Confirma cancelamento.
4. Sistema remove o agendamento.

### Fluxos Alternativos

**A1 — Prazo de cancelamento expirado**
Sistema informa que não é possível cancelar.

### RF Relacionados

RF10 — O sistema deve permitir cancelamento de aulas.

### RNF Relacionados

RNF01 — Sistema deve responder rapidamente.

### RN Relacionadas

RN06 — Respeitar limite de vagas e regras de cancelamento.
<img width="790" height="438" alt="Captura de tela 2026-03-19 203040" src="https://github.com/user-attachments/assets/26f03579-39fa-4e4c-9867-e1f461e69079" />

---

# UC11 — Registrar Presença em Aula

### Ator Principal

Instrutor

### Objetivo

Registrar presença dos alunos em uma aula.

### Pré-condições

* Aula em andamento.
* Instrutor autenticado.

### Pós-condições

* Presença registrada no sistema.

### Fluxo Principal

1. Instrutor acessa lista de alunos.
2. Marca presença de cada aluno.
3. Sistema confirma registro.

### Fluxos Alternativos

**A1 — Aluno não encontrado**
Sistema solicita verificação do aluno.

### RF Relacionados

RF11 — O sistema deve registrar presença em aulas.

### RNF Relacionados

RNF01 — Sistema deve registrar informações rapidamente.

### RN Relacionadas

RN07 — Presença só pode ser registrada pelo instrutor da aula.
<img width="621" height="424" alt="Captura de tela 2026-03-19 203120" src="https://github.com/user-attachments/assets/e3962120-6740-4eff-a6a0-00abcec4661d" />

---

# UC12 — Registrar Avaliação Física

### Ator Principal

Instrutor

### Objetivo

Registrar avaliação física do aluno.

### Pré-condições

* Aluno cadastrado.
* Instrutor autenticado.

### Pós-condições

* Avaliação registrada no sistema.

### Fluxo Principal

1. Instrutor seleciona aluno.
2. Preenche dados da avaliação física.
3. Sistema salva a avaliação.

### Fluxos Alternativos

**A1 — Dados inválidos**
Sistema solicita correção dos dados.

### RF Relacionados

RF12 — O sistema deve permitir registro de avaliação física.

### RNF Relacionados

RNF01 — Sistema deve armazenar dados de forma segura.

### RN Relacionadas

RN08 — Avaliações só podem ser registradas por instrutores.
<img width="704" height="507" alt="Captura de tela 2026-03-19 203225" src="https://github.com/user-attachments/assets/6ffec358-91f1-473c-ac8a-e74cf92d5de9" />

---

# UC13 — Consultar Histórico do Aluno

### Ator Principal

Instrutor

### Objetivo

Permitir consulta ao histórico de atividades e avaliações do aluno.

### Pré-condições

* Aluno cadastrado.

### Pós-condições

* Histórico exibido.

### Fluxo Principal

1. Instrutor busca aluno.
2. Sistema apresenta histórico.

### Fluxos Alternativos

**A1 — Histórico inexistente**
Sistema informa que não há registros.

### RF Relacionados

RF13 — Sistema deve permitir consulta de histórico.

### RNF Relacionados

RNF01 — Sistema deve apresentar informações rapidamente.

### RN Relacionadas

RN09 — Histórico deve ser mantido pelo sistema.
<img width="720" height="387" alt="Captura de tela 2026-03-19 203330" src="https://github.com/user-attachments/assets/4ddeda93-ecf5-419b-939b-f2f96e108f8d" />

---

# UC14 — Criar Plano

### Ator Principal

Gerente

### Objetivo

Criar novo plano de academia.

### Pré-condições

* Gerente autenticado.

### Pós-condições

* Plano criado e disponível para matrícula.

### Fluxo Principal

1. Gerente insere dados do plano.
2. Sistema valida informações.
3. Sistema salva o plano.

### Fluxos Alternativos

**A1 — Dados incompletos**
Sistema solicita completar os dados.

### RF Relacionados

RF14 — Sistema deve permitir criação de planos.

### RNF Relacionados

RNF01 — Sistema deve validar integridade dos dados.

### RN Relacionadas

RN10 — Planos devem ter valor e duração definidos.
<img width="716" height="393" alt="Captura de tela 2026-03-19 203419" src="https://github.com/user-attachments/assets/17cc6764-2215-4d49-8e6b-34a0a039f501" />

---

# UC15 — Atualizar Plano

### Ator Principal

Gerente

### Objetivo

Atualizar informações de um plano existente.

### Pré-condições

* Plano existente.

### Pós-condições

* Plano atualizado.

### Fluxo Principal

1. Gerente seleciona plano.
2. Atualiza informações.
3. Sistema salva alterações.

### Fluxos Alternativos

**A1 — Plano não encontrado**
Sistema informa erro.

### RF Relacionados

RF15 — Sistema deve permitir atualização de planos.

### RNF Relacionados

RNF01 — Sistema deve manter consistência dos dados.

### RN Relacionadas

RN10 — Alterações devem seguir regras do plano.
<img width="795" height="501" alt="Captura de tela 2026-03-19 203510" src="https://github.com/user-attachments/assets/53f50284-f6c2-4ab0-8005-df3ae7010021" />

---

# UC16 — Excluir Plano

### Ator Principal

Gerente

### Objetivo

Excluir plano da academia.

### Pré-condições

* Plano existente.
* Nenhum aluno ativo no plano.

### Pós-condições

* Plano removido.

### Fluxo Principal

1. Gerente seleciona plano.
2. Confirma exclusão.
3. Sistema remove o plano.

### Fluxos Alternativos

**A1 — Plano possui alunos ativos**
Sistema bloqueia exclusão.

### RF Relacionados

RF16 — Sistema deve permitir exclusão de planos.

### RNF Relacionados

RNF01 — Sistema deve proteger dados sensíveis.

### RN Relacionadas

RN10 — Planos ativos não podem ser excluídos.
<img width="793" height="400" alt="Captura de tela 2026-03-19 203553" src="https://github.com/user-attachments/assets/28760eee-0d82-4927-945b-0761d3f298ac" />

---

# UC17 — Gerar Relatório de Alunos

### Ator Principal

Gerente

### Objetivo

Gerar relatório completo de alunos cadastrados.

### Pré-condições

* Gerente autenticado.

### Pós-condições

* Relatório disponível para visualização ou download.

### Fluxo Principal

1. Gerente acessa menu de relatórios.
2. Seleciona relatório de alunos.
3. Sistema gera relatório.

### RF Relacionados

RF17 — Sistema deve gerar relatórios de alunos.

### RNF Relacionados

RNF02 — Relatórios devem ser gerados em tempo adequado.

### RN Relacionadas

RN11 — Apenas gerentes podem acessar relatórios.
<img width="436" height="329" alt="Captura de tela 2026-03-19 203626" src="https://github.com/user-attachments/assets/46c94654-a2df-4020-92f8-9c53cce583b2" />

---

# UC18 — Gerar Relatório Financeiro

### Ator Principal

Gerente

### Objetivo

Gerar relatório financeiro detalhado.

### Pré-condições

* Gerente autenticado.

### Pós-condições

* Relatório disponível.

### Fluxo Principal

1. Gerente acessa menu financeiro.
2. Seleciona período e tipo de relatório.
3. Sistema gera relatório financeiro.

### Fluxos Alternativos

**A1 — Sem registros**
Sistema informa que não há dados.

### RF Relacionados

RF18 — Sistema deve gerar relatórios financeiros.

### RNF Relacionados

RNF02 — Sistema deve processar relatórios rapidamente.

### RN Relacionadas

RN11 — Apenas gerentes podem acessar dados financeiros.
<img width="792" height="411" alt="Captura de tela 2026-03-19 203703" src="https://github.com/user-attachments/assets/e951ade7-2d25-40ce-819c-0d07937859d8" />

---

# UC19 — Cadastrar Instrutor

### Ator Principal

Gerente

### Objetivo

Registrar um novo instrutor na academia.

### Pré-condições

* Gerente autenticado.

### Pós-condições

* Instrutor cadastrado com sucesso.

### Fluxo Principal

1. Gerente seleciona opção cadastrar instrutor.
2. Insere dados do instrutor.
3. Sistema valida e salva cadastro.

### Fluxos Alternativos

**A1 — CPF duplicado**
Sistema solicita correção do CPF.

### RF Relacionados

RF19 — Sistema deve permitir cadastro de instrutores.

### RNF Relacionados

RNF01 — Sistema deve validar dados inseridos.

### RN Relacionadas

RN12 — Instrutores devem ter dados profissionais completos.
<img width="683" height="448" alt="Captura de tela 2026-03-19 203743" src="https://github.com/user-attachments/assets/dcec977d-27c0-4a4f-a9a7-c097c943fcb4" />

---

# UC20 — Consultar Agenda de Aulas

### Ator Principal

Aluno

### Objetivo

Visualizar a agenda de aulas disponíveis.

### Pré-condições

* Aluno ativo.

### Pós-condições

* Agenda exibida com horários e vagas disponíveis.

### Fluxo Principal

1. Aluno acessa agenda de aulas.
2. Sistema exibe aulas e horários disponíveis.

### Fluxos Alternativos

**A1 — Aula lotada**
Sistema indica que a aula está cheia.

### RF Relacionados

RF20 — Sistema deve exibir agenda de aulas.

### RNF Relacionados

RNF01 — Sistema deve responder rapidamente.

### RN Relacionadas

RN06 — Limite de vagas deve ser respeitado.
<img width="691" height="340" alt="Captura de tela 2026-03-19 203825" src="https://github.com/user-attachments/assets/5b779a5c-7458-40d1-93ee-967bb2b13084" />

---
