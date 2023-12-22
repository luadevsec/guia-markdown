Texto simples <mark id= "text">
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

combina com [tabelas](#tables) e [checklists](#checklist)

-----------------------------

Titulos <mark id="title">
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

Tabelas <mark id="tables">
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

combina com [codificação](#code)

<br>

----------------


Listas <mark id="list">
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
 se tivermos uma lista junta com elementos de tipos diferentes teremos esse resultado <br> ![lista segmentada](./lista%201.png)<br>
 uma lista que se trasforma em duas listas separadas.<br><br> agora veja isso, se tivermos uma lista espaçada mas com um elemento do tipo 2 na lista 1 teremos novamente duas listas<br>
 ![lista segmentada](./lista%202.png) <br>
 uma comprimida do tipo 1 `*` e uma espaçada do tipo 2 `-`
 <br><br>
 e se tiramos o espaçamento as listas se ordenam da mesma forma <br>
 ![lista segmentada](./lista%203.png)<br>
 porem continua sendo duas listas separadas e tecnicamente distintas<br><br>

 por fim observe essa imagem ilustrativa das mesmas duas listas com um dos sinais intercalados no meio<br> ![lista segmentada](./lista%204.png)<br>

 dessa forma criamos literalmente 4 listas pois o markdown vai interpretar cada troca de sinal sendo uma lista nova de forma que um sinal intercalado criaria 3 listas diferentes

 >dessa forma lembre-se de usar o mesmo padrão sempre ou alterne se estiver lidando com listas diferentes no mesmo local
</details>

combina com [checklist](#checklist)

<br>

--------------------------

Codificação <mark id="code">
-------------------------------

linha de codigo: ``` ` ` ```


<details>
<summary>exemplo de linha</summary>


    `seu codigo`


</details><br>


bloco de codigo:
```
    ```
    ```
```

<details>
<summary>exemplo de bloco</summary>


    ```
    seu codigo 
    em bloco
    ```

</details><br>

bloco interpretado:

    ```markdown

    ```

<details>
<summary>exemplo interpretado</summary>


```markdown
# codigo
* seu codigo com interpretação em
    * markdown
    * html
    - python
    - javascript
**o que quiser**
~~e souber~~
```
<br>

<details>
<summary>HTML</summary>

```html
<style>
    .red {
        background-color: red !important;
    }
</style>

<body>
    <main class="purple">
        <p id="hw">hello world</p>
    </main>
</body>
```

</details><br>


<details>
<summary>JavaScript</summary>

```javascript
document.addEventListener('DOMContentLoaded', function() {
    const greeting = {
        name: 'world',
        getMessage: function() {
            return `Hello, ${this.name}!`;
        }
    };

    const hwElement = document.getElementById('hw');
    hwElement.textContent = greeting.getMessage();
});
```

</details><br>


<details>
<summary>CSS</summary>

```css
.red {
    background-color: red !important;
}

.purple {
    color: purple;
}
```

</details><br>


<details>
<summary>Python</summary>

```Python
class Greeting:
    def __init__(self, name):
        self.name = name

    def get_message(self):
        return f"Hello, {self.name}!"

greeting = Greeting('world')
print(greeting.get_message())
```

</details><br>


<details>
<summary>Ruby</summary>

```ruby
class Greeting
  def initialize(name)
    @name = name
  end

  def get_message
    "Hello, #{@name}!"
  end
end

greeting = Greeting.new('world')
puts greeting.get_message
```

</details><br>


<details>
<summary>C#</summary>

```C#
using System;

class Program
{
    static void Main()
    {
        Greeting greeting = new Greeting("world");
        Console.WriteLine(greeting.GetMessage());
    }
}

class Greeting
{
    private string Name;

    public Greeting(string name)
    {
        Name = name;
    }

    public string GetMessage()
    {
        return $"Hello, {Name}!";
    }
}
```

</details><br>


<details>
<summary>React</summary>

```jsx
import React, { useState, useEffect } from 'react';

const GreetingComponent = () => {
    const [greeting, setGreeting] = useState({ name: 'world' });

    useEffect(() => {
        setGreeting((prev) => ({ ...prev, message: `Hello, ${prev.name}!` }));
    }, []);

    return (
        <div className="purple">
            <p id="hw">{greeting.message}</p>
        </div>
    );
};

export default GreetingComponent;
```
</details><br>


</details><br>

----------------------------------------------

Notes <mark id="notes">
---------------------------------

notas simples `> `:

```markdown
> NOTE 
>
> eu sou um bloco de observação
```

<details>
<summary>resultado</summary>

>NOTE 
>
> eu sou um bloco de observação

</details><br>

notas complexas `>> `:

```markdown
> NOTE 
>
> eu sou um bloco de observação
>> com outra observação dentro
>>
>>> que também observa
>>
>>> e é observado
```

<details>
<summary>resultado</summary>

> NOTE 
>
> eu sou um bloco de observação
>> com outra observação dentro
>>
>>> que também observa
>>
>><br>
>>
>>> e é observado

</details><br>

> NOTE
>
> combina com qualquer outro elemento como listas, imagem, tabelas e outros. basta colocar o simbolo > e o outro simbolo que queira utilizar, como > * para listas ou > ` para codigos

combina com [textos simples](#text)

---------------------------------------


checklist
-----------------------------------------

checkbox vazia `[ ]`:
```markdown
- [ ] item a fazer
```
- [ ] item a fazer
---

<br>


checkbox cheia `[x]`:
```markdown
- [x] item feito
```
- [x] item feito<br>
---

<br>

checkbox cheia grifada `[x]`:
```markdown
- [x] ~~item feito grifado~~
```
- [x] ~~item feito grifado~~<br>
---

<br>

checklist:

  - [ ] item
  - [ ] outro
    - [ ]  sub item
  * [ ] mais item 
  
  <br>

  >NOTE
  >
  > as regras de lista se aplicam a checklist então consulte o funcionamento de [listas e simbolos ](#list)


combina com [texto simples](#text) e [listas](#list)

------------------------------------

Links e imagens <mark id="link">
-------------------------------------
```
Comming soon, to cansada vou dormir kkkk
```



