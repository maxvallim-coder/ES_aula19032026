<img width="336" height="326" alt="image" src="https://github.com/user-attachments/assets/63474de6-ff8b-4199-9e65-1f72e1f8d750" />

<img width="417" height="110" alt="image" src="https://github.com/user-attachments/assets/b8e6dd81-7a19-497c-9f1b-73ae78fbd50d" />

<img width="416" height="523" alt="image" src="https://github.com/user-attachments/assets/484a4874-9790-41e6-a265-ecbfef378afb" />

<img width="357" height="345" alt="image" src="https://github.com/user-attachments/assets/5256269e-c262-4635-8860-a92de069caf7" />

<img width="436" height="482" alt="image" src="https://github.com/user-attachments/assets/0f083c32-d60c-48fc-8557-1bd5d6225bcf" />

<img width="352" height="243" alt="image" src="https://github.com/user-attachments/assets/fae8b75b-8c93-4454-b116-cdd99e8eefe1" />


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
  O sistema impede o login e instrui o usuário a recuperar o acesso.

### RF Relacionados
- RF04

### RNF Relacionados
- RNF02
- RNF04

### RN Relacionadas
- RN06

<img width="1111" height="514" alt="image" src="https://github.com/user-attachments/assets/deba27c1-53cb-4b34-a1d4-314bb1e987db" />

## UC02 — Cadastrar Aluno 

### Ator Principal
Recepcionista

### Objetivo
Registrar novo aluno no sistema.

### Pré-condições
- Recepcionista autenticado.

### Pós-condições
- Aluno cadastrado e ativo.

### Fluxo Principal
1. Recepcionista acessa a tela de cadastro.
2. Informa dados pessoais e contato.
3. Seleciona plano.
4. Sistema valida dados.
5. Sistema salva cadastro.

### Fluxos Alternativos
- **A1 — Dados obrigatórios não informados:**  
  Sistema solicita preenchimento.

- **A2 — CPF já cadastrado:**  
  Sistema impede duplicidade.

### RF Relacionados
- RF01

### RNF Relacionados
- RNF02
- RNF04

### RN Relacionadas
- RN06
<img width="1104" height="617" alt="image" src="https://github.com/user-attachments/assets/4faf28b7-a81e-4ab8-956d-324ea22d28ed" />


## UC03 — Gerenciar Planos

### Ator Principal
Gerente

### Objetivo
Criar, editar, ativar ou desativar planos.

### Pré-condições
- Gerente autenticado.

### Pós-condições
- Plano atualizado.

### Fluxo Principal
1. Gerente acessa módulo de planos.
2. Seleciona ação desejada.
3. Informa dados do plano.
4. Sistema valida informações.
5. Sistema salva alterações.

### Fluxos Alternativos
- **A1 — Dados incompletos:**  
  Sistema impede salvamento.

- **A2 — Plano em uso por alunos:**  
  Sistema impede exclusão e sugere desativação.

### RF Relacionados
- RF02

### RNF Relacionados
- RNF05

### RN Relacionadas
- RN06
<img width="1309" height="757" alt="image" src="https://github.com/user-attachments/assets/f10ddcf6-3e74-4d75-b0bc-53fefb732a80" />


## UC04 — Registrar Pagamento

### Ator Principal
Recepcionista

### Objetivo
Registrar pagamento de mensalidade.

### Pré-condições
- Aluno cadastrado.

### Pós-condições
- Situação financeira atualizada.

### Fluxo Principal
1. Recepcionista seleciona aluno.
2. Informa forma de pagamento.
3. Confirma valor integral.
4. Sistema registra pagamento.
5. Sistema atualiza regularidade.

### Fluxos Alternativos
- **A1 — Valor incorreto:**  
  Sistema impede confirmação.

- **A2 — Falha na transação:**  
  Sistema cancela operação e solicita nova tentativa.

### RF Relacionados
- RF03

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN04
- RN07

<img width="737" height="702" alt="image" src="https://github.com/user-attachments/assets/d110d778-14c5-45a5-a595-6fb07cc64f2b" />

## UC05 — Verificar Regularidade do Aluno

### Ator Principal
Sistema

### Objetivo
Determinar se o aluno está apto.

