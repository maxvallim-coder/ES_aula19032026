<img width="417" height="852" alt="image" src="https://github.com/user-attachments/assets/995ff5cb-7655-4ec3-ad5d-46134793039a" />
<img width="433" height="774" alt="image" src="https://github.com/user-attachments/assets/fdbaae93-1e4f-4bf2-8d21-205cf0e429d9" />


## UC01 --- Realizar Login 
<img width="750" height="668" alt="image" src="https://github.com/user-attachments/assets/b8045bb0-c9f2-4656-b9e6-fb10f0593bfa" />

### Ator Principal

Usuário

### Objetivo

Permitir que o usuário acesse o sistema.

### Pré-condições

-   Usuário deve possuir cadastro ativo.

### Pós-condições

-   Sessão iniciada com sucesso.

### Fluxo Principal

1.  O usuário informa e-mail e senha.
2.  O sistema valida as credenciais.
3.  O sistema autentica o usuário e redireciona para a tela inicial.

### Fluxos Alternativos

-   **A1 --- Senha incorreta:**\
    O sistema exibe mensagem de erro.

-   **A2 --- Conta bloqueada:**\
    O sistema impede o login e instrui o usuário a recuperar o acesso.

### RF Relacionados

-   RF01

### RNF Relacionados

-   RNF02, RNF04

### RN Relacionadas

-   Nenhuma

## UC02 --- Cadastrar Aluno
<img width="564" height="593" alt="image" src="https://github.com/user-attachments/assets/a658bbcf-11ac-40a5-be33-e4b969c44df9" />

### Ator Principal

Recepcionista

### Objetivo

Cadastrar um novo aluno no sistema.

### Pré-condições

-   Recepcionista autenticado no sistema.

### Pós-condições

-   Aluno cadastrado com sucesso.

### Fluxo Principal

1.  O recepcionista acessa a opção de cadastro de aluno.
2.  O sistema apresenta o formulário de cadastro.
3.  O recepcionista preenche dados pessoais, contato, endereço e plano
    contratado.
4.  O sistema valida os dados informados.
5.  O sistema salva o cadastro.

### Fluxos Alternativos

-   **A1 --- Dados obrigatórios não preenchidos:**\
    O sistema solicita o preenchimento dos campos obrigatórios.

### RF Relacionados

-   RF01

### RNF Relacionados

-   RNF02, RNF04

### RN Relacionadas

-   Nenhuma

## UC03 --- Atualizar Cadastro de Aluno
<img width="564" height="593" alt="image" src="https://github.com/user-attachments/assets/41dae493-9ce9-4984-a8de-8e87b2f42b3a" />

### Ator Principal

Recepcionista

### Objetivo

Atualizar informações de um aluno.

### Pré-condições

-   Aluno deve estar cadastrado.

### Pós-condições

-   Dados do aluno atualizados.

### Fluxo Principal

1.  O recepcionista busca o aluno.
2.  O sistema exibe os dados cadastrados.
3.  O recepcionista altera as informações necessárias.
4.  O sistema salva as alterações.

### Fluxos Alternativos

-   **A1 --- Aluno não encontrado:**\
    O sistema informa que o cadastro não existe.

### RF Relacionados

-   RF01

### RNF Relacionados

-   RNF02

### RN Relacionadas

-   Nenhuma

## UC04 --- Criar Plano
<img width="248" height="367" alt="image" src="https://github.com/user-attachments/assets/a0d8cafe-1275-4162-b755-2e54876289bb" />

### Ator Principal

Gerente

### Objetivo

Criar um novo tipo de plano.

### Pré-condições

-   Gerente autenticado no sistema.

### Pós-condições

-   Plano cadastrado no sistema.

### Fluxo Principal

1.  O gerente acessa a área de planos.
2.  O gerente seleciona a opção de criar novo plano.
3.  O gerente informa nome, duração e valor.
4.  O sistema salva o plano.

### Fluxos Alternativos

-   **A1 --- Dados inválidos:**\
    O sistema solicita correção dos dados.

### RF Relacionados

-   RF02

### RNF Relacionados

-   RNF04

### RN Relacionadas

-   Nenhuma

## UC05 --- Editar Plano
<img width="344" height="431" alt="image" src="https://github.com/user-attachments/assets/95ba0d8a-6943-48c4-8a8b-7a04c11b9aa1" />


