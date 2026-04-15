# ⛓️ TypeScript Blockchain

Uma implementação simples de **Blockchain desenvolvida em TypeScript** com fins educacionais.  
Este projeto demonstra os principais conceitos por trás da tecnologia blockchain, como **blocos, hashes criptográficos, encadeamento de blocos, mineração e prova de trabalho (Proof of Work)**.

O objetivo é mostrar **como uma blockchain funciona internamente**, sem depender de frameworks ou bibliotecas complexas.

---

# 📚 Conceitos Implementados

Este projeto aborda os principais fundamentos de uma blockchain:

- 🔗 Estrutura de **Blocos**
- 🔐 **Hash criptográfico (SHA-256)**
- ⛏️ **Mineração de blocos**
- ⚙️ **Proof of Work**
- 📦 **Encadeamento de blocos via hash**
- 🛡️ **Validação da integridade da blockchain**

---

# ⚙️ Como Funciona

Cada **bloco** contém:

- Timestamp
- Dados
- Hash do bloco anterior
- Hash do bloco atual
- Nonce (usado na mineração)

Exemplo de estrutura de um bloco:

<img width="1149" height="685" alt="image" src="https://github.com/user-attachments/assets/0d1b2e90-1bb2-4381-8271-51f2b5c67873" />


```ts

export interface Bloco {
    header: {
        nonce: number
        hashBloco: string
    }
    payload: {
        sequencia: number
        timestamp: number
        dados: any
        hashAnterior: string
    }
}
