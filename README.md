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

<br>

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

<br>

Listas
----------------------------------------

Listas desordenadas:

para criar item de lista utilize `* ` ou `- `.

- item de camada 1
  - item de camada 2
    - item de camada 3 
      - item de camada 4
    - outro item de camada 3 
  - outro item de camada 2
-  outro item de camada 1

<details>
<summary>codigo de lista</summary>

```markdown

- item de camada 1
  - item de camada 2
    - item de camada 3 
      - item de camada 4
    - outro item de camada 3 
  - outro item de camada 2
-  outro item de camada 1

```


</details>


>NOTE
>
> você pode utilizar os dois simbolos `-` e `*` na mesma lista para criar itens desta lista mas observe que existe uma interação diferente utilizando o markdown.
>
<details>
<summary>ler mais...</summary>
 basicamente ele vai interpretar sendo listas diferentes e vai criar um espaçamento entre essas listas diferentes (mesmo fazendo parte da mesma lista)<br><br>

 observe este exemplo:<br>
 se tivermos uma lista junta com elementos de tipos diferentes teremos esse resultado ![lista segmentada](./lista%201.png)<br>
 uma lista que se trasforma em duas listas separadas.<br><br> agora veja isso, se tivermos uma lista espaçada mas com um elemento do tipo 2 na lista 1 teremos novamente duas listas 
 ![lista segmentada](./lista%202.png) <br>
 uma comprimida do tipo 1 `*` e uma espaçada do tipo 2 `-`
 <br><br>
 e se tiramos o espaçamento as listas se ordenam da mesma forma 
 ![lista segmentada](./lista%203.png)<br>
 porem continua sendo duas listas separadas e tecnicamente distintas<br><br>

 por fim observe essa imagem ilustrativa das mesmas duas listas com um dos sinais intercalados no meio ![lista segmentada](./lista%204.png)<br>

 dessa forma criamos literalmente 4 listas pois o markdown vai interpretar cada troca de sinal sendo uma lista nova de forma que um sinal intercalado criaria 3 listas diferentes

 >dessa forma lembre-se de usar o mesmo padrão sempre ou alterne se estiver lidando com listas diferentes no mesmo local
</details>
