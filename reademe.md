# Bootcamp DIO - Python AI Backend Developer
21/06/2024

## Objetivo Geral

Separar as funções existentes de saque, depósito e extrato em funções. Criar duas novas funções: cadastrar usuário (cliente) e cadastrar conta bancária

## Desafio DIO

Precisamos deixar nosso código mais modularizado, para isso vamos criar funções para as operações existentes: sacar, depositar e visualizar histórico. Além disso, para a versão 2 do nosso sistema, precisamos criar duas novas funções: criar usuário (cliente do banco) e criar conta corrente (vincular com usuário).

### Separação em funções

Devemos criar funções para todas as operações do sistema. Para exercitar tudo o que aprendemos neste módulo, cad função vai ter uma regra na passagem de argumentos. O retorno e a forma como serão chamadas, pode ser definida por você da forma que achar melhor.

### Operações de saque

A função de saque deve receber os argumentos apenas por nome (keyword only). Sugestão de argumentos: saldo, valor, extrato, limite, numero_saques, limite_saques. Sugestão de retorno: saldo e extrato.

### Operações de deposito

A função de depósito deve receber os argumentos apenas por posição (positional only). Sugestão de argumentos: saldo, valor, extrato. Sugestão de retorno: saldo e extrato.


### Operação de extrato

A função extrato deve receber os argumentos por posição e nome (positional only e keyword only). Argumentos posicionais: saldo. Argumentos nomeados: extrato.

### Novas funções

Precisamos criar duas novas funções: criar usuário e criar conta corrente. Fique a vontade para adicionar mais funções, exemplo listar contas, inativar contas, deletar contas etc.

- Criar usuários (cliente):
  O programa deve armazenar os usuários em uma lista, usuário é composto por nome, data de nascimento, cpf e endereço. O endereço é uma string com o formato: logradouro, nro, bairro, cidade e sigla do estado (exibição: logradouro, nro - bairro - cidade/uf). Deve ser armazenado somente os números do CPF. Não podemos cadastrar 2 usuários com o mesmo CPF.
<br>

- Criar conta corrente:
  O programa deve armazenar contas em uma lista, uma conta é composta por: agência, número da conta e usuário. O número da conta é sequencial, iniciando em 1. O número da agência é fixo "0001". O usuário pode ter mais de uma conta, mas uma conta pertence a somente um usuário.

# Dica

Para vincular um usuário a uma conta, filtre a lista de usuários buscando o número do CPF informado para cada usuário da lista.

Os valores devem ser exibidos utilizando o formato R$ xxx.xx, exemplo:

1500.45 = R$ 1500.45
