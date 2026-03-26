# UC01 — Realizar Login

## Ator Principal
- **Usuário**

## Objetivo
- Permitir que o usuário acesse o sistema.

## Pré-condições
- Usuário deve possuir cadastro ativo.

## Pós-condições
- Sessão iniciada com sucesso.

## Fluxo Principal
1. O usuário informa e-mail e senha.
2. O sistema valida as credenciais.
3. O sistema autentica o usuário e redireciona para a tela inicial.

## Fluxos Alternativos
- **A1 — Senha incorreta**  
  O sistema exibe mensagem de erro.

- **A2 — Conta bloqueada**  
  O sistema impede o login.

## Requisitos Funcionais Relacionados
- **RF01**

## Requisitos Não Funcionais Relacionados
- **RNF02**

## Regras de Negócio Relacionadas
- **RN06**

## Diagrama
<img width="271" height="323" alt="image" src="https://github.com/user-attachments/assets/044590aa-f9c3-4e60-a77f-67ac83308386" />


# UC02 — Cadastrar Aluno

## Ator Principal
- **Recepcionista**

## Objetivo
- Cadastrar novos alunos no sistema.

## Pré-condições
- Usuário deve estar autenticado.

## Pós-condições
- Aluno cadastrado com sucesso.

## Fluxo Principal
1. Recepcionista acessa o módulo de cadastro.
2. Preenche dados do aluno.
3. Seleciona plano.
4. Sistema valida informações.
5. Sistema salva o cadastro.

## Fluxos Alternativos
- **A1 — Dados inválidos**  
  O sistema exibe erro.

## Requisitos Funcionais Relacionados
- **RF01**

## Requisitos Não Funcionais Relacionados
- **RNF04**

## Regras de Negócio Relacionadas
- **RN06**


## Diagrama
<img width="222" height="382" alt="image" src="https://github.com/user-attachments/assets/0cd9135c-1878-405d-b975-06ef5c04de43" />



# UC03 — Registrar Pagamento

## Ator Principal
- **Recepcionista**

## Objetivo
- Registrar o pagamento da mensalidade do aluno.

## Pré-condições
- Aluno deve estar cadastrado.

## Pós-condições
- Pagamento registrado e status atualizado.

## Fluxo Principal
1. Recepcionista seleciona aluno.
2. Informa forma de pagamento.
3. Sistema registra pagamento.
4. Sistema atualiza situação do aluno.

## Fluxos Alternativos
- **A1 — Falha no pagamento**  
  O sistema exibe erro.

## Requisitos Funcionais Relacionados
- **RF03**

## Requisitos Não Funcionais Relacionados
- **RNF03**

## Regras de Negócio Relacionadas
- **RN04**
- **RN07**

## Diagrama
<img width="153" height="318" alt="image" src="https://github.com/user-attachments/assets/707b5965-7342-47e9-ba78-b8d42b65846f" />



# UC04 — Validar Acesso na Catraca

## Ator Principal
- **Sistema**

## Objetivo
- Permitir ou bloquear entrada do aluno na academia.

## Pré-condições
- Aluno deve possuir RFID cadastrado.

## Pós-condições
- Acesso liberado ou negado.

## Fluxo Principal
1. Aluno aproxima RFID.
2. Sistema verifica cadastro.
3. Sistema verifica regularidade.
4. Sistema libera entrada.

## Fluxos Alternativos
- **A1 — Aluno inadimplente**  
  Acesso negado.

- **A2 — RFID inválido**  
  Acesso negado.

## Requisitos Funcionais Relacionados
- **RF04**
- **RF05**

## Requisitos Não Funcionais Relacionados
- **RNF03**
- **RNF06**

## Regras de Negócio Relacionadas
- **RN01**


## Diagrama
<img width="377" height="328" alt="image" src="https://github.com/user-attachments/assets/b1349fde-a58e-492d-9b99-f16d3ed873d7" />



# UC05 — Agendar Aula

## Ator Principal
- **Aluno**

## Objetivo
- Permitir que o aluno reserve uma vaga em aula.

## Pré-condições
- Aluno deve estar ativo.

## Pós-condições
- Aula agendada.

## Fluxo Principal
1. Aluno acessa agenda.
2. Visualiza horários.
3. Seleciona aula.
4. Sistema confirma reserva.

## Fluxos Alternativos
- **A1 — Vagas esgotadas**  
  Sistema impede agendamento.

## Requisitos Funcionais Relacionados
- **RF06**

## Requisitos Não Funcionais Relacionados
- **RNF04**

## Regras de Negócio Relacionadas
- **RN02**
- **RN03**

## Diagrama
<img width="266" height="323" alt="image" src="https://github.com/user-attachments/assets/348b911f-1c4b-4fc9-9549-5257f204dfe1" />



# UC06 — Registrar Avaliação Física

## Ator Principal
- **Instrutor**

## Objetivo
- Registrar dados físicos do aluno.

## Pré-condições
- Aluno deve estar ativo e regular.

## Pós-condições
- Avaliação salva no sistema.

## Fluxo Principal
1. Instrutor seleciona aluno.
2. Registra dados físicos.
3. Sistema salva avaliação.

## Fluxos Alternativos
- **A1 — Aluno irregular**  
  Sistema impede registro.

## Requisitos Funcionais Relacionados
- **RF08**

## Requisitos Não Funcionais Relacionados
- **RNF02**

## Regras de Negócio Relacionadas
- **RN05**

## Diagrama
<img width="271" height="323" alt="image" src="https://github.com/user-attachments/assets/d04148a1-e224-4575-b59d-915cf7df73f3" />

