

# GIT

> **Git** é um dos sistemas de versionamento de sources.
>
> Não deve ser usado para versionar binários, já que isso seria impossível (bin != source).

```
Source == plain/text
```

### 2 formas de ter seu código remotamente versionado:

1. Adicionando um repositório remoto à um código versionando apenas localmente.
2. Clonando um código (seu ou de outros) que já esteja em um repositório remoto.

----

## Etapas pela forma #1

1. Cria-se os arquivos locais

2. Dá-se o início do versionamento dentro da pasta do projeto em questão `git init`

3. Adicione o repositório remoto `git remote add [apelido do remoto] [url do remoto]`

    Ex: `git remote add origin https://github.com/user/meu-repo.git`

4. Execute o comando `git remote -v` e verá que a pasta tem como remoto o repositório clonado.

5. Aqui vc já tem um 'link' com o remoto. Versione normalmente o código (git add, git commit, etc), depois se quiser subir as alterações para o remoto, basta executar `git push [apelido do remoto] [branch que quero subir]`:

    Ex: `git push origin master`

6. Agora você tem seu código no repositório remoto.

----

## Etapas pela forma #2

1. Clona-se o repositório remoto desejado

    Ex: `git clone https://github.com/user/meu-repo.git`

2. Por padrão, na pasta onde se executou o comando, será criado uma pasta com o mesmo nome do repositório clonado, no caso `meu-repo`

3. Entre na pasta criada (pelo terminal executando `cd meu-repo`)

4. Execute o comando `git remote -v` e verá que a pasta tem como remoto o repositório clonado.

5. Crie novos arquivos ou altere os existente e versione normalmente o código (git add, git commit, etc), depois se quiser subir as alterações para o remoto, basta executar `git push [apelido do remoto] [branch que quero subir]`:

    Ex: `git push origin master`
6. Agora você tem seu código atualizado no repositório remoto.

----
