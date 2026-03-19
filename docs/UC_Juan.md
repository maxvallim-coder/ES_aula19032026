## UC01 — Realizar Login

### Ator Principal
Usuário

### Objetivo
Permitir que o usuário acesse o sistema.

### Pré-condições
- Usuário deve possuir cadastro ativo.

### Pós-condições
- Sessão iniciada com sucesso.

### Fluxo Principal
1. O usuário informa e-mail e senha.
2. O sistema valida as credenciais.
3. O sistema autentica o usuário e redireciona para a tela inicial.

### Fluxos Alternativos
- **A1 — Senha incorreta:**  
O sistema exibe mensagem de erro.

- **A2 — Conta bloqueada:**  
O sistema impede o login.

### RF Relacionados
- RF01

### RNF Relacionados
- RNF01

### RN Relacionadas
- RN01

---

## UC02 — Realizar Matrícula de Aluno

### Ator Principal
Recepcionista

### Objetivo
Cadastrar um novo aluno no sistema.

### Pré-condições
- Recepcionista autenticado no sistema.

### Pós-condições
- Aluno cadastrado com sucesso.

### Fluxo Principal
1. Recepcionista acessa cadastro de alunos.
2. Recepcionista informa dados do aluno.
3. Sistema valida as informações.
4. Sistema registra aluno.

### Fluxos Alternativos
- **A1 — Dados incompletos:**  
Sistema solicita preenchimento dos campos obrigatórios.

### RF Relacionados
- RF02

### RNF Relacionados
- RNF01

### RN Relacionadas
- RN02

---

## UC03 — Atualizar Cadastro de Aluno

### Ator Principal
Recepcionista

### Objetivo
Atualizar dados de um aluno.

### Pré-condições
- Aluno cadastrado.

### Pós-condições
- Dados atualizados.

### Fluxo Principal
1. Recepcionista busca aluno.
2. Sistema exibe dados.
3. Recepcionista altera informações.
4. Sistema salva alterações.

### Fluxos Alternativos
- **A1 — Aluno não encontrado**

### RF Relacionados
- RF03

### RNF Relacionados
- RNF02

### RN Relacionadas
- RN02

---

## UC04 — Contratar Plano

### Ator Principal
Recepcionista

### Objetivo
Associar um plano ao aluno.

### Pré-condições
- Aluno cadastrado.

### Pós-condições
- Plano registrado.

### Fluxo Principal
1. Recepcionista seleciona aluno.
2. Sistema mostra planos disponíveis.
3. Recepcionista escolhe plano.
4. Sistema registra contratação.

### Fluxos Alternativos
- **A1 — Plano indisponível**

### RF Relacionados
- RF04

### RNF Relacionados
- RNF01

### RN Relacionadas
- RN03

---

## UC05 — Registrar Pagamento

### Ator Principal
Recepcionista

### Objetivo
Registrar pagamento do aluno.

### Pré-condições
- Plano ativo.

### Pós-condições
- Pagamento registrado.

### Fluxo Principal
1. Recepcionista seleciona aluno.
2. Recepcionista informa pagamento.
3. Sistema registra transação.

### Fluxos Alternativos
- **A1 — Pagamento inválido**

### RF Relacionados
- RF05

### RNF Relacionados
- RNF02

### RN Relacionadas
- RN04

---

## UC06 — Liberar Acesso na Catraca

### Ator Principal
Sistema de Catraca

### Objetivo
Controlar entrada de alunos.

### Pré-condições
- Aluno com plano ativo.

### Pós-condições
- Acesso liberado ou negado.

### Fluxo Principal
1. Aluno aproxima cartão RFID.
2. Sistema verifica plano.
3. Catraca libera acesso.

### Fluxos Alternativos
- **A1 — Plano vencido**

### RF Relacionados
- RF06

### RNF Relacionados
- RNF01

### RN Relacionadas
- RN05

---

## UC07 — Agendar Aula

### Ator Principal
Aluno

### Objetivo
Reservar vaga em aula.

### Pré-condições
- Plano ativo.

### Pós-condições
- Aula agendada.

### Fluxo Principal
1. Aluno acessa agenda.
2. Seleciona aula.
3. Sistema registra reserva.

