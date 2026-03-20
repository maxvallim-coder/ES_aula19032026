# Entrega – Documento de Casos de Uso e Diagramas

## Identificação da Dupla
- Aluno 1: Leandro Coelho

## Arquivos Entregues

### Documento de Casos de Uso
Nome do arquivo entregue: UC_LeandroCoelho.md

## Issues Relacionadas
- Relacionado à Issue **#1 – Documento de Casos de Uso**
- Relacionado à Issue **#2 – Diagrama de Casos de Uso**

## Checklist Antes do Envio

- [x] O documento contém **20 casos de uso completos**, seguindo o template do arquivo `/docs/casosdeuso.md`
- [x] O nome do arquivo segue o padrão exigido
- [x] Os diagramas representam **todos os casos de uso listados** no documento
- [x] Todos os diagramas estão em **formato PNG**
- [x] As Issues foram referenciadas corretamente
- [x] O PR contém **apenas** os arquivos exigidos

---
<img width="509" height="1716" alt="image" src="https://github.com/user-attachments/assets/12f60c16-f084-4162-b02c-0b50194650d1" />

## UC01 — Realizar Login

<img width="509" height="291" alt="image" src="https://github.com/user-attachments/assets/504e33bf-2dca-44d5-8eb1-bfb60b76908a" />

### Ator Principal
Aluno, Recepcionista, Instrutor, Gerente

### Objetivo
Permitir que o usuário acesse o sistema de acordo com seu perfil.

### Pré-condições
- Usuário deve possuir cadastro ativo no sistema.

### Pós-condições
- Sessão iniciada com sucesso e menu correspondente ao perfil carregado.

### Fluxo Principal
1. O usuário informa e-mail e senha.
2. O sistema valida as credenciais e o perfil do usuário.
3. O sistema autentica o usuário e redireciona para a tela inicial.

### Fluxos Alternativos
- **A1 — Senha incorreta:** O sistema exibe mensagem de erro e solicita nova tentativa.
- **A2 — Conta bloqueada/inativa:** O sistema impede o login e instrui o usuário a contatar a recepção.

### RF Relacionados
- N/A

### RNF Relacionados
- RNF02, RNF04

### RN Relacionadas
- RN06

---

## UC02 — Cadastrar Novo Aluno

<img width="415" height="431" alt="image" src="https://github.com/user-attachments/assets/57965b76-466a-4884-a9fd-c86303d7d379" />

### Ator Principal
Recepcionista

### Objetivo
Registrar um novo aluno na base de dados da academia.

### Pré-condições
- Recepcionista deve estar logado no sistema.

### Pós-condições
- Aluno cadastrado no sistema com dados pessoais e pronto para contratação de plano.

### Fluxo Principal
1. A recepcionista acessa a tela de cadastro de alunos.
2. Preenche os dados pessoais, contato e endereço.
3. O sistema valida as informações e salva o registro.

### Fluxos Alternativos
- **A1 — CPF já cadastrado:** O sistema avisa que o aluno já existe e sugere ir para a tela de atualização.

### RF Relacionados
- RF01

### RNF Relacionados
- RNF02, RNF04

### RN Relacionadas
- RN06

---

## UC03 — Editar Dados do Aluno

<img width="509" height="364" alt="image" src="https://github.com/user-attachments/assets/aeecac77-97ce-4361-b852-5aa6d694df42" />


### Ator Principal
Recepcionista

### Objetivo
Atualizar informações pessoais, de contato ou endereço de um aluno.

### Pré-condições
- O aluno deve estar previamente cadastrado.

### Pós-condições
- Os dados do aluno são atualizados no banco de dados.

### Fluxo Principal
1. A recepcionista busca o aluno pelo nome ou CPF.
2. Altera os dados necessários (ex: novo telefone).
3. O sistema salva as alterações e exibe mensagem de sucesso.

### Fluxos Alternativos
- **A1 — Aluno não encontrado:** O sistema exibe mensagem informando que a busca não retornou resultados.

### RF Relacionados
- RF01

### RNF Relacionados
- RNF02

### RN Relacionadas
- RN06

---

## UC04 — Cadastrar Plano

