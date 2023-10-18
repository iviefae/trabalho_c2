Esse sistema lida com informações de clientes, contas bancárias e movimentações bancárias. A estrutura geral do código principal.py e suas principais funções que consistem em:

**Importação de Módulos**:

O código começa importando vários módulos do pacote `utils`, `reports`, e `controller`, que contêm funcionalidades auxiliares para a aplicação.

**Instanciação de Objetos**:

Depois das importações, são criadas instâncias de várias classes, como `SplashScreen`, `Relatorio`, `Controller_Cliente`, `Controller_Conta`, e `Controller_Movimentacao`. Essas instâncias provavelmente serão usadas para interagir com as funcionalidades do sistema.

**Funções**:

O código define quatro funções principais: `reports`, `inserir`, `atualizar`, e `excluir`. Cada uma dessas funções aceita um argumento `opcao` que determina qual funcionalidade do sistema será acionada.

`reports(opcao_relatorio)`: Esta função gera relatórios com base na opção selecionada. Dependendo do valor de `opcao_relatorio`, ela chama diferentes métodos do objeto `relatorio` para gerar relatórios sobre clientes, contas, movimentações, tipos de contas por cliente ou saldo e quantidade de movimentações por conta.

inserir(opcao_inserir)`: Esta função permite a inserção de novos registros no sistema. Dependendo da opção selecionada, ela chama métodos de objetos como `ctrl_cliente`, `ctrl_conta`, ou `ctrl_movimentacao` para inserir um novo cliente, conta ou movimentação.

atualizar(opcao_atualizar)`: Esta função lida com a atualização de registros. Ela exibe relatórios (por meio do objeto `relatorio`) e permite a atualização de informações de clientes, contas ou movimentações.

`excluir(opcao_excluir)`: Similar às funções anteriores, esta função permite a exclusão de registros. Ela exibe relatórios e permite a exclusão de clientes, contas ou movimentações.

**Função `run`**:

A função `run` é o ponto de entrada da aplicação. Ela exibe uma tela inicial, depois entra em um loop que permite que o usuário escolha entre diferentes opções. Dependendo da opção escolhida, as funções `reports`, `inserir`, `atualizar` ou `excluir` são chamadas. O loop continua até que o usuário selecione a opção de sair, encerrando o programa.

**Seção `if __name__ == "__main__":`**:

A seção final verifica se o script está sendo executado como um programa independente (não importado como um módulo) e, nesse caso, chama a função `run` para iniciar a aplicação.