### Fluxos Alternativos
- **A1 — Aula lotada**

### RF Relacionados
- RF07

### RNF Relacionados
- RNF01

### RN Relacionadas
- RN06

---

## UC08 — Cancelar Agendamento

### Ator Principal
Aluno

### Objetivo
Cancelar reserva de aula.

### Pré-condições
- Aula agendada.

### Pós-condições
- Reserva cancelada.

### Fluxo Principal
1. Aluno acessa agendamentos.
2. Seleciona aula.
3. Sistema cancela reserva.

### Fluxos Alternativos
- **A1 — Prazo de cancelamento expirado**

### RF Relacionados
- RF08

### RNF Relacionados
- RNF01

### RN Relacionadas
- RN07

---

## UC09 — Registrar Presença em Aula

### Ator Principal
Instrutor

### Objetivo
Registrar presença dos alunos.

### Pré-condições
- Aula iniciada.

### Pós-condições
- Presença registrada.

### Fluxo Principal
1. Instrutor acessa lista.
2. Marca presença.
3. Sistema salva registro.

### Fluxos Alternativos
- **A1 — Aluno não inscrito**

### RF Relacionados
- RF09

### RNF Relacionados
- RNF01

### RN Relacionadas
- RN08

---

## UC10 — Registrar Avaliação Física

### Ator Principal
Instrutor

### Objetivo
Registrar avaliação física do aluno.

### Pré-condições
- Aluno cadastrado.

### Pós-condições
- Avaliação salva.

### Fluxo Principal
1. Instrutor seleciona aluno.
2. Insere dados físicos.
3. Sistema registra avaliação.

### Fluxos Alternativos
- **A1 — Dados inválidos**

### RF Relacionados
- RF10

### RNF Relacionados
- RNF02

### RN Relacionadas
- RN09

---

## UC11 — Consultar Avaliação Física

### Ator Principal
Aluno

### Objetivo
Consultar avaliações físicas.

### Fluxo Principal
1. Aluno acessa histórico.
2. Sistema exibe avaliações.

---

## UC12 — Gerar Relatório Financeiro

### Ator Principal
Gerente

### Objetivo
Gerar relatório financeiro.

### Fluxo Principal
1. Gerente seleciona relatório.
2. Sistema gera relatório.

---

## UC13 — Gerar Relatório de Matrículas

### Ator Principal
Gerente

### Objetivo
Visualizar número de matrículas.

### Fluxo Principal
1. Gerente solicita relatório.
2. Sistema exibe dados.

---

## UC14 — Gerenciar Planos

### Ator Principal
Gerente

### Objetivo
Criar ou editar planos.

### Fluxo Principal
1. Gerente acessa planos.
2. Sistema permite edição.

---

## UC15 — Gerenciar Instrutores

### Ator Principal
Gerente

### Objetivo
Cadastrar instrutores.

### Fluxo Principal
1. Gerente cadastra instrutor.
2. Sistema registra.

---

## UC16 — Consultar Frequência

### Ator Principal
Gerente

### Objetivo
Consultar frequência de alunos.

### Fluxo Principal
1. Gerente acessa relatório.
2. Sistema mostra frequência.

---

## UC17 — Validar Pagamento

### Ator Principal
Sistema

### Objetivo
Verificar status de pagamento.

### Fluxo Principal
1. Sistema consulta pagamento.
2. Sistema valida status.

---

## UC18 — Consultar Agenda de Aulas

### Ator Principal
Aluno

### Objetivo
Visualizar agenda.

### Fluxo Principal
1. Aluno acessa agenda.
2. Sistema exibe aulas.

---

## UC19 — Cancelar Plano

### Ator Principal
Recepcionista

### Objetivo
Cancelar plano de aluno.

### Fluxo Principal
1. Recepcionista seleciona aluno.
2. Sistema cancela plano.

---

## UC20 — Gerar Relatório de Frequência

### Ator Principal
Gerente

### Objetivo
Gerar relatório de frequência.

### Fluxo Principal
1. Gerente solicita relatório.
2. Sistema gera relatório.

---

# Diagrama de Casos de Uso

![Diagrama](DUC_01_Juan.png)