### Ator Principal

Gerente

### Objetivo

Alterar informações de um plano existente.

### Pré-condições

-   Plano cadastrado.

### Pós-condições

-   Plano atualizado.

### Fluxo Principal

1.  O gerente seleciona um plano.
2.  O sistema exibe os dados do plano.
3.  O gerente altera as informações.
4.  O sistema salva as alterações.

### Fluxos Alternativos

-   **A1 --- Plano inexistente:**\
    O sistema informa erro.

### RF Relacionados

-   RF02

### RNF Relacionados

-   RNF04

### RN Relacionadas

-   Nenhuma

## UC06 --- Ativar Plano
<img width="211" height="312" alt="image" src="https://github.com/user-attachments/assets/8399fc9e-2955-41f7-b1bf-18381b264705" />

### Ator Principal

Gerente

### Objetivo

Disponibilizar um plano para contratação.

### Pré-condições

-   Plano cadastrado.

### Pós-condições

-   Plano ativo no sistema.

### Fluxo Principal

1.  O gerente seleciona um plano.
2.  O gerente escolhe ativar o plano.
3.  O sistema atualiza o status do plano.

### Fluxos Alternativos

-   **A1 --- Plano já ativo:**\
    O sistema informa que o plano já está ativo.

### RF Relacionados

-   RF02

### RNF Relacionados

-   RNF04

### RN Relacionadas

-   Nenhuma

## UC07 --- Desativar Plano
<img width="223" height="312" alt="image" src="https://github.com/user-attachments/assets/0a5e42cd-5a4b-44c2-b18f-79e1e39e8dff" />

### Ator Principal

Gerente

### Objetivo

Desativar um plano existente.

### Pré-condições

-   Plano ativo.

### Pós-condições

-   Plano indisponível para novos alunos.

### Fluxo Principal

1.  O gerente seleciona um plano ativo.
2.  O gerente escolhe desativar o plano.
3.  O sistema altera o status do plano.

### Fluxos Alternativos

-   **A1 --- Plano já desativado:**\
    O sistema informa que o plano já está desativado.

### RF Relacionados

-   RF02

### RNF Relacionados

-   RNF04

### RN Relacionadas

-   Nenhuma

## UC08 --- Registrar Pagamento
<img width="579" height="538" alt="image" src="https://github.com/user-attachments/assets/caf69781-823b-4a1c-a177-8f01b37e09d5" />

### Ator Principal

Recepcionista

### Objetivo

Registrar pagamento da mensalidade.

### Pré-condições

-   Aluno cadastrado.

### Pós-condições

-   Pagamento registrado.

### Fluxo Principal

1.  O recepcionista seleciona o aluno.
2.  O sistema exibe débitos pendentes.
3.  O recepcionista registra pagamento (dinheiro, cartão ou PIX).
4.  O sistema confirma a operação.

### Fluxos Alternativos

-   **A1 --- Pagamento recusado:**\
    O sistema informa falha no pagamento.

### RF Relacionados

-   RF03

### RNF Relacionados

-   RNF02

### RN Relacionadas

-   Nenhuma

## UC09 --- Gerar Boleto ou Pagamento Online
<img width="340" height="376" alt="image" src="https://github.com/user-attachments/assets/f2e4bb8d-ee53-44ca-bc16-071b90b434af" />

### Ator Principal

Sistema

### Objetivo

Gerar cobrança online para pagamento.

### Pré-condições

-   Aluno com mensalidade pendente.

### Pós-condições

-   Boleto ou link de pagamento gerado.

### Fluxo Principal

1.  O sistema identifica pagamento pendente.
2.  O sistema gera boleto ou link de pagamento.
3.  O sistema envia ao aluno.

### Fluxos Alternativos

-   **A1 --- Falha na geração:**\
    O sistema informa erro.

### RF Relacionados

-   RF03

### RNF Relacionados

-   RNF01, RNF03

### RN Relacionadas

-   Nenhuma

## UC10 --- Verificar Regularidade do Aluno
<img width="307" height="367" alt="image" src="https://github.com/user-attachments/assets/5442b7b0-c825-4f8f-a2b1-17ae5e8746f6" />

### Ator Principal

Sistema

### Objetivo

Verificar se o aluno está com mensalidade em dia.

### Pré-condições

-   Aluno cadastrado.

### Pós-condições

