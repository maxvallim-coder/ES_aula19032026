Expanded use cases for user interactions, including login, registration, check-in, and more. Enhanced details for each use case with actors, objectives, and flows.

# Entrega – Documento de Casos de Uso e Diagramas

## Identificação da Dupla
- Aluno 1: Miguel Turatti Quirino
- Aluno 2: Luis Felipe Scacabarozi Vasconcellos

## Arquivos Entregues

### Documento de Casos de Uso
Nome do arquivo entregue: UC_MiguelTuratti_LuisVasconcellos.md

### Diagramas de Casos de Uso
<img width="501" height="1948" alt="image" src="https://github.com/user-attachments/assets/20f3d30d-5860-49f7-8778-4c4a41525180" />
---

## UC01 — Realizar Login

### Ator Principal

Usuário (Aluno, Instrutor ou Administrador)

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

* **A1 — Senha incorreta:** O sistema exibe mensagem de erro.
* **A2 — Conta bloqueada:** O sistema impede o login e instrui o usuário a recuperar o acesso.

### RF Relacionados

* RF01: Autenticação de usuários.

### RNF Relacionados

* RNF01: Criptografia de senhas.

### RN Relacionadas

* RN01: Bloqueio após 3 tentativas falhas.

<img width="659" height="422" alt="image" src="https://github.com/user-attachments/assets/014642a8-f497-4cdc-8d4c-38d36ea78236" />


---

## UC02 — Cadastrar Aluno

### Ator Principal

Recepcionista / Administrador

### Objetivo

Registrar novos alunos no sistema para controle de acesso e cobrança.

### Pré-condições

* Usuário autenticado com perfil administrativo.

### Pós-condições

* Aluno cadastrado com matrícula ativa.

### Fluxo Principal

1. O usuário preenche dados pessoais (nome, CPF, contato).
2. O sistema valida a unicidade do CPF.
3. O sistema gera um número de matrícula único.
4. O sistema salva o registro.

### Fluxos Alternativos

* **A1 — CPF já cadastrado:** O sistema impede o registro e sugere recuperar cadastro.

### RF Relacionados

* RF02: Gestão de perfis de alunos.

### RNF Relacionados

* RNF02: Armazenamento seguro de dados pessoais (LGPD).

### RN Relacionadas

* RN02: Idade mínima de 14 anos para cadastro independente.
<img width="431" height="367" alt="image" src="https://github.com/user-attachments/assets/85dd3d38-5a41-41d1-aeac-c009fd7a4c80" />

---

## UC03 — Registrar Entrada (Check-in)

### Ator Principal

Aluno

### Objetivo

Validar a entrada do aluno na academia via QR Code ou Biometria.

### Pré-condições

* Aluno possuir plano ativo e sem pendências financeiras.

### Pós-condições

* Registro de presença salvo; acesso liberado.

### Fluxo Principal

1. O aluno apresenta sua identificação (QR Code via app).
2. O sistema verifica o status do plano e pagamento.
3. O sistema registra data/hora e libera o acesso.

### Fluxos Alternativos

* **A1 — Plano vencido:** O sistema bloqueia a entrada e exibe alerta financeiro.

### RF Relacionados

* RF03: Controle de acesso.

### RNF Relacionados

* RNF03: Tempo de resposta inferior a 2 segundos.

### RN Relacionadas

* RN03: Impedir entrada com atraso de pagamento superior a 5 dias.
<img width="392" height="367" alt="image" src="https://github.com/user-attachments/assets/35d16d88-e3f2-446a-a423-18b8cd73e786" />



---

## UC04 — Montar Ficha de Treino

### Ator Principal

Instrutor

### Objetivo

Prescrever exercícios e séries para o aluno.

### Pré-condições

* Aluno selecionado no sistema; Instrutor logado.

### Pós-condições

* Ficha de treino vinculada ao aluno.

### Fluxo Principal

1. O instrutor seleciona os exercícios do catálogo.
2. O instrutor define séries, repetições e carga.
3. O sistema salva e disponibiliza o treino no app do aluno.

### Fluxos Alternativos

* **A1 — Aluno sem avaliação física:** O sistema emite um aviso recomendando avaliação prévia.

### RF Relacionados

* RF04: Prescrição de treinos.

### RNF Relacionados

* RNF04: Interface responsiva para tablets.
<img width="346" height="506" alt="image" src="https://github.com/user-attachments/assets/f6f9ed9f-9ab0-4aa9-a16b-ceedc94189b8" />



---

## UC05 — Visualizar Treino do Dia

### Ator Principal

Aluno

### Objetivo

Permitir que o aluno consulte sua rotina de exercícios pelo celular.

### Pré-condições

