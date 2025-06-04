# mi-guia-git-github.io

Cenário A: Você já tem um código em uma pasta local

Navegue até a pasta do seu projeto:
Abra seu terminal ou prompt de comando e use cd para ir até a pasta onde seu código está. Exemplo:

Bash

cd /caminho/para/minha/pasta/projeto
Inicializar o Git no seu projeto:
Este comando cria um novo repositório Git vazio na pasta atual, adicionando uma pasta oculta .git.

Bash

git init
Adicionar seus arquivos ao "stage" (área de preparação):
Este comando adiciona todos os arquivos da sua pasta atual (e subpastas) ao "stage". O stage é uma área intermediária onde você prepara os arquivos que serão incluídos no próximo commit.

Bash

git add .
Ou para adicionar um arquivo específico: git add nome_do_arquivo.txt

Criar seu primeiro commit:
Um commit é um "snapshot" das suas alterações em um determinado momento. A mensagem do commit deve ser descritiva.

Bash

git commit -m "Meu primeiro commit: Projeto inicial"
Adicionar o repositório remoto (GitHub):
Este comando informa ao Git local qual é o repositório no GitHub para onde você quer enviar seu código.

Vá para a página do seu repositório no GitHub.
Clique no botão verde "Code" (ou "Clone").
Copie a URL HTTPS (geralmente começa com https://github.com/seu-usuario/seu-repositorio.git).
No seu terminal, use a URL copiada:

Bash

git remote add origin https://github.com/seu-usuario/seu-repositorio.git
origin é o nome padrão para o repositório remoto principal.

Renomear sua branch principal para main (se necessário):
O Git tradicionalmente usava master como nome da branch principal. O GitHub e a comunidade Git agora recomendam main. Se o seu Git local inicializou com master, é uma boa prática renomear:

Bash

git branch -M main
Enviar seu código para o GitHub:
Este é o comando que "empurra" (push) suas alterações do seu repositório local para o repositório remoto no GitHub.

Bash

git push -u origin main
git push: Envia as alterações.
-u origin main: Define a branch local main para rastrear a branch remota main do origin. Isso significa que, nas próximas vezes, você poderá usar apenas git push e git pull.
Você será solicitado a inserir seu nome de usuário e senha do GitHub. Se você usa autenticação de dois fatores, precisará de um Personal Access Token (Token de Acesso Pessoal) em vez da sua senha (veja a seção "Autenticação" abaixo).
