# apt-menu versão 1.0
Um pequeno menu em Bash Script para o gerenciamento básico e buscas nos pacotes do Debian e derivados. O script foi originalmente pensado como um recurso didático, tanto para exercitar a programação em Shell/Bash Script, quanto para demonstrar o uso do `apt` e alguns de seus comandos mais comuns.

## Opções

O `apt-menu` trabalha com as seguintes opções:

1. Atualização do cachê de pacotes:  
`sudo apt update`
2. Listagem dos pacotes marcados para atualização  
`apt list --upgradable`
3. Instalação das atualizações marcadas:  
`sudo apt upgrade`
4. Remoção de pacotes obsoletos:  
`sudo apt autoclean`
5. Remoção de dependências sem uso:  
`sudo apt autoremove`
6. Busca por pacotes disponíveis no cachê:  
`apt-cache search <termos de busca>`
7. Busca de informações sobre pacotes no cachê:  
`apt-cache show <nome do pacote>`
8. Listagem de todos os pacotes instalados:
`apt list --installed`

São, portanto, as opções mais utilizadas além dos comandos de instalação e remoção de pacotes (que, por questões de segurança, ficaram de fora do nosso menu).

Existe ainda uma última opção, que é a opção **Utilizar o terminal**, para que o usuário possa executar qualquer operação na linha de comandos e retornar ao menu (com o comando `exit`) quando quiser continuar.

## Dependências

O `apt-menu` só funciona em sistemas baseados em **Debian** que usem o `apt` e o `apt-get` para gerenciar pacotes pelo terminal. Fora isso, a única dependência que não vem instalada por padrão na maioria dessas distribuições é o *fuzzy finder* (`fzf`), que pode ser instalado facilmente com o comando:

```
sudo apt install fzf
```

## Instalação

Basta clonar o repositório, entrar pelo terminal na pasta onde ele foi clonado e executar o script.

```
git clone https://github.com/debxp/apt-menu.git
cd apt-menu
./apt-menu
```

Alternativamente, você pode [baixar o repositório zipado](https://github.com/debxp/apt-menu/archive/master.zip), extrai-lo onde desejar e executar o script pelo terminal.

## Como contribuir

O `apt-menu` é um script didático que objetiva exercitar a programação em Shell/Bash e os comandos do `apt`. Sendo assim, você pode colaborar com as suas opiniões, dúvidas e sugestões nas [**Issues** do projeto no GitHub](https://github.com/debxp/apt-menu/issues).
