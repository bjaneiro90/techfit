# Mod01

## Important Notes:
As we are working with private repositories, we must also work with each user's tokens
therefore, to create our token we have to:

To obtain the personal access token on GitHub, follow these steps:

 **Access your GitHub account:**

Go to github.com and log into your account.

**Go to Settings:**

In the top right corner of the page, click your profile icon and select "Settings."

**Access the tokens section:**

In the menu on the left, scroll down until you find the "Developer settings" section. Click on it and then click on "Personal access tokens".

**Generate a new token:**

Click "Generate new token".

**Set token permissions:**

Give your token a name so you know what it is being used for. 

For __example, "Repository Cloning".__

Then select the required permissions. To clone a repository, you may need "__repo__" permissions. Select at least the following permissions:

__repo__ (full repository access, including private repositories)

**Generate and copy the token:**

After selecting the required permissions, click "Generate token" at the bottom of the page.

## Important: 
**This token will only be displayed once.** 

Copy it immediately and keep it in a safe place.

Now, you can use the token to clone the repository. Use the command below in the Visual Studio Code terminal, replacing <TOKEN> with your personal access token:

```bash
git clone https://<TOKEN>@github.com/user/test_Mod02.git d:\path\to\local\repo\Mod02 --progress
```
<strong style="color: blue;">Personally, I use keepass to store this type of stuff and it's on my OneDrive so I can access it.</strong>.




<details>
<summary>1º Passo: Ver as diferenças entre o local e o remoto</summary>

```bash
git status
```
Passo para actualizar o nosso repo LOCAL.

```bash
git pull origin main
```
</details>

<details>
<summary>2º Para trabalharem num branch vosso sem estragar o main ou main</summary>
:warning: **Aviso:** Para trabalharem num branch individual

 ```bash 
git checkout -b 202407161357-%Issue%-%Task%-%DescricaoDoActualizado%
```
**202407161357** é AnoMesDiaHoraMin.
  
**%Issue%** é o 1.1.
  
**%Task%** é o 1.1.1.
   
**%DescricaoDoActualizado%** é a vossa descricao "UpdateDoExercicio".

**Exemplo** git checkout -b 202407172124-1.1-1.1.1-UpdateDeDescricao
</details>

<details>
<summary>2º Passo v2 Para trabalharem directamente no repo sem branchs</summary>
   :warning: **Aviso:** Para trabalharem directamente no principal.
	
 ```bash 
	git add /1.1-introdução-ao-Devops.md
```
um por cada ficheiro.
 
   Passo o push (o enviar do ficheiro para  repo) .
   ```bash
	git push -u origin main`
  ```
   Passo para confirmar os ficheiros enviados (commit) com a mensagem desejada -m.
   ```bash
	git commit -m 202407161357-%Issue%-%Task%-%DescricaoDoActualizado%
  ```

**Exemplo** git commit -m 202407172124-1.1-1.1.1-UpdateDeDescricao

   So para confirmar tudo.
  ```bash 
	git push
	git status
 ```

 </details>
 
<details>
<summary>3º Passo - Adicionar os ficheiros que querem adicionar sucessivamente</summary>
	
```bash
	git add /1.1-introdução-ao-Devops.md
 ```

um por cada ficheiro.
 
   Passo seguinte, fazer o push (o enviar do ficheiro para  repo) 
   
```bash   
	git push -u origin 202407161357-%Issue%-%Task%-%DescricaoDoActualizado%
 ```
   Passo para confirmar os ficheiros enviados (commit) com a mensagem desejada -m 
   
```bash   
	git commit -m 202407161357-%Issue%-%Task%-%DescricaoDoActualizado%
 ```
**Exemplo** git commit -m 202407172124-1.1-1.1.1-UpdateDeDescricao.

   So para confirmar tudo
   
 ```bash  
	git push
	git status
 ```
</details>

<details>
<summary>4º Passo para voltarmos ao branch Main ou main</summary>
	
```bash
git checkout main
```
	
   Passo para actualizar o nosso repo LOCAL.
   
```bash
git pull origin master
```
</details>
