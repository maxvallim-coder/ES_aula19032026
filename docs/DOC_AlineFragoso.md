<img width="777" height="230" alt="image" src="https://github.com/user-attachments/assets/10f55d49-018c-4482-b6a0-25962a5a0960" />

# UC01 — Realizar Login

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

---
<img width="777" height="146" alt="image" src="https://github.com/user-attachments/assets/e11e6c02-62e5-4ba7-9313-b8e8d0d21de8" />

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

---
<img width="777" height="194" alt="image" src="https://github.com/user-attachments/assets/1112208d-8729-49a6-8ba6-dbf8bb807659" />

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

---
<img width="777" height="114" alt="image" src="https://github.com/user-attachments/assets/ec3c053c-e536-4604-a6c9-5328a837914d" />

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

---
<img width="777" height="146" alt="image" src="https://github.com/user-attachments/assets/544e8d3d-4def-47e4-af43-c7d67c5333a5" />

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

---
<img width="777" height="51" alt="image" src="https://github.com/user-attachments/assets/d40f333e-5a94-45d2-b9ef-48b89825ef3f" />

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

---
<img width="777" height="108" alt="image" src="https://github.com/user-attachments/assets/ef214a87-e1cf-4b70-9689-0af237774eec" />

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

---
<img width="777" height="114" alt="image" src="https://github.com/user-attachments/assets/ae3932a6-f584-43fd-ac57-db932b9fb7d8" />

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

---
<img width="777" height="97" alt="image" src="https://github.com/user-attachments/assets/a8c5dca8-79ac-42c2-bd28-c75177a0a3a2" />

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

---
<img width="777" height="146" alt="image" src="https://github.com/user-attachments/assets/9d1dd7bc-c2e5-4563-bdd7-4f0a67122d56" />

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

---
<img width="777" height="114" alt="image" src="https://github.com/user-attachments/assets/f9a5e8e7-b764-47a6-85a3-b7920a2cc2f3" />

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

---
<img width="777" height="116" alt="image" src="https://github.com/user-attachments/assets/a35f3090-11f9-4201-8448-a3397b65cd60" />

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

---
<img width="777" height="112" alt="image" src="https://github.com/user-attachments/assets/c6fdbe87-63f8-43c0-992a-796a252acd2b" />

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

---
<img width="777" height="114" alt="image" src="https://github.com/user-attachments/assets/56719281-12e4-4ede-b349-79da0a833759" />

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

---
<img width="777" height="114" alt="image" src="https://github.com/user-attachments/assets/f08c7cac-7f65-436e-badc-84261ef6ca3f" />

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

---
<img width="777" height="71" alt="image" src="https://github.com/user-attachments/assets/b7f2cd59-7733-47da-a80d-7255dee65114" />

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

---
<img width="777" height="99" alt="image" src="https://github.com/user-attachments/assets/263656f8-d10f-447e-a954-52bc73ca9f1d" />

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

---
<img width="777" height="115" alt="image" src="https://github.com/user-attachments/assets/77b9728b-0883-4669-a947-6df67aa0bfbf" />

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

---
<img width="777" height="83" alt="image" src="https://github.com/user-attachments/assets/0eb948af-8a93-426d-b3bf-9f3b53fd6f9d" />

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

---