<img width="436" height="375" alt="image" src="https://github.com/user-attachments/assets/e06328db-9644-46c6-9da2-128221ddc109" />


### Ator Principal
Gerente

### Objetivo
Criar um novo tipo de plano (mensal, anual, etc.) para comercialização.

### Pré-condições
- Gerente deve estar logado no sistema.

### Pós-condições
- Novo plano disponível para atribuição a alunos.

### Fluxo Principal
1. O gerente acessa a gestão de planos e seleciona "Novo Plano".
2. Define nome, duração, valor e modalidades inclusas.
3. O sistema salva e ativa o plano no catálogo.

### Fluxos Alternativos
- **A1 — Dados incompletos:** O sistema bloqueia o salvamento e destaca os campos obrigatórios.

### RF Relacionados
- RF02

### RNF Relacionados
- RNF04

### RN Relacionadas
- RN06

---

## UC05 — Editar/Desativar Plano

<img width="351" height="434" alt="image" src="https://github.com/user-attachments/assets/28e3f736-1a2c-4c0b-ae00-c0c15d296579" />


### Ator Principal
Gerente

### Objetivo
Alterar valores de um plano existente ou desativá-lo para não ser mais vendido.

### Pré-condições
- O plano deve existir no sistema.

### Pós-condições
- Plano atualizado ou desativado do catálogo de vendas.

### Fluxo Principal
1. O gerente lista os planos cadastrados e seleciona um.
2. Altera os parâmetros desejados ou marca como "Inativo".
3. O sistema salva as alterações.

### Fluxos Alternativos
- **A1 — Plano com alunos ativos:** Se for inativado, o sistema avisa que os alunos atuais continuam com acesso até o fim do contrato vigente.

### RF Relacionados
- RF02

### RNF Relacionados
- N/A

### RN Relacionadas
- RN06

---

## UC06 — Registrar Pagamento Presencial

<img width="509" height="422" alt="image" src="https://github.com/user-attachments/assets/e9552bf6-73d5-42dd-9034-b74c75246eb3" />

### Ator Principal
Recepcionista

### Objetivo
Registrar o pagamento da mensalidade feito fisicamente na academia.

### Pré-condições
- Aluno deve estar cadastrado e com plano atribuído.

### Pós-condições
- Pagamento registrado e regularidade do aluno atualizada.

### Fluxo Principal
1. A recepcionista localiza o aluno e acessa a fatura pendente.
2. Seleciona o método de pagamento (dinheiro, cartão ou PIX).
3. Confirma o recebimento do valor integral.
4. O sistema registra o pagamento e atualiza a situação do aluno.

### Fluxos Alternativos
- **A1 — Tentativa de pagamento parcial:** O sistema bloqueia a transação, pois o valor deve ser integral.

### RF Relacionados
- RF03, RF04

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN04, RN06, RN07

---

## UC07 — Realizar Pagamento Online

<img width="377" height="431" alt="image" src="https://github.com/user-attachments/assets/29d61c80-b336-4075-942f-f0ac56523c48" />

### Ator Principal
Aluno

### Objetivo
Permitir que o aluno pague sua mensalidade pelo sistema web/mobile.

### Pré-condições
- Aluno logado e com fatura em aberto.

### Pós-condições
- Pagamento processado e regularidade atualizada automaticamente.

### Fluxo Principal
1. O aluno acessa a área financeira.
2. Seleciona a fatura em aberto e escolhe Cartão de Crédito ou PIX.
3. Realiza o pagamento através da integração com o gateway.
4. O sistema confirma a transação e atualiza o status para regular.

### Fluxos Alternativos
- **A1 — Pagamento recusado:** O sistema notifica o aluno da recusa e mantém a fatura em aberto.

### RF Relacionados
- RF03, RF04

### RNF Relacionados
- RNF02, RNF03

### RN Relacionadas
- RN04, RN07

---

## UC08 — Validar Acesso via Catraca (RFID)

<img width="389" height="486" alt="image" src="https://github.com/user-attachments/assets/a49f71d9-a74a-415b-8b43-fc1e7f6d66a2" />