### Pré-condições
- Aluno cadastrado.

### Pós-condições
- Status atualizado.

### Fluxo Principal
1. Sistema consulta pagamentos.
2. Verifica vencimentos.
3. Define situação como regular ou irregular.

### Fluxos Alternativos
- **A1 —Mensalidade vencida:**  
  Aluno marcado como inadimplente.

- **A2 —Dados financeiros indisponíveis:**  
 Sistema registra erro e mantém status anterior.

### RF Relacionados
- RF04

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN01
<img width="596" height="401" alt="image" src="https://github.com/user-attachments/assets/5cd70f95-9afe-4bca-bce9-c048206fd0e4" />


## UC06 — Validar Acesso na Catraca

### Ator Principal
Sistema de Catraca

### Objetivo
Permitir ou bloquear entrada.

### Pré-condições
- Aluno identificado por RFID.

### Pós-condições
- Entrada registrada ou negada.

### Fluxo Principal
1. Catraca envia identificação ao sistema.
2. Sistema verifica regularidade.
3. Sistema autoriza acesso.
4. Catraca libera entrada.

### Fluxos Alternativos
- **A1 —Aluno inadimplente:**  
  Acesso negado.

- **A2 —Falha de comunicação com API:**  
 Catraca permanece bloqueada.

### RF Relacionados
- RF05

### RNF Relacionados
- RNF03
- RNF06

### RN Relacionadas
- RN01

<img width="912" height="509" alt="image" src="https://github.com/user-attachments/assets/2676ee52-250a-4a1a-8927-02cca986d11e" />

## UC07 — Visualizar Aulas Disponíveis

### Ator Principal
Aluno

### Objetivo
Consultar horários de aulas.

### Pré-condições
- Aluno autenticado.

### Pós-condições
- Lista exibida.

### Fluxo Principal
1. Aluno acessa área de aulas.
2. Sistema apresenta horários disponíveis.


### Fluxos Alternativos
- **A1 — Nenhuma aula disponível:**  
  Sistema informa indisponibilidade.

- **A2 — Falha na consulta:**  
  Sistema exibe mensagem de erro.

### RF Relacionados
- RF06

### RNF Relacionados
- RNF04

### RN Relacionadas
- Nenhuma
 
<img width="782" height="374" alt="image" src="https://github.com/user-attachments/assets/e19e6452-e7eb-4779-aa29-8d5ccd20dbef" />

## UC08 — Agendar Aula

### Ator Principal
Aluno

### Objetivo
Reservar vaga em aula.

### Pré-condições
- Aluno regular.

### Pós-condições
- Reserva confirmada.

### Fluxo Principal
1. Aluno seleciona aula.
2. Sistema verifica vagas.
3. Sistema registra reserva.


### Fluxos Alternativos
- **A1 — Aula lotada:**  
  Reserva bloqueada.

- **A2 — Aluno irregular:**  
  Sistema impede agendamento

### RF Relacionados
- RF06

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN02

<img width="605" height="484" alt="image" src="https://github.com/user-attachments/assets/e193000d-42ce-4869-9527-dfec685396e7" />

## UC09 — Cancelar Agendamento

### Ator Principal
Aluno

### Objetivo
Cancelar reserva.

### Pré-condições
- Agendamento existente.

### Pós-condições
- Vaga liberada.

### Fluxo Principal
1. Aluno acessa agendamentos.
2. Seleciona aula.
3. Confirma cancelamento.
4. Sistema remove reserva.


### Fluxos Alternativos
- **A1 — Prazo expirado:**  
  Cancelamento bloqueado.

- **A2 — Agendamento inexistente:**  
  Sistema informa erro.

### RF Relacionados
- RF06

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN03

<img width="762" height="579" alt="image" src="https://github.com/user-attachments/assets/a48d902c-4ac0-4b88-8303-b723d40e6259" />

## UC10 — Registrar Presença em Aula

### Ator Principal
Instrutor

### Objetivo
Confirmar presença dos alunos.

### Pré-condições
- Aula em andamento.

### Pós-condições
- Lista atualizada.

### Fluxo Principal
1. Instrutor acessa lista da aula.
2. Marca presença dos alunos.
3. Sistema salva registros.


