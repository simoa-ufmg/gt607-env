## Instalação do Anaconda

Faça o download da distribuição do Anaconda para o Windows no seguinte link https://www.anaconda.com/products/distribution.
Ao instalar o Anaconda, escolha "instalar somente para mim" ao invés de "instalar para todos os usuários", pois isso irá simplificar a instalação de outros pacotes necessários.

## Instalação do exiftool e definição como variável de ambiente

Baixe o executável para Windows do exiftool em https://exiftool.org e descompacte-o para um algum diretório que for conveniente, como o C:\exiftool. Agora é preciso informar ao código em Python onde encontrar o exiftool (para não termos que configurá-lo em cada script que escrevemos), isso é feito adicionando o caminho para o exiftool como uma variável de ambiente.
Isso pode ser feito no Windows da seguinte maneira:

- Crie uma variável de ambiente chamada exiftoolpath com um valor do caminho completo para o exiftool. Por exemplo, C:\exiftool\exiftool.exe

- Clique com o botão direito do mouse em Meu Computador e clique em Propriedades.

- Clique na guia Avançado.

- Clique em Variáveis de ambiente.

- Clique em Nova para adicionar um novo nome e valor de variável.

- Nomeie a variável como exiftoolpath

- No valor da variável coloque C:\exiftool\exiftool.exe

## Criação do Ambiente

Abra um console Anaconda no modo administrador no menu Iniciar como administrador e execute os seguintes comandos no console:

```shell
cd <caminho do diretório para o qual você clonou este repositório>
conda env create -f gt607_conda_env.yml
```

Essa sequência irá configurar um ambiente anaconda com todas as ferramentas e bibliotecas necessárias para executar as ferramentas de processamento e modelagem do GT-607.
Quando estiver pronto, executar o comando

```shell
conda activate gt607
```

Para ativar o ambiente configurado.

Cada vez que você for usar as ferramentas disponibilizadas pelo GT-607 será necessário executar o comando acima de ativação do ambiente.