* Aplicativo instalado; Treino prescrito pelo instrutor.

### Pós-condições

* Exercícios exibidos na tela.

### Fluxo Principal

1. O aluno acessa a aba "Meus Treinos".
2. O sistema exibe a ficha atualizada conforme o cronograma (ex: Treino A).

### Fluxos Alternativos

* **A1 — Sem treino cadastrado:** O sistema orienta o aluno a procurar um instrutor.

### RF Relacionados

* RF05: Consulta de ficha técnica.
<img width="447" height="312" alt="image" src="https://github.com/user-attachments/assets/6c9beef9-7086-4e7b-9de9-e2af2be19c60" />



---

## UC06 — Realizar Avaliação Física

### Ator Principal

Instrutor / Avaliador

### Objetivo

Registrar medidas antropométricas e percentual de gordura.

### Pré-condições

* Perfil do aluno ativo.

### Pós-condições

* Relatório de evolução gerado.

### Fluxo Principal

1. O usuário insere peso, altura e dobras cutâneas.
2. O sistema calcula automaticamente o IMC e composição corporal.
3. O sistema salva os dados e gera o comparativo.

### RF Relacionados

* RF06: Módulo de avaliação física.

### RN Relacionadas

* RN04: Cálculos baseados no protocolo de Pollock (7 dobras).

 <img width="283" height="303" alt="image" src="https://github.com/user-attachments/assets/103d9ccf-ccf0-4efc-95d2-b6897ff0f585" />



---

## UC07 — Gerenciar Planos e Mensalidades

### Ator Principal

Administrador

### Objetivo

Criar e editar modalidades de planos (Mensal, Anual, VIP).

### Pré-condições

* Usuário logado como administrador.

### Fluxo Principal

1. O usuário define o nome do plano, preço e duração.
2. O sistema registra as regras de renovação.
3. O sistema disponibiliza o plano para novas vendas.

### RF Relacionados

* RF07: Configuração de produtos/serviços.

<img width="286" height="248" alt="image" src="https://github.com/user-attachments/assets/92b87eb2-bf5e-49dd-aba5-99a2b664abc6" />



---

## UC08 — Processar Pagamento

### Ator Principal

Recepcionista

### Objetivo

Registrar o recebimento de mensalidades.

### Pré-condições

* Aluno com fatura em aberto.

### Pós-condições

* Status do aluno atualizado para "Pago".

### Fluxo Principal

1. O usuário seleciona o aluno e a fatura.
2. O sistema registra o método de pagamento (Pix, Cartão, Dinheiro).
3. O sistema emite o recibo digital.

### RF Relacionados

* RF08: Fluxo financeiro PDV.

<img width="315" height="358" alt="image" src="https://github.com/user-attachments/assets/a20e213a-b720-4ac2-90fd-6ccbcb798d9b" />



---

## UC09 — Agendar Aula Coletiva

### Ator Principal

Aluno

### Objetivo

Reservar vaga em aulas com limite de participantes.

### Pré-condições

* Existência de vagas disponíveis.

### Fluxo Principal

1. O aluno escolhe a aula e o horário no aplicativo.
2. O sistema valida a disponibilidade de vaga.
3. O sistema confirma o agendamento.

### Fluxos Alternativos

* **A1 — Lista de espera:** O sistema oferece inclusão em lista se a aula estiver lotada.

### RF Relacionados

* RF09: Reserva de horários.

<img width="511" height="431" alt="image" src="https://github.com/user-attachments/assets/c5406556-b0b2-4e77-b14f-94537fbc2017" />



---

## UC10 — Consultar Histórico de Frequência

### Ator Principal

Aluno / Administrador

### Objetivo

Visualizar a assiduidade do aluno na academia.

### Fluxo Principal

1. O usuário seleciona o período desejado.
2. O sistema lista todos os dias e horários de entrada registrados.

<img width="286" height="248" alt="image" src="https://github.com/user-attachments/assets/9efe9946-e0d8-4a79-a246-1f21cedc519c" />



---

## UC11 — Bloquear Aluno por Inadimplência

### Ator Principal

Sistema (Automático)

### Objetivo

Suspender o acesso de alunos com atrasos financeiros.

### Pré-condições

* Data de vencimento ultrapassada.

### Pós-condições

* Matrícula suspensa para entrada.

### Fluxo Principal

1. O sistema verifica diariamente as faturas vencidas.
2. O sistema altera o status da matrícula para "Bloqueado".
3. O sistema envia uma notificação automática ao aluno.

<img width="284" height="303" alt="image" src="https://github.com/user-attachments/assets/12c47ecc-f5ce-4be7-8b7c-bf3224618309" />



---

