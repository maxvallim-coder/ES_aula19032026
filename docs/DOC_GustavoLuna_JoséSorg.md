UC01 — Realizar Login

Ator Principal
Usuário (Aluno, Recepcionista, Instrutor ou Gerente)

Objetivo
Permitir que o usuário acesse o sistema.

Pré-condições
Usuário deve possuir cadastro ativo.

Pós-condições
Sessão iniciada com sucesso.

Fluxo Principal
O usuário informa e-mail e senha.
O sistema valida as credenciais.
O sistema autentica o usuário e redireciona para a tela inicial.

Fluxos Alternativos

A1 — Senha incorreta
O sistema exibe mensagem de erro.

A2 — Conta bloqueada
O sistema impede o login e instrui o usuário a recuperar o acesso.

RF Relacionados
RF01 — Autenticação de usuário

RNF Relacionados
RNF01 — Segurança do sistema

RN Relacionadas
RN01 — Apenas usuários cadastrados podem acessar o sistema

<img width="220" height="262" alt="image" src="https://github.com/user-attachments/assets/7185a23f-c8be-4f12-8a1a-4cf971dd6549" />


UC02 — Cadastrar Aluno

Ator Principal
Recepcionista

Objetivo
Permitir o cadastro de um novo aluno no sistema.

Pré-condições
Recepcionista deve estar autenticado.

Pós-condições
Aluno cadastrado no sistema.

Fluxo Principal
Recepcionista acessa a tela de cadastro.
Recepcionista informa os dados do aluno.
Sistema valida as informações.
Sistema registra o aluno no banco de dados.

Fluxos Alternativos

A1 — CPF já cadastrado
Sistema informa que o aluno já existe.

RF Relacionados
RF02 — Cadastro de alunos

RNF Relacionados
RNF01 — Segurança de dados

RN Relacionadas
RN02 — CPF deve ser único

<img width="163" height="184" alt="image" src="https://github.com/user-attachments/assets/3315126c-71da-4f3b-b6d9-6085dad31f88" />

UC03 — Atualizar Dados do Aluno

Ator Principal
Recepcionista

Objetivo
Atualizar as informações cadastrais do aluno.

Pré-condições
Aluno deve estar cadastrado.

Pós-condições
Dados atualizados no sistema.

Fluxo Principal
Recepcionista busca o aluno.
Recepcionista altera os dados.
Sistema valida as informações.
Sistema salva as alterações.

Fluxos Alternativos

A1 — Aluno não encontrado
Sistema informa erro.

RF Relacionados
RF03 — Atualização de cadastro

RNF Relacionados
RNF01 — Segurança

RN Relacionadas
RN03 — Apenas usuários autorizados podem alterar dados

<img width="210" height="193" alt="image" src="https://github.com/user-attachments/assets/bc841ec4-fc80-4538-a5b4-9e11b230ee0b" />

UC04 — Realizar Matrícula

Ator Principal
Recepcionista

Objetivo
Registrar a matrícula de um aluno em um plano.

Pré-condições
Aluno deve estar cadastrado.

Pós-condições
Matrícula registrada.

Fluxo Principal
Recepcionista seleciona o aluno.
Sistema exibe planos disponíveis.
Recepcionista escolhe o plano.
Sistema registra a matrícula.

Fluxos Alternativos

A1 — Plano indisponível
Sistema informa indisponibilidade.

RF Relacionados
RF04 — Gestão de matrículas

RNF Relacionados
RNF02 — Disponibilidade do sistema

RN Relacionadas
RN04 — Aluno deve possuir apenas uma matrícula ativa

<img width="170" height="185" alt="image" src="https://github.com/user-attachments/assets/5682f6ef-4beb-40b9-b71f-cd9b97a061df" />

UC05 — Gerenciar Planos

Ator Principal
Gerente

Objetivo
Cadastrar ou alterar planos da academia.

Pré-condições
Gerente autenticado.

Pós-condições
Plano criado ou atualizado.

Fluxo Principal
Gerente acessa gerenciamento de planos.
Gerente cadastra ou edita plano.
Sistema salva informações.

