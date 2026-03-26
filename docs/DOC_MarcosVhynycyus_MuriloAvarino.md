
# 📘 FitPass Gym Management — Documento de Casos de Uso

---

# 🧩 Diagrama de Casos de Uso

<img width="758" height="794" alt="DUC_MarcosVhynycyus_MuriloAvarino" src="https://github.com/user-attachments/assets/7a882457-e74e-46a4-a9d3-3ed5e4fc6efc" />



---

# 📑 Casos de Uso

---

## 🔹 UC01 — Cadastrar Aluno

**Ator:** Recepcionista  

**Descrição:** Cadastro de novos alunos  

**Pré-condição:** Usuário autenticado  

**Pós-condição:** Aluno registrado  

### Fluxo Principal
1. Acessa módulo de alunos  
2. Seleciona cadastrar  
3. Informa dados  
4. Sistema valida  
5. Sistema salva  

### Fluxo Alternativo
- Dados inválidos → solicitar correção  

### 🔄 Diagrama de Atividade

<img width="233" height="312" alt="image" src="https://github.com/user-attachments/assets/e2c181ef-ab87-49ab-bb88-381ec4ae1987" />


---

## 🔹 UC02 — Gerenciar Planos

**Ator:** Gerente  

### Fluxo Principal
1. Acessa módulo  
2. Cria/edita plano  
3. Salva alterações  

### 🔄 Diagrama de Atividade

<img width="138" height="248" alt="image" src="https://github.com/user-attachments/assets/8f13c319-3638-45ee-9e6f-1b6d2dab9a53" />


---

## 🔹 UC03 — Registrar Pagamento

**Ator:** Recepcionista  

### Fluxo Principal
1. Buscar aluno  
2. Registrar pagamento  
3. Confirmar  
4. Atualizar regularidade  

### 🔄 Diagrama de Atividade

<img width="161" height="248" alt="image" src="https://github.com/user-attachments/assets/e00b322a-313b-461c-922d-cd894a65b091" />


---

## 🔹 UC04 — Verificar Regularidade

**Ator:** Sistema  

### Fluxo Principal
1. Verifica vencimento  
2. Verifica pagamentos  
3. Define status  

### 🔄 Diagrama de Atividade

<img width="159" height="248" alt="image" src="https://github.com/user-attachments/assets/5f4ad287-4181-4556-85a4-7ad303bf187b" />


---

## 🔹 UC05 — Validar Acesso

**Atores:** Aluno / Catraca  

### Fluxo Principal
1. Aproxima RFID  
2. Consulta sistema  
3. Verifica regularidade  
4. Autoriza ou bloqueia  

### 🔄 Diagrama de Atividade

<img width="259" height="312" alt="image" src="https://github.com/user-attachments/assets/0f2630c8-1769-464f-921f-921500187449" />


---

## 🔹 UC06 — Consultar Horários

**Ator:** Aluno  

### Fluxo Principal
1. Acessa agenda  
2. Visualiza aulas  

### 🔄 Diagrama de Atividade

<img width="132" height="193" alt="image" src="https://github.com/user-attachments/assets/82a72bc7-3851-4f16-b0d8-d3f99a8765aa" />


---

## 🔹 UC07 — Agendar Aula

**Ator:** Aluno  

### Fluxo Principal
1. Seleciona aula  
2. Verifica vagas  
3. Confirma  

### Fluxo Alternativo
- Aula lotada  

### 🔄 Diagrama de Atividade

<img width="302" height="367" alt="image" src="https://github.com/user-attachments/assets/08eca142-a33a-4af9-8110-cd44e6b96b15" />


---

## 🔹 UC08 — Cancelar Agendamento

**Ator:** Aluno  

### Fluxo Principal
1. Acessa reservas  
2. Cancela  
3. Confirma  

### 🔄 Diagrama de Atividade

<img width="343" height="257" alt="image" src="https://github.com/user-attachments/assets/4e5e2d40-4448-4d52-9bba-08feeb517173" />


---

## 🔹 UC09 — Registrar Presença

**Ator:** Instrutor  

### Fluxo Principal
1. Acessa aula  
2. Marca presença  

### 🔄 Diagrama de Atividade

<img width="148" height="193" alt="image" src="https://github.com/user-attachments/assets/90cf5a4b-aa59-4d50-b10c-e787f02dab69" />


---

## 🔹 UC10 — Registrar Avaliação Física

**Ator:** Instrutor  

### Fluxo Principal
1. Seleciona aluno  
2. Verifica regularidade  
3. Registra dados  

### 🔄 Diagrama de Atividade

<img width="235" height="422" alt="image" src="https://github.com/user-attachments/assets/3c735496-6bd8-437e-9438-8a926ea1854f" />


---

## 🔹 UC11 — Anexar Arquivo de Avaliação

**Ator:** Instrutor  

### Fluxo Principal
1. Adiciona arquivo  
2. Sistema armazena  

### 🔄 Diagrama de Atividade

<img width="144" height="248" alt="image" src="https://github.com/user-attachments/assets/eccfcafa-108d-4770-a26f-4f71a9e54352" />


---

## 🔹 UC12–UC15 — Emitir Relatórios

**Ator:** Gerente  

### Tipos:
- Inadimplência  
- Alunos ativos  
- Acessos  
- Ocupação  

### 🔄 Diagrama de Atividade

<img width="189" height="303" alt="image" src="https://github.com/user-attachments/assets/d0a88598-348b-498f-bd54-14d0dffdf041" />


---

## 🔹 UC16–UC18 — Notificações

**Ator:** Sistema  

### Fluxo Principal
1. Detecta evento  
2. Envia notificação  

### 🔄 Diagrama de Atividade

<img width="138" height="248" alt="image" src="https://github.com/user-attachments/assets/bf7e9326-e802-44a8-b8f4-830030a92582" />


---

## 🔹 UC19 — Atualizar Regularidade

**Ator:** Sistema  

### Fluxo Principal
1. Recebe pagamento  
2. Atualiza status  

### 🔄 Diagrama de Atividade

<img width="155" height="193" alt="image" src="https://github.com/user-attachments/assets/85537c86-731e-4081-a30a-d51462e6dbb4" />


---

## 🔹 UC20 — Autenticar Usuário

**Atores:** Funcionários  

### Fluxo Principal
1. Inserir login  
2. Validar credenciais  
3. Liberar acesso  

### 🔄 Diagrama de Atividade

<img width="243" height="312" alt="image" src="https://github.com/user-attachments/assets/1b06f817-25fd-4f45-9897-68277f61089b" />


---

# 🔷 Fluxo Geral do Sistema (Opcional)

<img width="235" height="303" alt="image" src="https://github.com/user-attachments/assets/fea4f564-4696-438a-b978-04b13dfaf06c" />
