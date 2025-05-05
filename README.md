# Estudo: Criação de Máquina Virtual na Azure

A criação de uma máquina virtual (VM) na Azure pode ser feita com o objetivo de **testes** ou **produção**. O processo envolve diversas configurações, algumas das quais podem ser predefinidas para facilitar a criação. Abaixo estão os principais parâmetros e etapas envolvidos:

---

## 1. Configurações Iniciais

- **Assinatura:** Escolha da assinatura vinculada à conta.
- **Grupo de Recursos:** Define o agrupamento lógico dos recursos da Azure.
- **Nome da Máquina Virtual**
- **Região:** Local geográfico onde a VM será criada.
- **Zona de Disponibilidade:** Define a redundância geográfica.
- **Opções de Disponibilidade:**
  - Conjunto de disponibilidade
  - Conjunto de dimensionamento de máquinas virtuais (VM Scale Set)

---

## 2. Segurança e Acesso

- **Tipo de Segurança:** Padrão ou personalizada.
- **Chaves SSH:** Para acesso seguro via terminal.
- **Grupo de Segurança de Rede (NSG):** Controle de tráfego de entrada e saída da VM.

---

## 3. Imagem e Instanciamento

- **Imagem:** Escolha do sistema operacional (ex: Windows, Linux).
- **Contagem de Instâncias:**
  - Padrão: 2 instâncias
  - Pode ser ajustado via **dimensionamento automático (autoscale)**

---

## 4. Escalonamento Automático

- **Critério de Escalonamento:** Por padrão, baseado no uso da CPU:
  - Escalonamento para **cima**: uso de CPU > 80%
  - Escalonamento para **baixo**: uso de CPU < 20%
- **Duração da Consulta (Cool-down):** Padrão de 10 minutos.

---
