# dio-desafio-github-primeiro-repositorio
Desafio de Projeto sobre git/GitHhub


Estados
Modificado (modified);
Preparado (staged/index)
Consolidado (comitted)

Setar usuário
git config --global user.name "Renatao1234"

Setar email
git config --global user.email nome@endereco.com.br

Setar editor  
git config --global core.editor visual studio

Setar ferramenta de merge
git config --global merge.tool visual studio

Setar arquivos a serem ignorados
git config --global core.excludesfile ~/.gitignore

Listar configurações
git config --list


Repositório Local


Criar novo repositório
git init

Verificar estado dos arquivos/diretórios
git status


Adicionar arquivo/diretório (staged area)

Adicionar um arquivo em específico
git add meu_arquivo.txt

Adicionar um diretório em específico
git add meu_diretorio

Adicionar todos os arquivos/diretórios
git add .	

Adicionar um arquivo que esta listado no .gitignore (geral ou do repositório)
git add -f arquivo_no_gitignore.txt


Comitar arquivo/diretório


Comitar um arquivo
git commit meu_arquivo.txt

Comitar vários arquivos
git commit meu_arquivo.txt meu_outro_arquivo.txt

Comitar informando mensagem
git commit meuarquivo.txt -m "minha mensagem de commit"


Remover arquivo/diretório


Remover arquivo
git rm meu_arquivo.txt

Remover diretório
git rm -r diretorio


Repositório Remoto


Exibir os repositórios remotos
git remote
git remote -v

Vincular repositório local com um repositório remoto
git remote add origin git@github.com:leocomelli/curso-git.git

Exibir informações dos repositórios remotos
git remote show origin

Renomear um repositório remoto
git remote rename origin curso-git

Desvincular um repositório remoto
git remote rm curso-git

Enviar arquivos/diretórios para o repositório remoto
O primeiro push de um repositório deve conter o nome do repositório remoto e o branch.

git push -u origin master
Os demais pushes não precisam dessa informação
git push


Atualizar repositório local de acordo com o repositório remoto


Atualizar os arquivos no branch atual
git pull

Buscar as alterações, mas não aplica-las no branch atual
git fetch

Clonar um repositório remoto já existente
git clone git@github.com:leocomelli/curso-git.git


Visualizar histórico

Exibir histórico
git log

Exibir histórico com diff das duas últimas alterações
git log -p -2

Exibir resumo do histórico (hash completa, autor, data, comentário e qtde de alterações (+/-))
git log --stat

Exibir informações resumidas em uma linha (hash completa e comentário)
git log --pretty=oneline

Exibir histórico com formatação específica (hash abreviada, autor, data e comentário)
git log --pretty=format:"%h - %an, %ar : %s"

%h: Abreviação do hash;
%an: Nome do autor;
%ar: Data;
%s: Comentário.