### Fluxos Alternativos
- **A1 — Aluno não inscrito:**  
  Sistema impede marcação.

- **A2 — Falha ao salvar:**  
  Sistema solicita nova tentativa.

### RF Relacionados
- RF07

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN06

<img width="774" height="592" alt="image" src="https://github.com/user-attachments/assets/a22823e0-1c8a-4c5c-918a-4c7ffb0808fb" />

## UC11 — Registrar Avaliação Física

### Ator Principal
Instrutor

### Objetivo
Cadastrar dados físicos.

### Pré-condições
- Aluno regular.

### Pós-condições
- Avaliação registrada.

### Fluxo Principal
1. Instrutor seleciona aluno.
2. Informa medidas físicas.
3. Anexa arquivos.
4. Sistema salva avaliação.


### Fluxos Alternativos
- **A1 — Aluno irregular:**  
  Avaliação bloqueada.

- **A2 — Dados inválidos:**  
  Sistema solicita correção.

### RF Relacionados
- RF08

### RNF Relacionados
- RNF02

### RN Relacionadas
- RN05

<img width="908" height="619" alt="image" src="https://github.com/user-attachments/assets/15017044-06b7-4ef9-af64-a2596d2eca74" />

## UC12 — Consultar Avaliações Físicas

### Ator Principal
Instrutor

### Objetivo
Visualizar histórico.

### Pré-condições
- Avaliações registradas.

### Pós-condições
- Dados exibidos.

### Fluxo Principal
1. Instrutor seleciona aluno.
2. Sistema exibe histórico.


### Fluxos Alternativos
- **A1 — Nenhuma avaliação encontrada:**  
  Sistema informa ausência de dados.

- **A2 — Falha na consulta:**  
  Sistema exibe erro.

### RF Relacionados
- RF08

### RNF Relacionados
- RNF04

### RN Relacionadas
- Nenhuma

<img width="866" height="449" alt="image" src="https://github.com/user-attachments/assets/bc65e089-ecb5-4bc6-9dbb-84a89f431c92" />


## UC13 — Emitir Relatório de Inadimplência

### Ator Principal
Gerente

### Objetivo
Identificar alunos inadimplentes.

### Pré-condições
- Gerente autenticado.

### Pós-condições
- Relatório gerado.

### Fluxo Principal
1. Gerente solicita relatório.
2. Sistema processa dados.
3. Sistema exibe resultado.

### Fluxos Alternativos
- **A1 — Nenhum aluno inadimplente:**  
  Sistema informa ausência.

- **A2 — Falha na geração:**  
  Sistema exibe erro.

### RF Relacionados
- RF09

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN01

<img width="891" height="374" alt="image" src="https://github.com/user-attachments/assets/86497839-62e1-430f-91a5-f86d329452ff" />

## UC14 — Emitir Relatório de Alunos Ativos

### Ator Principal
Gerente

### Objetivo
Listar alunos ativos.

### Pré-condições
- Gerente autenticado.

### Pós-condições
- Relatório exibido.

### Fluxo Principal
1. Gerente solicita relatório.
2. Sistema gera lista.


### Fluxos Alternativos
- **A1 — Nenhum aluno ativo:**  
  Sistema informa ausência.

- **A2 — Falha na consulta:**  
  Sistema exibe erro.

### RF Relacionados
- RF09

### RNF Relacionados
- RNF03

### RN Relacionadas
- Nenhuma

<img width="842" height="374" alt="image" src="https://github.com/user-attachments/assets/4212b23c-b930-44bc-8ed9-d262df7bd63f" />

## UC15 — Emitir Relatório de Acessos

### Ator Principal
Gerente

### Objetivo
Consultar histórico de entradas.

### Pré-condições
- Registros existentes.

### Pós-condições
- Relatório exibido.

### Fluxo Principal
1. Gerente solicita relatório.
2. Sistema compila dados.
3. Exibe histórico.

### Fluxos Alternativos
- **A1 — Nenhum acesso registrado:**  
  Sistema informa ausência.

- **A2 — Falha na consulta:**  
  Sistema exibe erro.

### RF Relacionados
- RF09

### RNF Relacionados
- RNF03