Fluxos Alternativos

A1 — Dados inválidos
Sistema solicita correção.

RF Relacionados
RF05 — Gestão de planos

RNF Relacionados
RNF01 — Segurança

RN Relacionadas
RN05 — Apenas gerente pode alterar planos

<img width="168" height="185" alt="image" src="https://github.com/user-attachments/assets/bb4cd71a-edfb-480a-b75d-06d016c7279d" />

UC06 — Registrar Pagamento

Ator Principal
Recepcionista

Objetivo
Registrar pagamento da mensalidade do aluno.

Pré-condições
Aluno deve possuir matrícula ativa.

Pós-condições
Pagamento registrado.

Fluxo Principal
Recepcionista seleciona o aluno.
Recepcionista registra pagamento.
Sistema confirma a transação.

Fluxos Alternativos

A1 — Falha no pagamento
Sistema informa erro.

RF Relacionados
RF06 — Registro de pagamentos

RNF Relacionados
RNF03 — Confiabilidade

RN Relacionadas
RN06 — Pagamento deve ser vinculado a matrícula

<img width="188" height="189" alt="image" src="https://github.com/user-attachments/assets/15cd0169-31d5-4c10-a987-839134a81648" />

UC07 — Validar Acesso na Catraca

Ator Principal
Sistema de Catraca

Objetivo
Permitir acesso do aluno à academia.

Pré-condições
Aluno com matrícula ativa.

Pós-condições
Acesso liberado ou negado.

Fluxo Principal
Aluno aproxima cartão RFID.
Sistema verifica matrícula.
Sistema libera catraca.

Fluxos Alternativos

A1 — Matrícula vencida
Sistema bloqueia acesso.

RF Relacionados
RF07 — Controle de acesso

RNF Relacionados
RNF04 — Tempo de resposta rápido

RN Relacionadas
RN07 — Apenas alunos ativos podem acessar

<img width="218" height="195" alt="image" src="https://github.com/user-attachments/assets/e1bc86c1-4a42-430e-a52c-5e00e4db96b1" />

UC08 — Consultar Status da Matrícula

Ator Principal
Aluno

Objetivo
Permitir que o aluno consulte a situação da matrícula.

Pré-condições
Aluno autenticado.

Pós-condições
Informações exibidas.

Fluxo Principal
Aluno acessa menu matrícula.
Sistema mostra status da matrícula.

Fluxos Alternativos

A1 — Matrícula inexistente
Sistema informa ausência de matrícula.

RF Relacionados
RF08 — Consulta de matrícula

RNF Relacionados
RNF02 — Disponibilidade

RN Relacionadas
RN08 — Aluno pode visualizar apenas seus dados

<img width="234" height="198" alt="image" src="https://github.com/user-attachments/assets/d9e70156-7796-48ef-8745-54b50fb9d016" />

UC09 — Agendar Aula

Ator Principal
Aluno

Objetivo
Permitir que o aluno reserve uma vaga em aula.

Pré-condições
Aluno com matrícula ativa.

Pós-condições
Aula agendada.

Fluxo Principal
Aluno acessa agenda de aulas.
Aluno escolhe aula disponível.
Sistema confirma agendamento.

Fluxos Alternativos

A1 — Aula lotada
Sistema informa indisponibilidade.

RF Relacionados
RF09 — Agendamento de aulas

RNF Relacionados
RNF02 — Disponibilidade

RN Relacionadas
RN09 — Limite de vagas por aula
<img width="150" height="182" alt="image" src="https://github.com/user-attachments/assets/0e48846f-dd64-4ee5-9473-4c66b59f0bca" />

UC10 — Cancelar Agendamento de Aula

Ator Principal
Aluno

Objetivo
Cancelar aula previamente agendada.

Pré-condições
Aula deve estar agendada.

Pós-condições
Agendamento removido.

Fluxo Principal
Aluno acessa lista de aulas.
Aluno cancela agendamento.
Sistema confirma cancelamento.