-   Status do aluno atualizado.

### Fluxo Principal

1.  O sistema consulta pagamentos do aluno.
2.  O sistema verifica vencimentos.
3.  O sistema atualiza o status do aluno.

### Fluxos Alternativos

-   **A1 --- Aluno inadimplente:**\
    O sistema marca o aluno como inadimplente.

### RF Relacionados

-   RF04

### RNF Relacionados

-   RNF03

### RN Relacionadas

-   Nenhuma

## UC11 --- Validar Entrada na Academia
<img width="786" height="435" alt="image" src="https://github.com/user-attachments/assets/c7b0e052-ba5d-493d-a74e-c374aafdccc8" />

### Ator Principal

Aluno

### Objetivo

Permitir acesso à academia pela catraca.

### Pré-condições

-   Aluno cadastrado e regular.

### Pós-condições

-   Entrada liberada na catraca.

### Fluxo Principal

1.  O aluno aproxima o cartão RFID da catraca.
2.  O sistema consulta o cadastro.
3.  O sistema verifica a regularidade do pagamento.
4.  O sistema libera a catraca.

### Fluxos Alternativos

-   **A1 --- Aluno inadimplente:**\
    O sistema bloqueia a entrada.

-   **A2 --- Cartão inválido:**\
    O sistema nega acesso.

### RF Relacionados

-   RF05

### RNF Relacionados

-   RNF03, RNF06

### RN Relacionadas

-   Nenhuma

## UC12 --- Visualizar Horários de Aulas
<img width="231" height="308" alt="image" src="https://github.com/user-attachments/assets/8b404218-3211-453a-aa09-44c031402210" />

### Ator Principal

Aluno

### Objetivo

Permitir que o aluno visualize aulas disponíveis.

### Pré-condições

-   Aluno autenticado no sistema.

### Pós-condições

-   Horários exibidos.

### Fluxo Principal

1.  O aluno acessa a área de aulas.
2.  O sistema exibe horários disponíveis.

### Fluxos Alternativos

-   **A1 --- Nenhuma aula disponível:**\
    O sistema informa ausência de aulas.

### RF Relacionados

-   RF06

### RNF Relacionados

-   RNF04

### RN Relacionadas

-   Nenhuma

## UC13 --- Reservar Aula
<img width="413" height="480" alt="image" src="https://github.com/user-attachments/assets/638d5edf-b03b-4c39-be61-400731091af4" />

### Ator Principal

Aluno

### Objetivo

Reservar vaga em uma aula.

### Pré-condições

-   Aluno ativo.

### Pós-condições

-   Vaga reservada.

### Fluxo Principal

1.  O aluno escolhe uma aula.
2.  O sistema verifica disponibilidade de vagas.
3.  O sistema registra a reserva.

### Fluxos Alternativos

-   **A1 --- Aula lotada:**\
    O sistema informa indisponibilidade.

### RF Relacionados

-   RF06

### RNF Relacionados

-   RNF03

### RN Relacionadas

-   Nenhuma

## UC14 --- Cancelar Reserva de Aula
<img width="327" height="362" alt="image" src="https://github.com/user-attachments/assets/9330cc2f-eaed-489e-ba63-7ce3e8621e1d" />

### Ator Principal

Aluno

### Objetivo

Cancelar reserva realizada.

### Pré-condições

-   Reserva existente.

### Pós-condições

-   Reserva removida.

### Fluxo Principal

1.  O aluno acessa suas reservas.
2.  O aluno seleciona cancelar reserva.
3.  O sistema confirma cancelamento.

### Fluxos Alternativos

-   **A1 --- Prazo de cancelamento expirado:**\
    O sistema impede o cancelamento.

### RF Relacionados

-   RF06

### RNF Relacionados

-   RNF04

### RN Relacionadas

-   Nenhuma

## UC15 --- Registrar Presença
<img width="326" height="362" alt="image" src="https://github.com/user-attachments/assets/559bdb84-e6e1-4772-bb6d-29c27f68276a" />

### Ator Principal

Instrutor

### Objetivo

Registrar presença dos alunos nas aulas.

### Pré-condições

-   Aula em andamento.

### Pós-condições

-   Presença registrada.

### Fluxo Principal

1.  O instrutor acessa a lista da aula.
2.  O instrutor marca presença dos alunos.
3.  O sistema salva os registros.

