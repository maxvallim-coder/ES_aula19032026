# Casos de Uso — Sistema FitPass Gym Management

### Imagens dos Casos de Uso

![e471ef83-db8a-4503-a661-90dc3ecfe9a8](https://github.com/user-attachments/assets/d2412457-f48c-49de-8edc-ef9ae8cce4cd) 
![a29d5c75-1e0a-4a9d-8e7c-72ee11cf8ac1](https://github.com/user-attachments/assets/780776cc-5646-4f3f-95cf-bb23ea466f22)
![4c1c2c47-9a9d-4314-853f-585fabadc579](https://github.com/user-attachments/assets/5bdf984c-0cc2-4fe6-bb62-b464d8982729)
![4ece5196-f690-439f-a379-353466aa8eac](https://github.com/user-attachments/assets/a8001196-beda-4082-8359-6624ba6a802c)

## UC01 — Cadastrar Aluno
### Ator Principal
Recepcionista

### Objetivo
Permitir o cadastro de novos alunos no sistema.

### Pré-condições
- Recepcionista deve estar autenticado no sistema.

### Pós-condições
- Aluno registrado no sistema com plano associado.

### Fluxo Principal
1. O recepcionista acessa a opção de cadastro de aluno.
2. O sistema solicita dados pessoais, contato e endereço.
3. O recepcionista seleciona o plano desejado.
4. O sistema valida os dados informados.
5. O sistema registra o aluno no banco de dados.

### Fluxos Alternativos
- **A1 — Dados obrigatórios ausentes:**  
  O sistema solicita o preenchimento dos campos faltantes.

### RF Relacionados
- RF01 — Cadastro de Alunos

### RNF Relacionados
- RNF04 — Usabilidade

### RN Relacionadas
- RN06 — Acesso restrito por perfil

- Digrama de atividade
  
<img width="612" height="532" alt="image" src="https://github.com/user-attachments/assets/d734cc07-263a-4626-9c25-fb0cdf9f308b" />


---

## UC02 — Gerenciar Planos
### Ator Principal
Gerente

### Objetivo
Permitir a criação e manutenção dos planos oferecidos pela academia.

### Pré-condições
- Gerente autenticado no sistema.

### Pós-condições
- Plano criado, atualizado ou desativado.

### Fluxo Principal
1. O gerente acessa o módulo de planos.
2. O sistema exibe a lista de planos cadastrados.
3. O gerente seleciona criar ou editar um plano.
4. O gerente informa nome, valor e duração.
5. O sistema salva as alterações.

### Fluxos Alternativos
- **A1 — Dados inválidos:**  
  O sistema solicita correção das informações.

### RF Relacionados
- RF02 — Gerenciamento de Planos

### RNF Relacionados
- RNF04 — Usabilidade

### RN Relacionadas
- RN06 — Acesso restrito por perfil

- Diagrama de atividade

<img width="473" height="587" alt="image" src="https://github.com/user-attachments/assets/e78d8dc7-af2e-4b91-a1ee-20d930f3e97b" />

---

## UC03 — Registrar Pagamento
### Ator Principal
Recepcionista

### Objetivo
Registrar o pagamento de mensalidade do aluno.

### Pré-condições
- Aluno cadastrado no sistema.
- Recepcionista autenticado.

### Pós-condições
- Pagamento registrado e situação do aluno atualizada.

### Fluxo Principal
1. O recepcionista localiza o aluno no sistema.
2. O sistema exibe a situação financeira.
3. O recepcionista seleciona a opção de registrar pagamento.
4. O recepcionista informa o método de pagamento.
5. O sistema registra o pagamento.
6. O sistema atualiza a regularidade do aluno.

### Fluxos Alternativos
- **A1 — Pagamento parcial informado:**  
  O sistema rejeita o pagamento.

### RF Relacionados
- RF03 — Controle de Pagamentos

### RNF Relacionados
- RNF02 — Segurança

### RN Relacionadas
- RN04 — Pagamento parcial  
- RN07 — Atualização automática da regularidade

- Diagrama de Atividade

<img width="408" height="477" alt="image" src="https://github.com/user-attachments/assets/7f3db792-6270-49f5-a0e4-570003c45a83" />


---

## UC04 — Verificar Regularidade do Aluno
### Ator Principal
Sistema

### Objetivo
Determinar se o aluno está com mensalidade em dia.

### Pré-condições
- Aluno cadastrado.

### Pós-condições
- Status de regularidade atualizado.

### Fluxo Principal
1. O sistema consulta o histórico de pagamentos.
2. O sistema verifica a data de vencimento da mensalidade.
3. O sistema define o status como regular ou inadimplente.

### Fluxos Alternativos
- **A1 — Pagamento vencido:**  
  O sistema marca o aluno como inadimplente.

### RF Relacionados
- RF04 — Regularidade do Aluno

### RNF Relacionados
- RNF03 — Performance

### RN Relacionadas
- RN01 — Bloqueio por inadimplência

- Diagrama de atividade

<img width="507" height="367" alt="image" src="https://github.com/user-attachments/assets/ef682793-5ecc-4159-a415-944478d4d41f" />

---

## UC05 — Validar Acesso na Catraca
### Ator Principal
Sistema de Catraca

### Objetivo
Permitir ou negar a entrada do aluno na academia.

### Pré-condições
- Aluno possuir RFID cadastrado.

### Pós-condições
- Entrada liberada ou bloqueada.

### Fluxo Principal
1. O aluno aproxima o cartão RFID da catraca.
2. A catraca envia o identificador para o sistema.
3. O sistema verifica a regularidade do aluno.
4. O sistema retorna autorização ou bloqueio.

### Fluxos Alternativos
- **A1 — Aluno inadimplente:**  
  O acesso é bloqueado.

### RF Relacionados
- RF05 — Controle de Acesso

### RNF Relacionados
- RNF03 — Performance  
- RNF06 — Integração

### RN Relacionadas
- RN01 — Bloqueio por inadimplência

- Diagrama de atividade

<img width="368" height="367" alt="image" src="https://github.com/user-attachments/assets/de635877-4ab6-4770-828e-a2adbe1a29ea" />

---

## UC06 — Agendar Aula
### Ator Principal
Aluno

### Objetivo
Permitir que o aluno reserve vaga em uma aula.

### Pré-condições
- Aluno autenticado.
- Aula disponível.

### Pós-condições
- Reserva registrada.

### Fluxo Principal
1. O aluno acessa a lista de aulas disponíveis.
2. O sistema exibe horários e vagas.
3. O aluno seleciona uma aula.
4. O sistema registra a reserva.

### Fluxos Alternativos
- **A1 — Aula lotada:**  
  O sistema bloqueia o agendamento.

### RF Relacionados
- RF06 — Agendamento de Aulas

### RNF Relacionados
- RNF04 — Usabilidade

### RN Relacionadas
- RN02 — Limite de vagas

- Diagrama de atividade

<img width="414" height="367" alt="image" src="https://github.com/user-attachments/assets/14f336fa-f6a2-4a11-812b-de467c266dcc" />

---

## UC07 — Cancelar Agendamento de Aula
### Ator Principal
Aluno

### Objetivo
Permitir que o aluno cancele uma reserva.

### Pré-condições
- Agendamento existente.

### Pós-condições
- Reserva cancelada.

### Fluxo Principal
1. O aluno acessa seus agendamentos.
2. O aluno seleciona a aula.
3. O aluno solicita cancelamento.
4. O sistema remove a reserva.

### Fluxos Alternativos
- **A1 — Prazo expirado:**  
  O sistema impede o cancelamento.

### RF Relacionados
- RF06 — Agendamento de Aulas

### RNF Relacionados
- RNF04 — Usabilidade

### RN Relacionadas
- RN03 — Cancelamento de agendamento

- Diagrama de atividade

<img width="409" height="367" alt="image" src="https://github.com/user-attachments/assets/db5d761c-bfac-4956-b4d0-644f3933f59c" />

---

## UC08 — Registrar Presença em Aula
### Ator Principal
Instrutor

### Objetivo
Registrar presença dos alunos nas aulas.

### Pré-condições
- Aula iniciada.

### Pós-condições
- Presença registrada.

### Fluxo Principal
1. O instrutor acessa a aula no sistema.
2. O sistema exibe lista de alunos inscritos.
3. O instrutor marca presença.
4. O sistema salva o registro.

### Fluxos Alternativos
- **A1 — Aluno não compareceu:**  
  O instrutor marca ausência.

### RF Relacionados
- RF07 — Lista de Presença

### RNF Relacionados
- RNF04 — Usabilidade

### RN Relacionadas
- RN06 — Acesso restrito por perfil

- Diagrama de atividade

<img width="337" height="462" alt="image" src="https://github.com/user-attachments/assets/808509cd-0ae3-4f45-bdf2-a6b2dd5cdb0b" />

---

## UC09 — Registrar Avaliação Física
### Ator Principal
Instrutor

### Objetivo
Registrar dados da avaliação física do aluno.

### Pré-condições
- Aluno ativo.

### Pós-condições
- Avaliação armazenada no sistema.

### Fluxo Principal
1. O instrutor seleciona o aluno.
2. O instrutor insere dados como peso, IMC e percentual de gordura.
3. O instrutor anexa arquivos, se necessário.
4. O sistema salva a avaliação.

### Fluxos Alternativos
- **A1 — Aluno irregular:**  
  O sistema impede o registro da avaliação.

### RF Relacionados
- RF08 — Avaliação Física

### RNF Relacionados
- RNF02 — Segurança

### RN Relacionadas
- RN05 — Avaliação física

<img width="371" height="367" alt="image" src="https://github.com/user-attachments/assets/ea390341-3876-4ad9-94f3-3f0b5c2803c7" />



---

## UC10 — Emitir Relatórios Gerenciais
### Ator Principal
Gerente

### Objetivo
Gerar relatórios sobre o funcionamento da academia.

### Pré-condições
- Gerente autenticado.

### Pós-condições
- Relatório exibido ou exportado.

### Fluxo Principal
1. O gerente acessa o módulo de relatórios.
2. O sistema exibe opções disponíveis.
3. O gerente seleciona um tipo de relatório.
4. O sistema gera o relatório.

### Fluxos Alternativos
- **A1 — Nenhum dado disponível:**  
  O sistema informa ausência de dados.

### RF Relacionados
- RF09 — Relatórios Gerenciais

### RNF Relacionados
- RNF05 — Escalabilidade

<img width="404" height="312" alt="image" src="https://github.com/user-attachments/assets/4be895a0-8045-4ecb-81c0-54118ac55515" />


---

## UC11 — Consultar Dados do Aluno
### Ator Principal
Recepcionista

### Objetivo
Permitir visualizar os dados cadastrais e situação do aluno.

### Pré-condições
- Recepcionista autenticado.
- Aluno cadastrado no sistema.

### Pós-condições
- Informações do aluno exibidas na tela.

### Fluxo Principal
1. O recepcionista acessa a busca de alunos.
2. O recepcionista informa nome, CPF ou matrícula.
3. O sistema localiza o aluno.
4. O sistema exibe dados pessoais, plano e situação financeira.

### Fluxos Alternativos
- **A1 — Aluno não encontrado:**  
  O sistema informa que nenhum registro foi localizado.

### RF Relacionados
- RF01 — Cadastro de Alunos

### RNF Relacionados
- RNF03 — Performance

### RN Relacionadas
- RN06 — Acesso restrito por perfil

<img width="446" height="367" alt="image" src="https://github.com/user-attachments/assets/8e07acb0-dbad-48c0-b5fa-861110000af0" />


---

## UC12 — Atualizar Dados do Aluno
### Ator Principal
Recepcionista

### Objetivo
Permitir a atualização de dados cadastrais do aluno.

### Pré-condições
- Recepcionista autenticado.
- Aluno cadastrado.

### Pós-condições
- Dados atualizados no sistema.

### Fluxo Principal
1. O recepcionista localiza o aluno.
2. O sistema exibe os dados atuais.
3. O recepcionista altera as informações necessárias.
4. O sistema valida os dados.
5. O sistema salva as alterações.

### Fluxos Alternativos
- **A1 — Dados inválidos:**  
  O sistema solicita correção antes de salvar.

### RF Relacionados
- RF01 — Cadastro de Alunos

### RNF Relacionados
- RNF04 — Usabilidade

### RN Relacionadas
- RN06 — Acesso restrito por perfil

<img width="379" height="477" alt="image" src="https://github.com/user-attachments/assets/d914b12d-128c-435f-8e20-07450d7d16a7" />


---

## UC13 — Visualizar Grade de Aulas
### Ator Principal
Aluno

### Objetivo
Permitir que o aluno visualize todas as aulas disponíveis.

### Pré-condições
- Aluno autenticado.

### Pós-condições
- Lista de aulas exibida.

### Fluxo Principal
1. O aluno acessa o menu de aulas.
2. O sistema consulta a programação disponível.
3. O sistema exibe horários, instrutores e vagas restantes.

### Fluxos Alternativos
- **A1 — Nenhuma aula disponível:**  
  O sistema informa que não há aulas cadastradas.

### RF Relacionados
- RF06 — Agendamento de Aulas

### RNF Relacionados
- RNF04 — Usabilidade

### RN Relacionadas
- RN02 — Limite de vagas

<img width="451" height="312" alt="image" src="https://github.com/user-attachments/assets/8dd80081-b29f-4a67-a23d-18f916948bb1" />


---

## UC14 — Receber Notificação de Mensalidade
### Ator Principal
Aluno

### Objetivo
Informar o aluno sobre o vencimento da mensalidade.

### Pré-condições
- Aluno cadastrado no sistema.

### Pós-condições
- Notificação enviada ao aluno.

### Fluxo Principal
1. O sistema verifica datas de vencimento das mensalidades.
2. O sistema identifica mensalidades próximas do vencimento.
3. O sistema envia notificação ao aluno.

### Fluxos Alternativos
- **A1 — Falha no envio:**  
  O sistema registra erro e tenta reenviar posteriormente.

### RF Relacionados
- RF10 — Notificações

### RNF Relacionados
- RNF01 — Disponibilidade

### RN Relacionadas
- RN01 — Bloqueio por inadimplência

<img width="371" height="422" alt="image" src="https://github.com/user-attachments/assets/2b9a68a5-3c47-4489-8605-9cf909abe238" />

---

## UC15 — Confirmar Agendamento de Aula
### Ator Principal
Sistema

### Objetivo
Enviar confirmação ao aluno após reserva de aula.

### Pré-condições
- Agendamento realizado.

### Pós-condições
- Aluno recebe confirmação do agendamento.

### Fluxo Principal
1. O aluno realiza o agendamento de aula.
2. O sistema registra a reserva.
3. O sistema envia notificação de confirmação.

### Fluxos Alternativos
- **A1 — Falha na notificação:**  
  O sistema registra o erro.

### RF Relacionados
- RF10 — Notificações

### RNF Relacionados
- RNF01 — Disponibilidade

### RN Relacionadas
- RN02 — Limite de vagas

<img width="349" height="367" alt="image" src="https://github.com/user-attachments/assets/76745203-5f30-459f-9c3c-b26c0fbe204b" />



---

## UC16 — Registrar Novo Tipo de Aula
### Ator Principal
Gerente

### Objetivo
Cadastrar novos tipos de aulas no sistema.

### Pré-condições
- Gerente autenticado.

### Pós-condições
- Aula registrada na programação.

### Fluxo Principal
1. O gerente acessa o módulo de aulas.
2. O gerente seleciona criar nova aula.
3. O gerente informa nome, horário e capacidade.
4. O sistema salva o cadastro.

### Fluxos Alternativos
- **A1 — Capacidade inválida:**  
  O sistema solicita correção.

### RF Relacionados
- RF06 — Agendamento de Aulas

### RNF Relacionados
- RNF05 — Escalabilidade

### RN Relacionadas
- RN02 — Limite de vagas

<img width="350" height="422" alt="image" src="https://github.com/user-attachments/assets/c6eb87dd-625b-4253-90c1-ac5b2c8d6173" />


---

## UC17 — Consultar Histórico de Acessos
### Ator Principal
Gerente

### Objetivo
Visualizar registros de entrada e saída dos alunos.

### Pré-condições
- Gerente autenticado.

### Pós-condições
- Histórico exibido.

### Fluxo Principal
1. O gerente acessa o módulo de relatórios.
2. O gerente seleciona histórico de acessos.
3. O sistema consulta registros da catraca.
4. O sistema exibe o histórico.

### Fluxos Alternativos
- **A1 — Nenhum registro encontrado:**  
  O sistema informa ausência de dados.

### RF Relacionados
- RF09 — Relatórios Gerenciais

### RNF Relacionados
- RNF06 — Integração

### RN Relacionadas
- RN06 — Acesso restrito por perfil

<img width="418" height="367" alt="image" src="https://github.com/user-attachments/assets/6940369c-8fa6-49de-9f03-349b41eaa3e2" />



---

## UC18 — Gerar Relatório de Inadimplência
### Ator Principal
Gerente

### Objetivo
Identificar alunos com pagamentos atrasados.

### Pré-condições
- Gerente autenticado.

### Pós-condições
- Relatório exibido ou exportado.

### Fluxo Principal
1. O gerente acessa relatórios.
2. O gerente seleciona inadimplência.
3. O sistema consulta pagamentos vencidos.
4. O sistema gera relatório.

### Fluxos Alternativos
- **A1 — Nenhum aluno inadimplente:**  
  O sistema informa que não há registros.

### RF Relacionados
- RF09 — Relatórios Gerenciais

### RNF Relacionados
- RNF03 — Performance

### RN Relacionadas
- RN01 — Bloqueio por inadimplência

<img width="418" height="367" alt="image" src="https://github.com/user-attachments/assets/6edb68a3-e8af-4f96-99b0-b1d4e12dd3d4" />

---

## UC19 — Anexar Arquivo em Avaliação Física
### Ator Principal
Instrutor

### Objetivo
Adicionar arquivos ou documentos à avaliação física.

### Pré-condições
- Avaliação física iniciada.

### Pós-condições
- Arquivo anexado ao registro.

### Fluxo Principal
1. O instrutor abre a avaliação do aluno.
2. O instrutor seleciona anexar arquivo.
3. O sistema realiza upload do documento.
4. O sistema associa o arquivo à avaliação.

### Fluxos Alternativos
- **A1 — Arquivo inválido:**  
  O sistema rejeita o upload.

### RF Relacionados
- RF08 — Avaliação Física

### RNF Relacionados
- RNF02 — Segurança

### RN Relacionadas
- RN05 — Avaliação física

<img width="407" height="367" alt="image" src="https://github.com/user-attachments/assets/981eac6a-67bf-4136-b450-e80a0f693e7d" />


---

## UC20 — Verificar Situação do Aluno na Entrada
### Ator Principal
Recepcionista

### Objetivo
Permitir consulta rápida da situação do aluno.

### Pré-condições
- Recepcionista autenticado.
- Aluno cadastrado.

### Pós-condições
- Situação exibida.

### Fluxo Principal
1. O recepcionista busca o aluno.
2. O sistema consulta situação financeira.
3. O sistema exibe status do aluno.

### Fluxos Alternativos
- **A1 — Aluno inadimplente:**  
  O sistema alerta o recepcionista.

### RF Relacionados
- RF04 — Regularidade do Aluno

### RNF Relacionados
- RNF03 — Performance

### RN Relacionadas
- RN01 — Bloqueio por inadimplência

### RN Relacionadas
- RN06 — Acesso restrito por perfil

<img width="406" height="312" alt="image" src="https://github.com/user-attachments/assets/7206095f-c264-4c22-aaf0-9e41968f932f" />