### Ator Principal
Sistema de Catraca

### Objetivo
Liberar ou bloquear a entrada do aluno fisicamente na academia.

### Pré-condições
- O aluno deve aproximar sua tag RFID/Biometria da catraca.

### Pós-condições
- Catraca liberada ou bloqueada, com registro de log no sistema.

### Fluxo Principal
1. O Sistema de Catraca envia o ID do aluno via API para o sistema FitPass.
2. O sistema FitPass verifica a regularidade do aluno.
3. Sendo regular, retorna status de "Liberado".
4. O Sistema de Catraca libera a roleta e o FitPass registra o histórico de acesso.

### Fluxos Alternativos
- **A1 — Mensalidade vencida há > 5 dias:** O FitPass retorna "Bloqueado" e a catraca não abre.

### RF Relacionados
- RF04, RF05

### RNF Relacionados
- RNF03, RNF06

### RN Relacionadas
- RN01

---

## UC09 — Visualizar Horários de Aulas

<img width="509" height="362" alt="image" src="https://github.com/user-attachments/assets/8a96c20d-b7a6-4ab1-a15c-f13c0da4d34f" />


### Ator Principal
Aluno

### Objetivo
Consultar a grade de aulas disponíveis na academia.

### Pré-condições
- Aluno logado no sistema.

### Pós-condições
- Grade de aulas exibida com horários, instrutores e vagas disponíveis.

### Fluxo Principal
1. O aluno acessa a aba "Grade de Aulas".
2. O sistema exibe o calendário semanal com as aulas.
3. O aluno pode filtrar por modalidade.

### Fluxos Alternativos
- **A1 — Nenhuma aula agendada:** O sistema exibe mensagem de que não há turmas para o filtro selecionado.

### RF Relacionados
- RF06

### RNF Relacionados
- RNF04

### RN Relacionadas
- N/A

---

## UC10 — Agendar Aula

<img width="445" height="431" alt="image" src="https://github.com/user-attachments/assets/e5ee3907-d1a0-4923-a533-53449628c0e5" />


### Ator Principal
Aluno

### Objetivo
Reservar uma vaga em uma aula específica.

### Pré-condições
- Aluno logado, situação regular e aula com vagas abertas.

### Pós-condições
- Vaga reservada para o aluno e notificação de confirmação enviada.

### Fluxo Principal
1. Na grade de horários, o aluno clica em "Agendar" na aula desejada.
2. O sistema verifica se há vagas disponíveis.
3. O sistema confirma o agendamento e reduz o número de vagas.
4. O sistema envia notificação de confirmação ao aluno.

### Fluxos Alternativos
- **A1 — Limite de vagas atingido:** O botão de agendar fica bloqueado e o sistema informa que a turma está lotada.

### RF Relacionados
- RF06, RF10

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN02

---

## UC11 — Cancelar Agendamento de Aula

<img width="407" height="431" alt="image" src="https://github.com/user-attachments/assets/76adec31-5444-4f83-a337-c0920fd000ad" />


### Ator Principal
Aluno

### Objetivo
Cancelar uma reserva feita previamente.

### Pré-condições
- Aluno deve ter um agendamento ativo.

### Pós-condições
- Vaga liberada no sistema para outros alunos.

### Fluxo Principal
1. O aluno acessa "Meus Agendamentos".
2. Clica em "Cancelar" na aula desejada.
3. O sistema verifica a antecedência (maior que 1 hora).
4. O sistema processa o cancelamento e devolve a vaga para a turma.

### Fluxos Alternativos
- **A1 — Cancelamento com menos de 1 hora:** O sistema impede a ação e informa a regra de cancelamento.

### RF Relacionados
- RF06

### RNF Relacionados
- N/A

### RN Relacionadas
- RN03

---

## UC12 — Registrar Presença em Aula

<img width="312" height="489" alt="image" src="https://github.com/user-attachments/assets/b11beadf-468e-4230-af7b-e1b575441418" />

### Ator Principal
Instrutor

### Objetivo
Confirmar quais alunos agendados compareceram à aula.

### Pré-condições
- Instrutor logado e aula prestes a iniciar ou recém-finalizada.

