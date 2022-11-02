REMIX DEFAULT WORKSPACE

O espaço de trabalho padrão do Remix está presente quando:
eu. Remixar cargas pela primeira vez
ii. Um novo espaço de trabalho é criado com o modelo 'Padrão'
iii. Não há arquivos existentes no Explorador de Arquivos

Esta área de trabalho contém 3 diretórios:

1. 'contratos': Possui três contratos com níveis crescentes de complexidade.
2. 'scripts': Contém quatro arquivos typescript para implantar um contrato. Está explicado abaixo.
3. 'testes': Contém um arquivo de teste Solidity para o contrato 'Ballot' e um arquivo de teste JS para o contrato 'Storage'.

SCRIPTS

A pasta 'scripts' tem quatro arquivos typescript que ajudam a implantar o contrato 'Storage' usando as bibliotecas 'web3.js' e 'ethers.js'.

Para a implantação de qualquer outro contrato, basta atualizar o nome do contrato de 'Storage' para o contrato desejado e fornecer os argumentos do construtor de acordo
no arquivo `deploy_with_ethers.ts` ou `deploy_with_web3.ts`

Na pasta 'tests' existe um script contendo testes unitários do Mocha-Chai para o contrato 'Storage'.

Para executar um script, clique com o botão direito do mouse no nome do arquivo no explorador de arquivos e clique em 'Executar'. Lembre-se, o arquivo Solidity já deve estar compilado.
A saída do script aparecerá no terminal remix.

Observe que exigir/importar é suportado de maneira limitada para módulos compatíveis com Remix.
Por enquanto, os módulos suportados pelo Remix são ethers, web3, swarmgw, chai, multihashes, remix e hardhat apenas para objeto/plugin hardhat.ethers.
Para módulos não suportados, um erro como este será gerado: '<module_name> module require is not supported by Remix IDE' será mostrado.


