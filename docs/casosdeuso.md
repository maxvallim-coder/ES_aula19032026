# Casos de Uso – Sistema FitPass Gym Management
<img width="427" height="856" alt="image" src="https://github.com/user-attachments/assets/aa36c995-484e-4ef5-bf26-52141728aafd" />

<img width="418" height="1051" alt="image" src="https://github.com/user-attachments/assets/1a63db0c-63e5-4754-8683-8e34383a3111" />


## UC01 — Realizar Login

<img width="509" height="325" alt="image" src="https://github.com/user-attachments/assets/9f9040fd-fb5f-4b28-b32f-70b5f0a445c0" />


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
- RNF02

### RN Relacionadas
- RN06


## UC02 — Cadastrar Aluno

<img width="269" height="445" alt="image" src="https://github.com/user-attachments/assets/578624f1-a4be-4929-8785-bb191c608ebb" />


### Ator Principal
Recepcionista

### Objetivo
Cadastrar novos alunos no sistema.

### Pré-condições
- Usuário deve estar logado.

### Pós-condições
- Aluno cadastrado com sucesso.

### Fluxo Principal
1. O recepcionista acessa a tela de cadastro.
2. Preenche os dados do aluno.
3. O sistema valida os dados.
4. O sistema salva o cadastro.

### Fluxos Alternativos
- **A1 — Dados inválidos:**  
  O sistema solicita correção.

### RF Relacionados
- RF01

### RNF Relacionados
- RNF04

### RN Relacionadas
- RN06


## UC03 — Gerenciar Planos

<img width="547" height="536" alt="image" src="https://github.com/user-attachments/assets/e0c4489e-c29f-4e99-bf57-489a30451371" />

### Ator Principal
Gerente

### Objetivo
Criar e gerenciar planos da academia.

### Pré-condições
- Usuário autenticado como gerente.

### Pós-condições
- Plano atualizado no sistema.

### Fluxo Principal
1. O gerente acessa a área de planos.
2. Cria ou edita um plano.
3. Salva as alterações.

### Fluxos Alternativos
- **A1 — Dados inválidos:**  
  O sistema exibe erro.

### RF Relacionados
- RF02

### RNF Relacionados
- RNF04

### RN Relacionadas
- RN06


## UC04 — Registrar Pagamento

<img width="401" height="447" alt="image" src="https://github.com/user-attachments/assets/16ba4869-284b-4e1d-afd4-3eb252218d5f" />

### Ator Principal
Recepcionista

### Objetivo
Registrar pagamento do aluno.

### Pré-condições
- Aluno cadastrado.

### Pós-condições
- Pagamento registrado e status atualizado.

### Fluxo Principal
1. O recepcionista seleciona o aluno.
2. Informa o método de pagamento.
3. Confirma a operação.

### Fluxos Alternativos
- **A1 — Pagamento parcial:**  
  O sistema bloqueia operação.

### RF Relacionados
- RF03

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN04, RN07


## UC05 — Verificar Regularidade

<img width="445" height="227" alt="image" src="https://github.com/user-attachments/assets/71d7c2f5-8dd6-4755-9809-a4b102480131" />


### Ator Principal
Sistema

### Objetivo
Verificar se o aluno está em dia.

### Pré-condições
- Aluno cadastrado.

### Pós-condições
- Status atualizado.

### Fluxo Principal
1. O sistema verifica data de pagamento.
2. Define status do aluno.

### Fluxos Alternativos
- **A1 — Inadimplente:**  
  Sistema marca como irregular.

### RF Relacionados
- RF04

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN01


## UC06 — Validar Acesso na Catraca

<img width="320" height="450" alt="image" src="https://github.com/user-attachments/assets/ca5183d2-cd85-42ef-9abb-9ed87fa0632f" />


### Ator Principal
Sistema

### Objetivo
Controlar entrada do aluno.

### Pré-condições
- Aluno com RFID.

### Pós-condições
- Acesso liberado ou negado.

### Fluxo Principal
1. Aluno aproxima RFID.
2. Sistema valida status.
3. Libera entrada.

### Fluxos Alternativos
- **A1 — Inadimplente:**  
  Acesso negado.

### RF Relacionados
- RF05

### RNF Relacionados
- RNF06

### RN Relacionadas
- RN01


## UC07 — Agendar Aula

<img width="453" height="615" alt="image" src="https://github.com/user-attachments/assets/3ec49778-e997-42fa-9c81-5ac424f8c281" />


### Ator Principal
Aluno

### Objetivo
Reservar vaga em aula.

### Pré-condições
- Aluno ativo.

### Pós-condições
- Aula agendada.

### Fluxo Principal
1. Aluno visualiza horários.
2. Seleciona aula.
3. Confirma reserva.

### Fluxos Alternativos
- **A1 — Lotação máxima:**  
  Sistema bloqueia.

### RF Relacionados
- RF06

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN02


## UC08 — Cancelar Agendamento

### Ator Principal
Aluno

### Objetivo
Cancelar aula agendada.

### Pré-condições
- Aula previamente agendada.

### Pós-condições
- Vaga liberada.

### Fluxo Principal
1. Aluno acessa agendamentos.
2. Cancela aula.

### Fluxos Alternativos
- **A1 — Fora do prazo:**  
  Sistema impede cancelamento.

### RF Relacionados
- RF06

### RNF Relacionados
- RNF04

### RN Relacionadas
- RN03


## UC09 — Registrar Presença

### Ator Principal
Instrutor

### Objetivo
Registrar presença dos alunos.

### Pré-condições
- Aula em andamento.

### Pós-condições
- Presença registrada.

### Fluxo Principal
1. Instrutor acessa lista.
2. Marca presença.

### Fluxos Alternativos
- **A1 — Aluno não listado:**  
  Sistema bloqueia.