### Pós-condições
- Presença dos alunos registrada no banco de dados.

### Fluxo Principal
1. O instrutor acessa a aula específica no sistema.
2. O sistema lista todos os alunos que agendaram a aula.
3. O instrutor marca "Presente" ou "Falta" para cada um.
4. O sistema salva a lista de presença.

### Fluxos Alternativos
- **A1 — Aluno não agendado quer participar:** Se houver vaga, o instrutor pode adicionar o aluno manualmente à lista de presença na hora.

### RF Relacionados
- RF07

### RNF Relacionados
- RNF04

### RN Relacionadas
- RN06

---

## UC13 — Registrar Avaliação Física

<img width="479" height="431" alt="image" src="https://github.com/user-attachments/assets/90f573d9-4bf2-488d-8a23-df4056f99528" />


### Ator Principal
Instrutor

### Objetivo
Inserir métricas e documentos de avaliação física do aluno.

### Pré-condições
- Instrutor logado; aluno deve estar ativo e regular.

### Pós-condições
- Avaliação salva e notificação de liberação enviada ao aluno.

### Fluxo Principal
1. O instrutor seleciona o aluno e clica em "Nova Avaliação".
2. O sistema verifica a regularidade do aluno.
3. O instrutor insere peso, IMC, percentual de gordura e anexa arquivos (ex: bioimpedância).
4. O sistema salva os dados e dispara notificação ao aluno informando que a avaliação está disponível.

### Fluxos Alternativos
- **A1 — Aluno irregular:** O sistema bloqueia a criação da avaliação e avisa o instrutor.

### RF Relacionados
- RF08, RF10

### RNF Relacionados
- RNF02

### RN Relacionadas
- RN05, RN06

---

## UC14 — Visualizar Avaliação Física

<img width="508" height="375" alt="image" src="https://github.com/user-attachments/assets/de55ac60-78c8-44e0-a35b-7d9f59ab75a7" />


### Ator Principal
Aluno

### Objetivo
Acessar os resultados de suas avaliações físicas.

### Pré-condições
- Aluno logado e com avaliação já registrada pelo instrutor.

### Pós-condições
- Dados e anexos da avaliação exibidos em tela.

### Fluxo Principal
1. O aluno acessa o menu "Minhas Avaliações".
2. O sistema lista o histórico de avaliações por data.
3. O aluno seleciona uma avaliação para ver os detalhes e baixar anexos.

### Fluxos Alternativos
- **A1 — Nenhuma avaliação cadastrada:** O sistema exibe mensagem orientando a procurar um instrutor.

### RF Relacionados
- RF08

### RNF Relacionados
- RNF02 (Dados sensíveis e de saúde protegidos)

### RN Relacionadas
- N/A

---

## UC15 — Emitir Relatório de Inadimplência

<img width="491" height="375" alt="image" src="https://github.com/user-attachments/assets/343115f4-c758-472d-9086-febc845ce125" />


### Ator Principal
Gerente

### Objetivo
Visualizar lista de alunos com pagamentos atrasados.

### Pré-condições
- Gerente logado no sistema.

### Pós-condições
- Relatório gerado em tela com opção de exportação.

### Fluxo Principal
1. O gerente acessa o módulo de relatórios.
2. Seleciona "Relatório de Inadimplência".
3. O sistema compila e exibe a lista de alunos com faturas vencidas, ordenados por dias de atraso.

### Fluxos Alternativos
- **A1 — Nenhum inadimplente:** O sistema informa que todos os alunos estão regulares.

### RF Relacionados
- RF09

### RNF Relacionados
- N/A

### RN Relacionadas
- RN06

---

## UC16 — Emitir Relatório de Alunos Ativos

<img width="356" height="341" alt="image" src="https://github.com/user-attachments/assets/078d15a4-0d6f-4396-aa5b-dcd82d27b144" />


### Ator Principal
Gerente

### Objetivo
Acompanhar o total de alunos ativos divididos por planos.

### Pré-condições
- Gerente logado no sistema.

### Pós-condições
- Relatório quantitativo e qualitativo exibido.

