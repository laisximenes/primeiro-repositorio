## Passo a passo Git Bash:

###### Fonte: [https://medium.com/@andradegabriela20/o-que-é-git-git-bash-e-comandos-básicos-94a53de6d376](https://medium.com/@andradegabriela20/o-que-é-git-git-bash-e-comandos-básicos-94a53de6d376)

Existem diversos comandos Git. Aqui eu vou demonstrar apenas alguns básicos porém suficientes para que você consiga criar seu repositório, e trabalhar de forma integrada com ele.

- Primeiro crie seu repositório seu local. Sua pasta onde ficará seu projeto.
- Entre na pasta e clique com o botão direito do mouse. Selecione o Git Bash:

- Para iniciar o repositório utilize o comando **“git init”** :

- Você pode verificar o status do repositório com o comando **“git status”**. É uma boa prática sempre conferir o status antes de iniciar com o fluxo das alterações e durante ele também :

Se você ainda não tiver nenhum arquivo nessa pasta, crie algum para continuar com o processo. Essa é a camada Working Directory.

- A próxima camada é o Index. Para mandar o seu arquivo para o index, basta utilizar o comando “**git add nomeDoArquivo**” ou se você quiser enviar ao Index todos os arquivos basta utilizar o parâmetro all. Assim: “**git add -all**” :

- Para verificar se o git está acompanhando seu arquivo, dê o comando “**git status**”. Se estiver tudo certo, aparecerá esta mensagem, o que significa que seu arquivo criado está na camada Stage :

- Depois que seus arquivos novos ou modificados estiverem na camada de Stage, você pode commita-los, ou seja, envia-los à ultima camada do fluxo, HEAD. Para isso use o comando “**git commit -m “tituloDoCommit”**. O parâmetro “-m” é passado para que você possa escrever uma descrição junto ao commit 

Agora a última etapa do fluxo é enviar o(s) arquivo(s) ao repositório remoto. Se você ainda não tem, crie um repositório remoto, pode ser no GitHub, GitLab ou qualquer outro de sua preferência.

- Depois de criado, copie a URL HTTP do seu repositório, ela será necessária :

- Volte ao Git Bash escreva o comando: “**git remote add origin urlDoRepositorio**”. Com esse comando você está especificando o repositório ao qual você deseja manter o seu projeto. “Origin” é apenas um apelido padrão, mas você pode utilizar qualquer nome :

- Depois de adicionado o repositório remoto, envie os arquivos utilizando o comando “**git push origin master**”.



Master é o nome da branch padrão quando você cria um repositório, é onde ficará o seu código do produto final. Branch são ramificações do repositório, elas facilitam a organização do projeto, do time e garante segurança para o seu projeto final pois permitem que você trabalhe de forma isolada em diferentes funcionalidades e não tudo junto no produto final. Se você tiver outras branchs no seu repositório basta alterar o nome master para o nome da branch que você quer na hora do git push. Lembrando que antes de iniciar todo o fluxo, você ja deve estar na branch que deseja enviar suas alterações. Vou explicar melhor sobre Branches depois.

Processo finalizado. Após o git push seus novos arquivos ou novas alterações já estão no repositório, você pode ir até lá verificar.