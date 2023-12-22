Texto simples
------------------------------
normal: 
abcd<br>
`seu texto normal`

italico: 
_abcd_<br>
`_seu texto italico_` ou `*seu texto italico*`

negrito: 
**abcd** <br>
`**seu texto negrito` ou `__seu texto negrito__`

grifado: 
~~abcd~~ <br>
`~~seu texto grifado~~`

<details>
<summary>combinações</summary>

resultado | italico | negrito | grifado | codigo
---: | :---: | :---: | :---:| :---
***abcde*** |X|X||`***abcde***`
*~~abcde~~* |X||X|`*~~abcde~~*`
~~**abcde**~~ ||X|X|`~~**abcde**~~`
~~__*abcde*__~~ |X|X|X|`~~__*abcde*__~~`

</details>

combina com [tabelas]() e [checklists]()

-----------------------------

Titulos
------------------------------


# titulo nivel 1 `# seu titulo`<br>

## titulo nivel 2 `## seu titulo`<br>
### titulo nivel 3 `### seu titulo`<br>

#### titulo nivel 4 `#### seu titulo`<br>

 ##### titulo nivel 5 `##### seu titulo`<br>


 ###### titulo nivel 6 `###### seu titulo`<br>


<details>
<summary>notação para codigo</summary>

titulo nivel 1 para codigo
====================================
```markdown
seu titulo de nivel 1
=====================================
```

titulo nivel 2 para codigo
------------------------------------
```markdown
seu titulo de nivel 2
--------------------------------------
```

</details><br><br>

>NOTE:
>
> utilize os titulos para declarar o nivel de hieraquia do conteudo e não o tamanho do titulo. isso não é css e não é pelo estilo e sim pelo uso

------------------------------------------

Tabelas
------------------------------------------

definindo colunas:
`|`
```markdown
coluna 1 | coluna 2
```

<details>
<summary>resultado</summary>

coluna 1 | coluna 2
---|---

</details><br>

definindo as linhas:
`---`

```markdown
coluna 1 | coluna 2
-------- | --------
```


<details>
<summary>resultado</summary>

coluna 1 | coluna 2
---|---
   |   
   |

</details><br>

criando os registros:

```markdown
coluna 1 | coluna 2
-------- | --------
registro | estado
registro | estado
registro | estado
registro | estado
registro | estado
```

<details>
<summary>resultado</summary>

coluna 1 | coluna 2
-------- | --------
registro | estado
registro | estado
registro | estado
registro | estado
registro | estado

</details><br>

Orientando o texto: 
`:---:`

```markdown
Para esquerda | Para o centro | para direita
:-------- | :--------: | --------:
X         |      X     |         X
X         |      X     |         X
X         |      X     |         X

```
<details>
<summary>resultado</summary>

Para esquerda | Para o centro | para direita
:-------- | :--------: | --------:
X         |      X     |         X
X         |      X     |         X
X         |      X     |         X

</details><br>

> NOTE
>
> o que vai mudar a orientação do texto é o uso do `:` e não a posição da letra ou espaçamento manual, eu fiz espaçado no codigo apenas por ilustração
>
> utilize `:---` para a esquerda
> `:---:` para o centro e
> `---:` para a direita assim como está no codigo de exemplo

<br><br>


exemplos de uso:

linguagem | programação|marcação | codigo de exemplo
:---:|---:|:---|:---
Javascript | Sim |Não| `console.log('hello world')`
Python | X ||`print('hello world')`
HTML | N |S| `<p>hello world</p>`
markdown | No |Yes| `> hello world`


<details>
<summary>codigo da tabela</summary>

```markdown
linguagem | programação|marcação | codigo de exemplo
:---:|---:|:---|:---
Javascript | Sim |Não| `console.log('hello world')`
Python | X ||`print('hello world')`
HTML | N |S| `<p>hello world</p>`
markdown | No |Yes| `> hello world`

```
</details>

combina com [codificação]()