## UC12 — Cadastrar Exercício no Catálogo

### Ator Principal

Administrador / Instrutor

### Objetivo

Alimentar o banco de dados de exercícios com fotos ou vídeos.

### Fluxo Principal

1. O usuário insere nome, grupo muscular e link do vídeo.
2. O sistema salva o exercício para uso na montagem de fichas.
<img width="231" height="248" alt="image" src="https://github.com/user-attachments/assets/ae0bb91b-1bea-4a31-9055-f2650011394a" />


---

## UC13 — Emitir Relatório de Faturamento

### Ator Principal

Administrador

### Objetivo

Gerar visão financeira de recebimentos mensais.

### Fluxo Principal

1. O usuário filtra o período (mês/ano).
2. O sistema soma os pagamentos confirmados.
3. O sistema exibe o total por categoria de plano.
<img width="352" height="303" alt="image" src="https://github.com/user-attachments/assets/5b7806af-a990-4a11-9a6f-e8f27ffe7818" />


---

## UC14 — Notificar Vencimento de Plano

### Ator Principal

Sistema (Automático)

### Objetivo

Alertar o aluno antes da expiração do plano.

### Fluxo Principal

1. O sistema identifica planos que vencem em 5 dias.
2. O sistema envia notificação Push para o celular do aluno.
<img width="334" height="303" alt="image" src="https://github.com/user-attachments/assets/ea3bafb2-daba-4e85-bd2a-75352cb301d9" />


---

## UC15 — Gerenciar Horários de Professores

### Ator Principal

Administrador

### Objetivo

Escalar instrutores para turnos e aulas coletivas.
<img width="287" height="303" alt="image" src="https://github.com/user-attachments/assets/e7233932-265c-4c50-956c-c819d4c3cba9" />


---

## UC16 — Cancelar Matrícula

### Ator Principal

Recepcionista

### Objetivo

Encerrar o vínculo contratual do aluno.

### RN Relacionadas

* RN05: Verificar se existem multas de rescisão para planos anuais.
<img width="286" height="576" alt="image" src="https://github.com/user-attachments/assets/50bd64e6-0454-4f0d-93ed-7a9d2a4db8a2" />

---

## UC17 — Vender Produtos (Loja)

### Ator Principal

Vendedor / Recepcionista

### Objetivo

Vender suplementos, água ou acessórios.
<img width="221" height="303" alt="image" src="https://github.com/user-attachments/assets/f2afa7db-5c10-4bb6-9af4-a56d1ba889ad" />

---

## UC18 — Alterar Senha de Acesso

### Ator Principal

Usuário

### Objetivo

Permitir a atualização da senha pessoal.
<img width="318" height="312" alt="image" src="https://github.com/user-attachments/assets/83c2f5ea-1d63-41ff-b7fc-12da1e0e5228" />

---

## UC19 — Exportar PDF de Avaliação Física

### Ator Principal

Aluno / Instrutor

### Objetivo

Gerar documento para impressão.

### Fluxo Principal

1. O usuário seleciona a avaliação desejada.
2. O sistema gera um arquivo .PDF formatado.
<img width="324" height="303" alt="image" src="https://github.com/user-attachments/assets/0453f5d6-87bc-48f4-be07-cd23a3f746fa" />

---

## UC20 — Configurar Unidade

### Ator Principal

Administrador

### Objetivo

Definir dados da unidade (São João da Boa Vista), horários e logotipos.
<img width="310" height="303" alt="image" src="https://github.com/user-attachments/assets/2b50cda5-bcc4-46df-9a4c-5207a509acb6" />

---
### DUC_MiguelTuratti_LuisVasconcellos
<img width="501" height="1948" alt="image" src="https://github.com/user-attachments/assets/2f5077da-8e56-4fb9-8d16-719859b81fb6" />




## Issues Relacionadas
> **Atenção:** As Issues devem ser **apenas referenciadas** — não utilize termos como *closes*, *fixes*, *resolve*.

- Relacionado à Issue **#1 – Documento de Casos de Uso**
- Relacionado à Issue **#2 – Diagrama de Casos de Uso**

## Checklist Antes do Envio

Marque cada linha após confirmar:

- [x] O documento contém **20 casos de uso completos**, seguindo o template do arquivo `/docs/casosdeuso.md`
- [x] O nome do arquivo segue o padrão exigido
- [x] Os diagramas representam **todos os casos de uso listados** no documento
- [x] Todos os diagramas estão em **formato PNG**
- [x] As Issues foram referenciadas corretamente
- [x] O PR contém **apenas** os arquivos exigidos

## Observações (Opcional)
Use este espaço caso queira explicar alguma decisão, dúvida ou comentário adicional.