### RF Relacionados
- RF07

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN06


## UC10 — Registrar Avaliação Física

### Ator Principal
Instrutor

### Objetivo
Registrar dados físicos do aluno.

### Pré-condições
- Aluno ativo.

### Pós-condições
- Avaliação salva.

### Fluxo Principal
1. Instrutor insere dados.
2. Salva avaliação.

### Fluxos Alternativos
- **A1 — Aluno irregular:**  
  Sistema bloqueia.

### RF Relacionados
- RF08

### RNF Relacionados
- RNF02

### RN Relacionadas
- RN05


## UC11 — Emitir Relatórios

<img width="264" height="282" alt="image" src="https://github.com/user-attachments/assets/8a981836-af9e-4da3-927c-01b967fc8ae4" />


### Ator Principal
Gerente

### Objetivo
Gerar relatórios gerenciais.

### Pré-condições
- Dados disponíveis.

### Pós-condições
- Relatório exibido.

### Fluxo Principal
1. Seleciona tipo de relatório.
2. Sistema gera resultado.

### Fluxos Alternativos
- **A1 — Sem dados:**  
  Exibe mensagem.

### RF Relacionados
- RF09

### RNF Relacionados
- RNF05

### RN Relacionadas
- RN06


## UC12 — Enviar Notificação

<img width="553" height="917" alt="image" src="https://github.com/user-attachments/assets/04cbe5cc-624a-4854-98f7-69ab9a164b4f" />


### Ator Principal
Sistema

### Objetivo
Notificar aluno.

### Pré-condições
- Evento disparado.

### Pós-condições
- Notificação enviada.

### Fluxo Principal
1. Sistema identifica evento.
2. Envia mensagem.

### Fluxos Alternativos
- **A1 — Falha envio:**  
  Reenvio automático.

### RF Relacionados
- RF10

### RNF Relacionados
- RNF01

### RN Relacionadas
- RN07


## UC13 — Atualizar Cadastro

### Ator Principal
Aluno

### Objetivo
Atualizar dados pessoais.

### Pré-condições
- Login realizado.

### Pós-condições
- Dados atualizados.

### Fluxo Principal
1. Edita informações.
2. Salva alterações.

### Fluxos Alternativos
- **A1 — Dados inválidos:**  
  Solicita correção.

### RF Relacionados
- RF01

### RNF Relacionados
- RNF04

### RN Relacionadas
- RN06


## UC14 — Consultar Planos

### Ator Principal
Aluno

### Objetivo
Visualizar planos disponíveis.

### Pré-condições
- Sistema ativo.

### Pós-condições
- Lista exibida.

### Fluxo Principal
1. Acessa área de planos.
2. Visualiza opções.

### Fluxos Alternativos
- **A1 — Nenhum plano:**  
  Exibe mensagem.

### RF Relacionados
- RF02

### RNF Relacionados
- RNF04

### RN Relacionadas
- RN06


## UC15 — Gerar Boleto

### Ator Principal
Sistema

### Objetivo
Gerar cobrança.

### Pré-condições
- Mensalidade ativa.

### Pós-condições
- Boleto gerado.

### Fluxo Principal
1. Sistema cria cobrança.
2. Disponibiliza ao aluno.

### Fluxos Alternativos
- **A1 — Falha:**  
  Reprocessa.

### RF Relacionados
- RF03

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN04


## UC16 — Consultar Histórico

### Ator Principal
Aluno

### Objetivo
Ver histórico de acessos.

### Pré-condições
- Login ativo.

### Pós-condições
- Dados exibidos.

### Fluxo Principal
1. Acessa histórico.
2. Visualiza dados.

### Fluxos Alternativos
- **A1 — Sem histórico:**  
  Exibe mensagem.

### RF Relacionados
- RF09

### RNF Relacionados
- RNF05

### RN Relacionadas
- RN06


## UC17 — Gerenciar Permissões

### Ator Principal
Gerente

### Objetivo
Controlar acessos.

### Pré-condições
- Perfil gerente.

### Pós-condições
- Permissões atualizadas.

### Fluxo Principal
1. Seleciona usuário.
2. Define permissões.

### Fluxos Alternativos
- **A1 — Perfil inválido:**  
  Exibe erro.

### RF Relacionados
- RF01

### RNF Relacionados
- RNF02

### RN Relacionadas
- RN06


## UC18 — Visualizar Agenda

### Ator Principal
Aluno

### Objetivo
Ver aulas disponíveis.

### Pré-condições
- Sistema ativo.

### Pós-condições
- Agenda exibida.

### Fluxo Principal
1. Acessa agenda.
2. Visualiza horários.

### Fluxos Alternativos
- **A1 — Sem aulas:**  
  Exibe aviso.

### RF Relacionados
- RF06

### RNF Relacionados
- RNF04

### RN Relacionadas
- RN02


## UC19 — Atualizar Status do Aluno

### Ator Principal
Sistema

### Objetivo
Atualizar situação automaticamente.

### Pré-condições
- Pagamento registrado.

### Pós-condições
- Status atualizado.

### Fluxo Principal
1. Detecta pagamento.
2. Atualiza status.

### Fluxos Alternativos
- **A1 — Falha:**  
  Reprocessa.

### RF Relacionados
- RF04

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN07


## UC20 — Integrar com Catraca

### Ator Principal
Sistema

### Objetivo
Comunicar com hardware.

### Pré-condições
- API ativa.

### Pós-condições
- Comunicação realizada.

### Fluxo Principal
1. Sistema envia requisição.
2. Recebe resposta.

### Fluxos Alternativos
- **A1 — Falha comunicação:**  
  Sistema tenta novamente.

### RF Relacionados
- RF05

### RNF Relacionados
- RNF06

### RN Relacionadas
- RN01
