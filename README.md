# Sistema Bancário em Python
Descrição
Este projeto implementa um sistema bancário simples em Python, permitindo a criação e gerenciamento de contas correntes para clientes pessoa física. O sistema suporta operações como depósito, saque, consulta de extrato, criação de novos clientes e contas, além de listar todas as contas existentes.
Funcionalidades

Criação de Clientes: Cadastro de clientes pessoa física com informações como nome, CPF, data de nascimento e endereço.
Criação de Contas: Criação de contas correntes vinculadas a clientes, com limite de saques e valor máximo por saque.
Depósito: Permite depositar valores positivos em uma conta.
Saque: Permite sacar valores, respeitando limites de saldo, valor máximo por saque (R$500) e número máximo de saques diários (50).
Extrato: Exibe o histórico de transações (depósitos e saques) e o saldo atual da conta.
Listagem de Contas: Lista todas as contas registradas com informações como agência, número, titular e saldo.
Limite de Transações: Restringe o número de transações por dia a duas por conta.

Estrutura do Código
O código é organizado em classes que representam as entidades e funcionalidades do sistema bancário:

Cliente: Classe base para clientes, com suporte à adição de contas e realização de transações.
PessoaFisica: Herda de Cliente, representando um cliente pessoa física com atributos como nome, CPF, data de nascimento e endereço.
Conta: Classe base para contas, com métodos para depósito, saque e histórico de transações.
ContaCorrente: Herda de Conta, adicionando limites de saque (valor e quantidade).
Historico: Gerencia o histórico de transações de uma conta, com suporte a relatórios e contagem de transações diárias.
Transacao: Classe abstrata para transações (depósito e saque).
Saque e Deposito: Implementações concretas de transações.
contasIterador: Iterador para listar contas de forma formatada.
Funções de Interface: Funções como menu, depositar, sacar, exibirExtrato, criarCliente, criarConta e listarContas para interação com o usuário.

Como Executar

Pré-requisitos: Python 3.x instalado.
Clonar o Repositório:git clone <URL_DO_REPOSITORIO>
cd <NOME_DO_REPOSITORIO>


Executar o Programa:python main.py


Interagir com o Menu: Escolha as opções disponíveis no menu para realizar operações como depósito, saque, extrato, criação de cliente ou conta, listagem de contas ou sair.

Exemplo de Uso

Execute o programa.
No menu, selecione [nu] para criar um novo usuário, informando CPF, nome, data de nascimento e endereço.
Selecione [nc] para criar uma nova conta vinculada ao CPF do cliente.
Use [d] para depositar, [s] para sacar, ou [e] para consultar o extrato.
Use [lc] para listar todas as contas.
Selecione [q] para sair.

Limitações

O sistema não persiste dados (os dados são armazenados em memória e perdidos ao encerrar o programa).
Apenas uma conta por cliente é selecionada automaticamente para transações (não há escolha de conta).
O limite de saques diários é fixo em 50, e o limite de transações por dia é 2 por conta.

Possíveis Melhorias

Adicionar persistência de dados (ex.: salvar em arquivo ou banco de dados).
Permitir que o cliente escolha qual conta usar em transações.
Implementar autenticação para maior segurança.
Adicionar suporte a outros tipos de contas (ex.: conta poupança).

Contribuição

Faça um fork do repositório.
Crie uma branch para sua feature (git checkout -b feature/nova-funcionalidade).
Commit suas alterações (git commit -m 'Adiciona nova funcionalidade').
Envie para o repositório remoto (git push origin feature/nova-funcionalidade).
Abra um Pull Request.

Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
