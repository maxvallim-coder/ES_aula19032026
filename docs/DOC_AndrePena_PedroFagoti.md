# Documento de Modelagem - FitPass Gym Management

---

# 1. Diagrama de Casos de Uso (Descrição Geral)

**Atores:**
- Usuário (Aluno)
- Recepcionista
- Instrutor
- Gerente
- Sistema de Pagamento
- Catraca (RFID)

**Casos de Uso:**
- UC01 - Realizar Login  
- UC02 - Cadastrar Aluno  
- UC03 - Gerenciar Planos  
- UC04 - Registrar Pagamento  
- UC05 - Validar Acesso  
- UC06 - Agendar Aula  
- UC07 - Registrar Presença  
- UC08 - Registrar Avaliação Física  
- UC09 - Emitir Relatórios  
- UC10 - Enviar Notificações  

---

# 2. Casos de Uso + Diagramas de Atividade

---

## UC01 - Realizar Login

**Ator Principal:** Usuário  
**Objetivo:** Permitir acesso ao sistema  

**Pré-condições:**
- Usuário cadastrado

**Pós-condições:**
- Sessão iniciada

**Fluxo Principal:**
1. Usuário informa e-mail e senha  
2. Sistema valida credenciais  
3. Sistema autentica e redireciona  

**Fluxos Alternativos:**
- A1: Senha incorreta - exibe erro  
- A2: Conta bloqueada - impede acesso  

**RF:** RF01  
**RN:** RN06  
**RNF:** RNF02  

### Diagrama de Atividade
@startuml
start
:Usuário informa e-mail e senha;
:Sistema valida credenciais;

if (Válidas?) then (sim)
  :Redireciona dashboard;
else
  :Exibe erro;
endif

stop
@enduml