### Fluxos Alternativos

-   **A1 --- Aluno não reservado:**\
    O sistema informa inconsistência.

### RF Relacionados

-   RF07

### RNF Relacionados

-   RNF03

### RN Relacionadas

-   Nenhuma

## UC16 --- Registrar Avaliação Física
<img width="230" height="362" alt="image" src="https://github.com/user-attachments/assets/62214d4d-6c22-4f56-bef9-70e6e5bd82db" />

### Ator Principal

Instrutor

### Objetivo

Registrar dados da avaliação física.

### Pré-condições

-   Aluno cadastrado.

### Pós-condições

-   Avaliação registrada.

### Fluxo Principal

1.  O instrutor seleciona o aluno.
2.  O instrutor registra peso, IMC e percentual de gordura.
3.  O sistema salva os dados.

### Fluxos Alternativos

-   **A1 --- Dados inválidos:**\
    O sistema solicita correção.

### RF Relacionados

-   RF08

### RNF Relacionados

-   RNF02

### RN Relacionadas

-   Nenhuma

## UC17 --- Anexar Arquivo de Avaliação
<img width="210" height="362" alt="image" src="https://github.com/user-attachments/assets/14dc364f-90d9-4f7f-b3a7-89da4ff13f63" />

### Ator Principal

Instrutor

### Objetivo

Adicionar arquivos à avaliação física.

### Pré-condições

-   Avaliação existente.

### Pós-condições

-   Arquivo anexado.

### Fluxo Principal

1.  O instrutor seleciona a avaliação.
2.  O instrutor envia o arquivo.
3.  O sistema salva o anexo.

### Fluxos Alternativos

-   **A1 --- Formato inválido:**\
    O sistema rejeita o arquivo.

### RF Relacionados

-   RF08

### RNF Relacionados

-   RNF02

### RN Relacionadas

-   Nenhuma

## UC18 --- Emitir Relatório de Inadimplência
<img width="260" height="254" alt="image" src="https://github.com/user-attachments/assets/c12e1d35-ccca-485b-9fb7-0dd538d3b67c" />

### Ator Principal

Gerente

### Objetivo

Gerar relatório de alunos inadimplentes.

### Pré-condições

-   Gerente autenticado.

### Pós-condições

-   Relatório exibido.

### Fluxo Principal

1.  O gerente acessa relatórios.
2.  O gerente seleciona relatório de inadimplência.
3.  O sistema gera o relatório.

### Fluxos Alternativos

-   **A1 --- Nenhum aluno inadimplente:**\
    O sistema informa ausência de registros.

### RF Relacionados

-   RF09

### RNF Relacionados

-   RNF03

### RN Relacionadas

-   Nenhuma

## UC19 --- Emitir Relatório de Ocupação de Aulas
<img width="284" height="308" alt="image" src="https://github.com/user-attachments/assets/52ef9a6d-6a51-447c-893a-f2733c141d8f" />

### Ator Principal

Gerente

### Objetivo

Gerar relatório de ocupação das aulas.

### Pré-condições

-   Aulas registradas.

### Pós-condições

-   Relatório exibido.

### Fluxo Principal

1.  O gerente seleciona relatório de ocupação.
2.  O sistema calcula taxa de ocupação.
3.  O sistema apresenta os dados.

### Fluxos Alternativos

-   **A1 --- Nenhuma aula registrada:**\
    O sistema informa ausência de dados.

### RF Relacionados

-   RF09

### RNF Relacionados

-   RNF03

### RN Relacionadas

-   Nenhuma

## UC20 --- Enviar Notificações ao Aluno
<img width="263" height="362" alt="image" src="https://github.com/user-attachments/assets/cc8ee1b2-9a23-417d-a65e-d965857338e0" />

### Ator Principal

Sistema

### Objetivo

Enviar notificações sobre eventos importantes.

### Pré-condições

-   Evento registrado no sistema.

### Pós-condições

-   Notificação enviada.

### Fluxo Principal

1.  O sistema identifica evento (vencimento, reserva ou avaliação).
2.  O sistema envia notificação ao aluno.

### Fluxos Alternativos

-   **A1 --- Falha no envio:**\
    O sistema registra erro.

### RF Relacionados

-   RF10

### RNF Relacionados

-   RNF01, RNF03

### RN Relacionadas

-   Nenhuma
