# Fundamentos do HTML

O **HTML (Linguagem de Marcação de HiperTexto)** é uma linguagem de marcação utilizada para estruturar e apresentar conteúdo na web. É um componente essencial da web juntamente com **CSS** e **JavaScript**.

Ao longo deste repositório, conterá:
1. O que é o HTML e como ele funciona.

2. A sintaxe básica e as principais tags do HTML.

3. Como criar textos e conteúdos com HTML.
4. Como estruturar sites com HTML.
5. Como trabalhar com listas, tabelas e formulários.
6. Os novos recursos do HTML5.

## Requisitos

### 1. Navegador
 - Microsoft Edge
 - Google Chrome
 - Mozilla Firefox

### 2. Editor de código 
 - Visual Studio Code

<br>
<blockquote>
O navegador será necessário para visualizar o resultado do código HTML que é escrito no editor. Já o editor de código servirá para escrever o código em si e gerar seus conteúdos.
</blockquote>
<br>


## 1. O que é o HTML e como ele funciona?
HTML significa Linguagem de Marcação de HiperTexto (HyperText Markup Language). É uma linguagem de computador que permite estruturar e apresentar conteúdo na web por meio de marcações dentro do texto.

As marcações do HTML são interpretadas pelo navegador web, que renderiza os elementos na tela formando a página que vemos.

O HTML utiliza tags para criar essas marcações no conteúdo. As tags são palavras-chave entre sinais de maior e menor que (< >) e definem como o conteúdo será exibido.

Por exemplo:

```
<h1> Isso é um título da página </h1>

<p>Este é um parágrafo na página.</p>
```

No exemplo acima, as tags <code>h1</code> definem um título de nível 1, enquanto as tags <code>p</code> definem um parágrafo de texto.

A maioria das tags HTML são compostas por uma tag de abertura e uma de fechamento para delimitar os elementos. O que estiver entre essas tags será afetado pelo elemento em questão.

## 2. A sintaxe básica e as principais tags do HTML.

Todo documento HTML possui uma estrutura padrão:

```
<!DOCTYPE html>
<html>

<head><!-- cabeça do documento --></head>

<body><!-- corpo do documento --></body>

</html>
```


Analisando o exemplo:

```<!DOCTYPE html>```: Define que esse documento é um HTML5. É obrigatório estar no início do documento.

```<html>  </html>:``` Tag raiz que envolve todo o conteúdo HTML. Tudo o que estiver no documento precisa estar dentro dessas tags.

```<head>  </head>```: Contém informações sobre o documento que não são mostradas diretamente na página (metadados).

```<body>  </body>```: Contém o conteúdo visível da página que será renderizado no navegador.

Essa é a estrutura básica de qualquer documento HTML. Dentro do <code>body</code>, adicionamos os elementos e tags para criar o conteúdo da página: textos, imagens, vídeos, tabelas e tudo mais.


## Elementos e Tags
As tags ou elementos HTML servem para definir a estrutura e o significado semântico dos diferentes tipos de conteúdo na página.

Alguns dos elementos HTML mais comuns:

### 1. Textos e Títulos

<code> h1 h2 h3 h4 h5 h6</code> 
Títulos de nível 1 a 6

```<p>```: Parágrafo de texto
<br>
```<br>```: Quebra de linha
<br>
```<hr>```: Linha horizontal


### 2. Listas

```<ol>```:Listas ordenadas
<br>
```<ul>```: Listas não-ordenadas
<br>
```<li>```: Itens das listas

### 3. Imagens e Multimídia

```<img>```: Exibe imagens
<br>
```<audio>```> e ```<video>```: Reproduz vídeos e áudios.

### 4. Tabelas
```
<table>

<tr>: Linha de tabela
<td>: Célula de dados

</table>
```
### 5. Formulários
```
<form>

<input>: Caixas de entrada
<button> sou um botão </button>

</form>
```
Cada elemento possui uma **semântica** (significado) e um comportamento diferente para representar da melhor forma o seu conteúdo.

Por exemplo, os elementos de título ```<h1>```possuem maior relevância, os parágrafos ```<p>``` representam texto comum, os elementos de lista ```<li> ```representam itens e por aí vai.