### RN Relacionadas
- Nenhuma

<img width="861" height="374" alt="image" src="https://github.com/user-attachments/assets/e704da87-b744-43da-90de-d478b72e8c6d" />

## UC16 — Emitir Relatório de Ocupação de Aulas

### Ator Principal
Gerente

### Objetivo
Avaliar demanda das aulas.

### Pré-condições
- Aulas registradas.

### Pós-condições
- Relatório exibido.

### Fluxo Principal
1. Gerente solicita relatório.
2. Sistema analisa reservas.
3. Exibe ocupação.

### Fluxos Alternativos
- **A1 — Nenhuma aula cadastrada:**  
  Sistema informa ausência.

- **A2 — Falha na geração:**  
  Sistema exibe erro.

### RF Relacionados
- RF09

### RNF Relacionados
- RNF05

### RN Relacionadas
- RN02

<img width="671" height="444" alt="image" src="https://github.com/user-attachments/assets/2232ab13-a2fe-442f-97a9-71cddfd9baaa" />

## UC17 — Enviar Notificação de Vencimento

### Ator Principal
Sistema

### Objetivo
Avisar sobre mensalidade.

### Pré-condições
- Mensalidade próxima do vencimento.

### Pós-condições
- Notificação enviada.

### Fluxo Principal
1. Sistema identifica vencimento.
2. Gera notificação.
3. Envia ao aluno.


### Fluxos Alternativos
- **A1 — Falha no envio:**  
  Sistema agenda nova tentativa.

- **A2 — Dados de contato inválidos:**  
  Sistema exibe erro.

### RF Relacionados
- RF010

### RNF Relacionados
- RNF01

### RN Relacionadas
- Nenhuma

<img width="575" height="331" alt="image" src="https://github.com/user-attachments/assets/d0283ee6-4e0f-40ab-9bc3-dfeb0861a831" />

## UC18 — Enviar Confirmação de Agendamento

### Ator Principal
Sistema

### Objetivo
Confirmar reserva.

### Pré-condições
- Agendamento realizado.

### Pós-condições
- Aluno notificado.

### Fluxo Principal
1. Sistema registra agendamento.
2. Envia confirmação.

### Fluxos Alternativos
- **A1 — Falha no envio:**  
  Sistema agenda reenvio.

- **A2 — Agendamento cancelado antes do envio:**  
  Notificação não enviada.

### RF Relacionados
- RF010

### RNF Relacionados
- RNF01

### RN Relacionadas
- Nenhuma
<img width="784" height="524" alt="image" src="https://github.com/user-attachments/assets/e8d19cca-437d-471e-92d1-205d39d45787" />


## UC19 — Enviar Notificação de Avaliação Disponível

### Ator Principal
Sistema

### Objetivo
Avisar liberação de avaliação.

### Pré-condições
- Nova avaliação permitida.

### Pós-condições
- Aluno informado.

### Fluxo Principal
1. Sistema verifica elegibilidade.
2. Envia notificação.

### Fluxos Alternativos
- **A1 — Falha no envio:**  
  Sistema agenda nova tentativa.

- **A2 — Aluno sem contato cadastrado:**  
  Sistema registra erro.

### RF Relacionados
- RF010

### RNF Relacionados
- RNF01

### RN Relacionadas
- Nenhuma
- 
<img width="482" height="276" alt="image" src="https://github.com/user-attachments/assets/384f92d0-cfdf-467f-adf6-9839853589fa" />


## UC20 — Atualizar Situação do Aluno

### Ator Principal
Sistema

### Objetivo
Manter status atualizado.

### Pré-condições
- Pagamento registrado.

### Pós-condições
- Situação regularizada.

### Fluxo Principal
1. Sistema recebe confirmação de pagamento.
2. Atualiza status do aluno.


### Fluxos Alternativos
- **A1 — Falha na atualização:**  
  Sistema mantém status anterior.

- **A2 — Pagamento inconsistente:**  
  Sistema solicita verificação manual.

### RF Relacionados
- RF04

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN07
<img width="538" height="371" alt="image" src="https://github.com/user-attachments/assets/5373ca35-1ee1-4399-8b51-dc9e5227872e" />

