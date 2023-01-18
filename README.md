# Repositorio-GetStarted--K1-T1-

## "git checkout -- path\_or\_file"

    Irá desfazer todas as alterações que não estejam no Stage desde o último commit.



## "git checkout HEAD -- path\_or\_file'"

    Desfazer as alterações desde o último commit incluindo o Stage.



## "git revert commit"

    Irá criar um novo commit que desfaz as alterações do commit especificado

    Últil para desfazer commit antigo



## "git revert -- hard commit"

     Resetar e remover todas as alterações.

      -Cuidado ao usar! Não usar se já estiver publicado.

     Útil para desfazer últimos commits.



## "git branch nova\_branch"

      Criar uma nova branch



## "git branch -d branch"

      Excluir uma branch



## "git checkout branch"

      Muda para a branch.

      Seu repositório passa a ter os commits que a branch possui e novos commits serão adicionados à ela.



## "git merge branch"

      Aplicar os commits de uma branch na branch atual.

      Encontra um commit comum(base) entre as branchs e aplica todos os commits que a branch atual não possui.

      Caso existam commits na branch atual que não estão na outra,será criado um commit de merge.



## "git rebase branch"

     Semelhante ao Merge porém é diferente na ordem de aplicar os commits.

     No Rebase,os seus commits na frente da base são removidos temporariamente,os commits de outra branch são aplicadas na sua branch e por fim seus commits são aplicados um a um.

      Pode acontecer conflitos que serão resolvidos para cada commit.



## "git fetch"

      Baixa as atualizações do remote porém não aplica elas no repositório.

      Permite fazer o rebase de uma branch em vez de fazer o merge.

      Pull = Fetch + Merge.

      Fetch e Rebase é melhor para manter o histórico do desenvolvimento.



## ".gitignore"

      Configura arquivos que devem ser ignorados

      Contém arquivos,caminhos e patterns



## "git commit -amend"

       Altera o último commit

         -Mensagem de comit

         -Adiciona arquivos



## "git stash"

      Guarda as alterações do Working Directory.
      Permite fazer rebase,merge,trocar de branch



## "git cerrypick commit"

     Aplica as alterações de um commit na branch atual.

     Cria um novo commit.

     Útil para recuperar histórico.



## "git blame"

      Mostra as alterações feitas em um arquivo por linha.

      Mostra o autor e o commit que foi feito aquela linha.

      Útil para verificar quando as alterações foram feitas,por que e por quem.



## "git bisect"

     Permite fazer uma busca binária nos commits para encontrar uma alteração.

     Útil para alterações que modificaram o comportamento e não pode ser identificados por código

     Quando a alteração pode ser bastante antiga.
