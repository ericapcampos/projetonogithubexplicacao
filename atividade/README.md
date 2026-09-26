# Ciclo de um Projeto no Github

***

## **Passo a passo da criação e envio**

Para começar, precisamos entrar no Github ou criar uma conta. Para criar um repositório, clicamos em ****Create new****, que tem o simbolo de "+". Depois, escolhemos "New repository". Assim, vamos para a página onde ficam as configurações do novo repositório.

Primeiro, colocamos o nome do repositório. Depois, podemos colocar uma descrição, escolher se ele será Publico ou privado, ativar o README, escolher um template e adicionar uma licença.

### **Processo de vincular uma pasta local no seu computador a esse reposotório remoto criado na nuvem.**

Depois de criar o repositório, podemos adicionar os arquivos do computador. Para isso, clicamos em ****Add file**** e depois em ****Upload files****. Na próxima página, clicamos em ****Choose your files****. Depois, procuramos no computador os arquivos que queremos enviar. No nosso caso, podemos pegar a pasta inteira e arrastar para o campo de ****Choose your files*****

### **O primeiro envio**

Depois de escolher os arquivos, precisamos fazer o envio. Para isso, clicamos no botão verde ****commit changes****. Assim, os arquivos são enviados para o repositório e podem ser visualizados. Se depois precisarmos mudar alguma coisa, basta clicar no arquivo e editar os códgicos.

***

## A Anatomia do README Perfeito

### **Para que serve o README e quem é o público-alvo dele?**

O ****README**** serve para explicar o projeto de forma simples. Nele, podemos mostrar o que o software faz, qual problema ele resolve e qual é seu objetivo. Ele é feito para pessoas que querem usar ou entender o projeto e também para recrutadores que estão vendo o portifólio.

### **Dados Fundamentais** 

- Titulo: Nome do projeto e seu principal objetivo
- Tecnologias usadas: Linguagens usadas para fazer o projeto
- Como rodar projeto: Explica como instalar e usar o projeto
- Status do desenvolvimento: Mostra se o projeto está em andamento ou finalizado
- Liencça: Mostra quem criou ou participou do projeto

### **Linguagem Mardown**
Utilizamos essa linguagem porque ela é simples e ajuda a deixar o texto mais organizado e fácil de entender.

***

## Mapa das Atualizações (Commits e Pushes)

### **Github Online**

Podemos alterar um arquivo diretamente pelo Github seguindo esses passos:

- Abra o reposiório do Git
- Procure o arquivo que deseja alterar
- Clique no icone de lápis
- Faça as alterações no editor
- Por fim, clique em commite changes

Quando usar: para fazer alterações simples nos arquivos e no README.

### **Git via Linha de Comando (Terminal)**
É uma forma de trabalhar com o Git usando comandos no terminal. Ele permite controlar melhor as etapas do desenvolvimento.

- Fluxo:
git config --global user.name "Seu Nome"
git config --global user.email "[seu_email@exemplo.com](mailto:seu_email@exemplo.com)"

Para não precisar colocar a senha toda vez que enviar algo, podemos fazer uma conexão segura. Para criar a chave, usamos: ssh-keygen -t ed25519 -C "[seu_email@exemplo.com](mailto:seu_email@exemplo.com)"

Depois, mostramos a chave pública, copiamos o conteúdo e colocamos em GitHub > Settings > SSH and GPG keys:
cat ~/.ssh/id_ed25519.pub

Em seguida, entramos na pasta do projeto e transformamos ela em um repositório Git local:
cd caminho/para/sua/pasta
git init
git branch -M main

Criamos o arquivo README.md, adicionamos os arquivos e fazemos o primeiro commit:
echo "# Meu Primeiro Projeto" > README.md
git add .
git commit -m "Primeiro commit"

Por fim, criamos um repositório vazio no GitHub, copiamos a URL e usamos os comandos abaixo para ligar o projeto ao Github e enviar os arquivos:
git remote add origin URL_DO_SEU_REPOSITORIO
git push -u origin main

### **Minha experiência utilizando a interface:**

De maneira geral, tive uma certa dificuldade para entender os assuntos da sessão 3, mas achei as interfaces fáceis de usar. No geral, foi uma experiência fácil e menos frustante.

### **GitHub Desktop**

O GitHub Desktop ajuda a usar o Git e o GitHub sem precisar ficar usando comandos no terminal.

Ele facilita:
- Visualizar alterações: mostra quais arquivos foram modificados.
- Selecionar alterações: permite escolher o que será colocado no commit.
- Criar Commits: permite salvar as alterações feitas no projeto.
- Enviar alterações: ajuda a enviar os commits para o GitHub.
- Acompanhar o histórico: mostra os commits e as alterações feitas no projeto.