Fluxos Alternativos

A1 — Prazo expirado
Sistema impede cancelamento.

RF Relacionados
RF10 — Cancelamento de aula

RNF Relacionados
RNF02 — Disponibilidade

RN Relacionadas
RN10 — Cancelamento deve ocorrer antes da aula

<img width="248" height="201" alt="image" src="https://github.com/user-attachments/assets/e27336af-2db1-4877-8d3e-fdf33f7b0eab" />

UC11 — Registrar Presença em Aula

Ator Principal
Instrutor

Objetivo
Registrar presença dos alunos na aula.

Pré-condições
Aula deve estar em andamento.

Pós-condições
Presenças registradas.

Fluxo Principal
Instrutor acessa lista de alunos.
Instrutor marca presença.
Sistema salva informações.

Fluxos Alternativos

A1 — Aluno não inscrito
Sistema impede registro.

RF Relacionados
RF11 — Controle de presença

RNF Relacionados
RNF03 — Confiabilidade

RN Relacionadas
RN11 — Apenas alunos inscritos podem ter presença registrada

<img width="226" height="197" alt="image" src="https://github.com/user-attachments/assets/c573ad32-ecfd-43ae-b513-9b3c52beb847" />

UC12 — Cadastrar Instrutor

Ator Principal
Gerente

Objetivo
Cadastrar novo instrutor no sistema.

Pré-condições
Gerente autenticado.

Pós-condições
Instrutor cadastrado.

Fluxo Principal
Gerente acessa cadastro.
Gerente insere dados do instrutor.
Sistema salva cadastro.

Fluxos Alternativos

A1 — Dados inválidos
Sistema solicita correção.

RF Relacionados
RF12 — Cadastro de instrutor

RNF Relacionados
RNF01 — Segurança

RN Relacionadas
RN12 — Instrutor deve possuir identificação única

<img width="175" height="187" alt="image" src="https://github.com/user-attachments/assets/334ce09c-7f92-4bbd-b5ea-19ddcf27e18e" />

UC13 — Criar Aula

Ator Principal
Instrutor

Objetivo
Criar uma nova aula no sistema.

Pré-condições
Instrutor autenticado.

Pós-condições
Aula cadastrada.

Fluxo Principal
Instrutor informa data, horário e capacidade.
Sistema registra aula.

Fluxos Alternativos

A1 — Conflito de horário
Sistema impede cadastro.

RF Relacionados
RF13 — Gestão de aulas

RNF Relacionados
RNF02 — Disponibilidade

RN Relacionadas
RN13 — Aula não pode conflitar com outra

<img width="124" height="180" alt="image" src="https://github.com/user-attachments/assets/06b1555c-799b-401e-9bcf-1a01cd8b6742" />

UC14 — Atualizar Aula

Ator Principal
Instrutor

Objetivo
Atualizar informações da aula.

Pré-condições
Aula existente.

Pós-condições
Aula atualizada.

Fluxo Principal
Instrutor seleciona aula.
Instrutor altera dados.
Sistema salva alterações.

Fluxos Alternativos

A1 — Aula inexistente
Sistema informa erro.

RF Relacionados
RF14 — Atualização de aula

RNF Relacionados
RNF01 — Segurança

RN Relacionadas
RN14 — Alterações devem ser registradas

<img width="150" height="182" alt="image" src="https://github.com/user-attachments/assets/5c6893b1-5254-448d-8446-929d659ec4d7" />

UC15 — Registrar Avaliação Física

Ator Principal
Instrutor

Objetivo
Registrar dados da avaliação física do aluno.

Pré-condições
Aluno cadastrado.

Pós-condições
Avaliação registrada.

Fluxo Principal
Instrutor acessa ficha do aluno.
Instrutor insere dados da avaliação.
Sistema salva informações.

Fluxos Alternativos

A1 — Dados inválidos
Sistema solicita correção.

RF Relacionados
RF15 — Avaliação física

RNF Relacionados
RNF01 — Segurança

RN Relacionadas
RN15 — Avaliação deve conter data e responsável

