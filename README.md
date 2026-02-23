# 🧠 Técnicas de Teste | Cenários a partir de Regras de Negócio (EBAC)

Projeto desenvolvido como parte do módulo **Técnicas de Testes** na formação de **Quality Assurance (QA)** da EBAC, com foco em transformar **regras de negócio** em **cenários de teste completos**, aplicando técnicas clássicas de testes de caixa-preta.

---

## 🎯 Objetivo

Praticar a identificação e documentação de cenários de teste usando:

- Partição de Equivalência
- Valor Limite
- Tabela de Decisão
- Transição de Estado

A partir de regras de negócio, garantindo cobertura e clareza na definição dos testes.

---

## 🛠️ Técnicas aplicadas

### 1) Partição de Equivalência
Aplicada para dividir entradas em classes **válidas** e **inválidas**, reduzindo redundância e garantindo cobertura.

Regras cobertas (exemplos):
- RN01: valores entre **R$19,00 e R$99,00**
- RN02: renovação de produtos com cadastro há **mais de 30 dias**
- RN03: cadastro máximo de **100 itens por vez** 

---

### 2) Valor Limite
Aplicada para validar o comportamento do sistema nos pontos críticos de borda.

Cobertura de limites (exemplos):
- RN01: **18,99 / 19,00 / 19,01** e **98,99 / 99,00 / 99,01**
- RN03: **99 / 100 / 101 itens** 

---

### 3) Tabela de Decisão
Aplicada para mapear combinações de condições e suas ações esperadas, garantindo cobertura dos cenários possíveis.

Condições avaliadas:
- RN02: produto com **> 30 dias**
- RN03: quantidade **<= 100**
Ações esperadas:
- Renovar?
- Cadastrar? 

---

### 4) Transição de Estado
Aplicada para validar comportamentos dependentes do estado anterior do sistema.

Tema aplicado no exercício:
**Rede Social — Conta de usuário existente**

Estados analisados:
- Conta ativa
- Conta desativada
- Conta banida
- Tentativa de login (bloqueada quando banida)

Fluxos definidos (exemplos):
- Ativa → Desativada
- Desativada → Ativa
- (Ativa/Desativada) → Banida
- Banida → (estado anterior) via recurso aceito
- Banida → Banida (tentativa de login deve bloquear) 

---

## 📄 Entrega

O documento contém:
- Regras analisadas (RN01, RN02, RN03)
- Cenários de teste por técnica
- Tabelas e fluxos com resultado esperado

---

## 🧠 Competências demonstradas

- Leitura e interpretação de regras de negócio
- Criação de cenários de teste com boa cobertura
- Raciocínio analítico e atenção a detalhes
- Aplicação prática de técnicas de caixa-preta
- Organização e documentação clara