### 6. Atributos
Além das tags, os elementos HTML também podem receber atributos, que são informações extras que configuram características adicionais ao elemento.

A sintaxe geral de um atributo é:
```
<elemento atributo="valor do atributo">
```
Por exemplo, a tag  ```<a>``` de link possui o atributo href para indicar o destino:

```
<a href="https://github.com/ojonatasquirino">Perfil Github • Jônatas Quirino</a>
```

<blockquote>
<a href="https://github.com/ojonatasquirino">Perfil Github • Jônatas Quirino</a>
</blockquote>
<br>



### Alguns atributos comuns:

*id*: Identificador único do elemento.
<hr>

*class*: Classe para aplicar CSS.

<hr>

*style*: Estilos inline CSS

<hr>

*src*: Endereço da mídia a ser carregada.

<hr>

*href*: Destino de um link


## 3. Como Criar Conteúdo com HTML
Agora que vimos a anatomia e sintaxe básica de HTML, vamos ver na prática como criar conteúdos em uma página web.

### Textos e Títulos
Para inserir textos e títulos, utilizamos as tags apropriadas para cada tipo de conteúdo textual:

#### Títulos

Os títulos servem para destacar temas e seções de uma página. Utilizamos as tags ```<h1>``` até ```<h6>``` para definir a importância do título, sendo ```<h1>``` o mais importante e ```<h6>``` o menos importante.
```
<h1>Título Principal</h1>
<h2>Subtítulo 1</h2>
<h3>Subtítulo 2</h3>
```
#### Parágrafos

O elemento ```<p>``` representa parágrafos de texto comum:

```
<p>Este é um parágrafo com algumas sentenças de texto que formam um conteúdo qualquer.</p>

<p>Este é outro parágrafo separado do primeiro.</p>

```
#### Negrito e Itálico

Podemos deixar parte do texto em negrito ou itálico para dar ênfase:

```
<p>Neste parágrafo temos um <b>texto em negrito</b> usando a tag B (não semântica).</p>

<p>Neste outro, temos um <i>texto em itálico</i> com a tag I(também não semântica).</p>

```
#### Quebras

Podemos indicar quebras de linha com a tag ```<br>```:

```
<p>Esta é a primeira linha do parágrafo.

<br>

E esta é a segunda linha.</p>
```
E quebras de seção com a tag ```<hr>```:

```
<p>Parágrafo antes da quebra.</p>

<hr>

<p>Parágrafo depois da quebra.</p>
```
#### Comentários

Também podemos adicionar comentários no HTML assim: ``` <!-- -->```
```
<!-- Comentário que não aparece na página -->

<p>Conteúdo da página</p>

```
#### Imagens
Podemos mostrar imagens com a tag ```<img>```:
```
<img src="foto.png">
```
O atributo ```src``` indica o caminho para a imagem.

Também podemos definir o texto alternativo no atributo ```alt```, que aparece quando a imagem não carrega e é utilizado por leitores de tela para deficientes visuais:
```
<img src="foto.png" alt="Minha foto">
```
#### Links
Os links servem para conectar documentos e páginas web umas com as outras:

```
<a href="https://github.com/ojonatas">Perfil Github • Jônatas Quirino</a>
```

O atributo href indica o destino do link, que geralmente é uma URL, mas também pode ser um caminho de arquivo.

#### Listas

#### 1. Listas não ordenadas

São listas com marcadores, geralmente pontos. Usamos a tag ```<ul>``` para envolver os itens e a tag ```<li>``` em cada item:
```
<ul> 

<li>Item 1</li> 
<li>Item 2</li>  
<li>Item 3</li>
 
</ul>
```
#### 2. Listas ordenadas

São listas com itens numerados, definidas com a tag ```<ol>``` e os itens em ```<li>```:
```
<ol>  

<li>Primeiro item</li>  
<li>Segundo item</li>  
<li>Terceiro item</li>

</ol> 
```

Podemos utilizar listas dentro de listas para aninhar itens.

#### Tabelas
As tabelas permitem apresentar dados em formato de linha e colunas. São definidas com a tag ```<table>```.