<img width="214" height="194" alt="image" src="https://github.com/user-attachments/assets/dc67c35b-faf6-4b0e-911d-05aac28b0cfe" />

UC16 — Consultar Avaliação Física

Ator Principal
Aluno

Objetivo
Visualizar avaliações físicas registradas.

Pré-condições
Aluno autenticado.

Pós-condições
Avaliação exibida.

Fluxo Principal
Aluno acessa área de avaliações.
Sistema mostra histórico.

Fluxos Alternativos

A1 — Nenhuma avaliação registrada
Sistema informa ausência.

RF Relacionados
RF16 — Consulta de avaliação

RNF Relacionados
RNF02 — Disponibilidade

RN Relacionadas
RN16 — Apenas o aluno pode visualizar suas avaliações

<img width="217" height="195" alt="image" src="https://github.com/user-attachments/assets/f66c2556-a4ee-45db-8c15-bcf307c8469f" />

UC17 — Gerar Relatório de Frequência

Ator Principal
Gerente

Objetivo
Gerar relatório de frequência dos alunos.

Pré-condições
Gerente autenticado.

Pós-condições
Relatório exibido.

Fluxo Principal
Gerente seleciona período.
Sistema gera relatório.

Fluxos Alternativos

A1 — Sem dados
Sistema informa ausência de registros.

RF Relacionados
RF17 — Relatórios de frequência

RNF Relacionados
RNF03 — Desempenho

RN Relacionadas
RN17 — Relatórios devem considerar período informado

<img width="242" height="200" alt="image" src="https://github.com/user-attachments/assets/7ed99031-2105-4b61-a44f-a1dfb5cf8e3f" />

UC18 — Gerar Relatório Financeiro

Ator Principal
Gerente

Objetivo
Gerar relatório financeiro da academia.

Pré-condições
Gerente autenticado.

Pós-condições
Relatório financeiro exibido.

Fluxo Principal
Gerente seleciona período.
Sistema compila pagamentos.
Sistema apresenta relatório.

Fluxos Alternativos

A1 — Sem pagamentos
Sistema informa ausência de registros.

RF Relacionados
RF18 — Relatórios financeiros

RNF Relacionados
RNF03 — Desempenho

RN Relacionadas
RN18 — Apenas gerente pode visualizar relatórios financeiros

<img width="219" height="195" alt="image" src="https://github.com/user-attachments/assets/a6e0385c-94f0-41de-9913-bafa7d7af63e" />

UC19 — Gerenciar Usuários do Sistema

Ator Principal
Gerente

Objetivo
Administrar contas de usuários do sistema.

Pré-condições
Gerente autenticado.

Pós-condições
Usuários atualizados.

Fluxo Principal
Gerente acessa área de usuários.
Gerente cria ou altera contas.
Sistema salva alterações.

Fluxos Alternativos

A1 — Usuário duplicado
Sistema informa erro.

RF Relacionados
RF19 — Gestão de usuários

RNF Relacionados
RNF01 — Segurança

RN Relacionadas
RN19 — Apenas gerente pode administrar usuários

<img width="243" height="200" alt="image" src="https://github.com/user-attachments/assets/65b0c272-09f5-403f-b01d-c414155ab064" />

UC20 — Encerrar Sessão

Ator Principal
Usuário

Objetivo
Encerrar a sessão atual no sistema.

Pré-condições
Usuário autenticado.

Pós-condições
Sessão finalizada.

Fluxo Principal
Usuário seleciona opção sair.
Sistema encerra sessão.
Sistema retorna à tela de login.

Fluxos Alternativos

A1 — Sessão expirada
Sistema redireciona para login automaticamente.

RF Relacionados
RF20 — Logout

RNF Relacionados
RNF01 — Segurança

RN Relacionadas
RN20 — Sessão deve ser encerrada após inatividade
eu preciso de um diagrama p cada uma dessas coisas
<img width="165" height="184" alt="image" src="https://github.com/user-attachments/assets/e0d7e1ec-04ef-4197-97a3-99cd12275793" />