### Fluxo Principal
1. O gerente acessa o módulo de relatórios e seleciona "Alunos Ativos".
2. O sistema busca os dados e apresenta um consolidado com totais e agrupamento por tipo de plano contratado.

### Fluxos Alternativos
- N/A

### RF Relacionados
- RF09

### RNF Relacionados
- N/A

### RN Relacionadas
- RN06

---

## UC17 — Emitir Relatório de Histórico de Acessos

<img width="509" height="341" alt="image" src="https://github.com/user-attachments/assets/f51b400a-48bd-441a-9dc6-95679bae79c4" />


### Ator Principal
Gerente

### Objetivo
Auditar os horários de pico e entrada de alunos via catraca.

### Pré-condições
- Gerente logado no sistema.

### Pós-condições
- Listagem e gráficos de acessos gerados.

### Fluxo Principal
1. O gerente seleciona "Histórico de Acessos".
2. Informa um período de datas.
3. O sistema gera a relação de entradas validadas e bloqueadas pela catraca no período informado.

### Fluxos Alternativos
- **A1 — Período sem registros:** O sistema exibe relatório em branco com aviso.

### RF Relacionados
- RF09

### RNF Relacionados
- N/A

### RN Relacionadas
- RN06

---

## UC18 — Emitir Relatório de Ocupação das Aulas

<img width="367" height="341" alt="image" src="https://github.com/user-attachments/assets/b4f57167-9c66-4e01-9413-3a50216625d6" />


### Ator Principal
Gerente

### Objetivo
Analisar quais aulas/modalidades estão mais cheias ou vazias.

### Pré-condições
- Gerente logado no sistema.

### Pós-condições
- Relatório de ocupação percentual e quantitativa gerado.

### Fluxo Principal
1. O gerente seleciona "Ocupação das Aulas".
2. Informa o mês ou semana desejada.
3. O sistema cruza os dados de agendamentos com as presenças registradas e exibe a taxa de ocupação de cada turma.

### Fluxos Alternativos
- N/A

### RF Relacionados
- RF09

### RNF Relacionados
- N/A

### RN Relacionadas
- RN06

---

## UC19 — Enviar Notificação de Vencimento

<img width="348" height="341" alt="image" src="https://github.com/user-attachments/assets/87ff614e-d51b-491e-b135-eec57bfafd88" />

### Ator Principal
Sistema (Tempo / Processo Batch)

### Objetivo
Avisar os alunos preventivamente sobre o vencimento de suas mensalidades.

### Pré-condições
- A fatura do aluno deve estar a 'x' dias do vencimento (ex: 3 dias antes).

### Pós-condições
- E-mail/Push notification enviado para o aluno.

### Fluxo Principal
1. Diariamente, o sistema varre o banco de dados buscando faturas próximas do vencimento.
2. Identifica os alunos correspondentes.
3. Dispara as mensagens de notificação padronizadas com o link para pagamento.

### Fluxos Alternativos
- N/A

### RF Relacionados
- RF10

### RNF Relacionados
- N/A

### RN Relacionadas
- N/A

---

## UC20 — Atualizar Status de Regularidade Automática

<img width="401" height="286" alt="image" src="https://github.com/user-attachments/assets/b71acc0d-a363-4529-82c2-4e104c84bbd6" />

### Ator Principal
Sistema (Trigger Financeiro)

### Objetivo
Modificar o status do aluno (regular/inadimplente) automaticamente com o passar dos dias ou compensação financeira.

### Pré-condições
- Fatura atingir 6 dias de atraso ou pagamento ser confirmado.

### Pós-condições
- Perfil do aluno bloqueado ou liberado para catraca/agendamentos.

### Fluxo Principal
1. O sistema recebe a confirmação de um pagamento (baixa automática) OU identifica via rotina diária que uma fatura passou de 5 dias de atraso.
2. O sistema altera o campo de regularidade no perfil do aluno correspondente.
3. A alteração reflete instantaneamente para a API da catraca e tela de agendamento.

### Fluxos Alternativos
- N/A

### RF Relacionados
- RF04

### RNF Relacionados
- RNF03

### RN Relacionadas
- RN01, RN07
