# Bruno e João

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
> :warning: **Aviso:** Para trabalharem num branch individual

git checkout -b 202407161357-%Issue%-%Task%-%DescricaoDoActualizado%
 
202407161357 é AnoMesDiaHoraMin.
  
%Issue% é o 1.1.
  
%Task% é o 1.1.1.
   
%DescricaoDoActualizado% é a vossa descricao "UpdateDoExercicio".
</details>
<details>
<summary>2º Passo v2 Para trabalharem directamente no repo sem branchs</summary>
  > :warning: **Aviso:** Para trabalharem directamente no principal.
  
	git add /1.1-introdução-ao-Devops.md
 
	... um por cada ficheiro
 
   Passo o push (o enviar do ficheiro para  repo) .
   
	git push -u origin main`
 
   Passo para confirmar os ficheiros enviados (commit) com a mensagem desejada -m .
   
	git commit -m 202407161357-%Issue%-%Task%-%DescricaoDoActualizado%
 
   So para confirmar tudo.
   
	git push
	git status
 </details>
 
<details>
<summary>3º Passo - Adicionar os ficheiros que querem adicionar sucessivamente</summary>
	git add /1.1-introdução-ao-Devops.md
 
	... um por cada ficheiro
 
   Passo o push (o enviar do ficheiro para  repo) 
   
	git push -u origin 202407161357-%Issue%-%Task%-%DescricaoDoActualizado%
 
   Passo para confirmar os ficheiros enviados (commit) com a mensagem desejada -m 
   
	git commit -m 202407161357-%Issue%-%Task%-%DescricaoDoActualizado%
 
   So para confirmar tudo
   
	git push
	git status
</details>

<details>
<summary>4º Passo para voltarmos ao branch Main ou main</summary>
	git checkout main
 
   Passo para actualizar o nosso repo LOCAL.
   
	git pull origin master
</details>
