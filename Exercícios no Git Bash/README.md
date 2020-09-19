1. Começando no Git Bash
2. Vamos configurar o Git Bash?
3. Como encontar um projeto localmente (sua máquina física)?
4. Como enviar seu repositório local para o repositório hospedado?
5. Clonando repositórios
6. Atualizar seu repositório local
7. Contribuindo com um projeto
8. Verificar conflitos


### Começando no Git Bash

Vamos começar? Clique com o botão direito do mouse e selecione **Git Bash here**

Como funciona? As ações são realizadas por linha de comando. Segue alguns termos utilizados!

`pwd` (*path working directory*) - mostra o caminho que você se encontra.
`ls` (*list*) - lista o que tem na pasta atual.
`mkdir` (*make a directory*) - cria uma nova pasta, para isso é necessário informar o nome da nova pasta `mkdir PastaNova`.
`cd` (*change directory*) - usado para entrar em uma pasta, para isso é necessário informar o nome da pasta `cd Pasta2`.
`cd ..` - volta uma pasta.
`echo`(*echo*) - cria um arquivo, para isso é necessário informar o nome do arquivo.
`rm` (*remove*) - deleta um arquivo, por exemplo: `rm PastaNova`.
`rm -r` ou `rm --recursive`(deleta uma pasta), por exemplo `rm -r PastaNova`.


### Vamos configurar o Git Bash?

Para isso você irá configurar o Git com seu `user.name` e `user.email`. Para isso os comandos utilizados são:

- `git config --global user.name "Instituto HUB"`
- `git config --global user.email "email@email.com.br"`

Para verificar se funcionou use o comando:
- `git config --list`


### Como encontar um projeto localmente (sua máquina física)?

Você pode usar o botão direito dentro do Git Bash ou usar `cd nome da Pasta` e em seguida utilizar os comandos:

- `git init`- inicia um repositório na pasta que você está.
- `git add <nome do arquivo>` ou `git add --all` ou `git add .` - adiciona arquivos no repositório iniciado.
- `git commit -m "Mensagem de commit"`- adicionar uma mensagem sobre a alteração do arquivo é uma boa prática.

### Como enviar seu repositório local para o repositório hospedado?

- Entre no seu repositório no site ou crie um repositório novo no site em seguida no Git Bash:

- `git remote add origin link`- adicionando o endereço do repositório remoto.
- `git push -u origin master` - enviando do Git local para o GitHub.



### Clonando repositórios
- Entre no repositório desejado.
- Copie o link http que aparece ao clicar no botão **Code**.
- Na sua máquina abra o Git Bash até a pasta desejada.
- `git clone link`
- `cd ` - para entrar na pasta do repositório clonado, lembre-se precisa chamar o nome do repositório, por exemplo: `cd Novo_Repositorio `.
- `ls`: para listar o que tem dentro da pasta.


### Atualizar seu repositório local
- Entrar no Git Bash dentro da pasta que deseja atualizar.
- `git remote -v`- verifica se o endereço remoto está correto.
- `git checkout master`- volta para a pasta principal.
- `git pull origin master`- atualiza a branch `master` conforme endereço `origin`.
- `git branch -d ex-aula-seuNome`- deleta a branch localmente porque já foi anexada no repositório remoto.


### Contribuindo com um projeto
- Entre no repositório do projeto.
- Cope o link http que aparece ao clicar no botão verde **Code**.
- Na sua máquina abra o Git Bash até a pasta desejada.
- `git clone link`
- `cd `: para entrar na pasta.
- `ls`: para listar o que tem dentro da pasta.
- `git branch -a`: para listar as branch's existentes.
- `git checkout -b nomedabash`: para ir para uma branch nova.
- Atere o projeto conforme desejado.
- No Git Bash na pasta.
- `git diff`- verique o que foi modificado.
- `git status`- verifique o status mais recente.
- `git add --all`- adicione todos os arquivos novos ou modificados.
- `git commit -m "Mensagem"` - adiciona a mensagem de boa prática.
- `git remote -v`- verifica se o endereço do repositório remoto.
- `git push origin nomedabash` - envie para o repositório remoto as alterações feitas.
- Verifique no GitHub se sua alteração foi enviada com sucesso clicando na aba **Pull requests** do repositório no GitHub.
- Clicar em **Compare** e verifique as alterações no código.
- **base: master <= compare: nomedabash**: Criar o **pull request** verificando se está indo da sua branch `nomedabash` para a branch master.
- Solicitar a revisão de código para a conta gerenciadora do repositorio.
- Aguardar a aprovação da sua solicitação.
- A conta gerenciadora fará o **merge** da sua branch `nomedabash` para a `master`.