Dentro delas, cada linha é representada pela tag <tr> (table row) e dentro de cada linha podemos colocar as células de dados <td> (table data):

```
<table>
<tr>

<td>Célula 1</td>    
<td>Célula 2</td>

</tr>    

<tr> 

<td>Célula 3</td>    
<td>Célula 4</td> 

</tr>

</table>

```

Resutado: 

<table>
<tr>

<td>Célula 1</td>    
<td>Célula 2</td>

</tr>    

<tr> 

<td>Célula 3</td>    
<td>Célula 4</td> 

</tr>

</table>

<hr>


Podemos juntar células horizontais ou verticais com o atributo colspan e rowspan.

Também podemos definir uma linha ou coluna como cabeçalho da tabela com a tag ```<th>``` (table header).

#### Formulários
Os formulários permitem a interação do usuário para inserir dados e enviar para o servidor:

```

<form> 

<label>Nome:</label>   
<input type="text">    
<label>Email:</label>  
<input type="email">    
<button type="submit">Enviar</button>

</form>

```

Resultado:

<form> 

<label>Nome:</label>   
<input type="text">    
<label>Email:</label>  
<input type="email">    
<button type="submit">Enviar</button>

</form>

O elemento ```<form>``` representa o formulário como um todo.

Dentro dele podemos colocar campos de entrada com ```<input>```, botões com ```<button>``` e outros elementos.

Existem vários tipos de ```<input>``` para diferentes tipos de dados, como texto, email, número, data, etc.

Também podemos usar ```<select>``` para criar menus suspensos e ```<textarea>``` para áreas de texto maiores.

## Semântica e Acessibilidade
Além de apenas definir a estrutura dos conteúdos com HTML, também precisamos nos preocupar em dar significado e proporcionar boa experiência de uso a todos os usuários.

Isso envolve seguir boas práticas de semântica e acessibilidade.

A semântica se refere a utilizar os elementos HTML de forma a representar corretamente a natureza e significado dos conteúdos.

Por exemplo, utilizar ```<h1>``` até ```<h6>``` para títulos ao invés de apenas formatar textos comuns em negrito ou itálico.

Já a acessibilidade significa tornar o conteúdo compreensível e funcional também para pessoas com deficiências ou limitações.

Isso pode envolver desde não depender somente de elementos visuais, provendo alternativas em áudio por exemplo, até possibilitar o uso total por meio de tecnologias assistivas como leitores de tela.

### Dicas de semântica e acessibilidade no HTML:

1. Utilizar elementos de acordo com o seu significado;
2. Prover texto alternativo para imagens com o atributo ```alt```;
3. Criar links compreensíveis fora de contexto;
4. Permitir ampliação de textos sem perda de layout.

## HTML5
HTML5 é a versão mais recente da linguagem lançada em 2014. Além de novas tags semânticas, ela também trouxe muitos outros recursos importantes:

### 1. Novo layout com tags semânticas. 
Veremos mais sobre essas tags ao longo do repositório. 

Introduziu novas tags como ```<header>```, ```<nav>```, ```<main>```, ```<section>```, ```<article>``` entre outras. Isso permite dar significado mais específico aos blocos de conteúdo.

### 2. Multimídia embutida

Agora podemos facilmente incorporar conteúdos multimídia com ```<video>```, ```<audio>``` e até gráficos vetoriais ```<svg>``` direto no HTML.

### 3. Acessibilidade aprimorada

Foco maior em acessibilidade com suporte a subtítulos, audiodescrição, texto alternativo aprimorado, entre outros.

### 4. Conectividade aprimorada

Permite interação em segundo plano com servidores com recursos como Server Sent Events e WebSockets.

### 5. Design responsivo

Adaptação mais simples para diferentes tamanhos de dispositivo, desde desktops até mobiles.

### 6. Compatibilidade aprimorada

Evolução dos navegadores modernos permitiu uso de muitos recursos novos do HTML5.

Resumidamente, o HTML5 trouxe excelentes funcionalidades que antes eram muito complexas ou necessitavam de outras tecnologias para serem implementadas.

Hoje, criar sites sofisticados e complexos utilizando apenas HTML e CSS é perfeitamente possível graças às novas funcionalidades do HTML5.