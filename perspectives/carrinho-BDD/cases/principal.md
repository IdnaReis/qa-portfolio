# 🛒 Projeto de Testes Manuais com BDD – Carrinho de Compras (E-commerce)

Este projeto aplica **BDD (Behavior Driven Development)** para estruturar casos de teste de forma clara e colaborativa, usando a linguagem **Gherkin**.

---

## 🎯 Objetivo
Validar a funcionalidade do carrinho de compras garantindo que os produtos possam ser adicionados, removidos, atualizados e que o valor total seja calculado corretamente.

---

## 📋 Cenários de Teste (BDD)

### Funcionalidade: Carrinho de Compras
**Como** cliente de um e-commerce  
**Quero** gerenciar meu carrinho de compras  
**Para** finalizar pedidos com segurança e precisão  

---

### Cenário: Adicionar produto ao carrinho
```gherkin
Given que o produto está disponível em estoque
When o usuário clica em "Adicionar ao carrinho"
Then o produto deve aparecer no carrinho com preço correto
```

### Cenário: Remover produto do carrinho
```gherkin
Given que o carrinho possui pelo menos um produto
When o usuário clica em "Remover"
Then o produto deve ser removido e o carrinho atualizado
```

### Cenário: Atualizar quantidade de produto
```gherkin
Given que o carrinho possui um produto
When o usuário altera a quantidade de 1 para 3
Then o sistema deve atualizar a quantidade e recalcular o valor corretamente
```

### Cenário: Calcular valor total
```gherkin
Given que o carrinho possui múltiplos produtos
When o usuário acessa o carrinho
Then o sistema deve exibir a soma correta dos valores dos produtos
```

### Cenário: Carrinho vazio
```gherkin
Given que o carrinho não possui produtos
When o usuário acessa o carrinho
Then o sistema deve exibir a mensagem "Seu carrinho está vazio"
```

















