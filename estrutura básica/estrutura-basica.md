## Estrutura Básica do HTML
A estrutura básica de um documento HTML segue uma hierarquia bem definida, onde cada parte desempenha um papel essencial para a organização e funcionamento da página web. Abaixo colocarei nos detalhes os principais elementos e suas funcionalidades de marcação:

### 1. DOCTYPE html
Essa declaração aparece no topo de todo documento HTML e informa ao navegador que tipo de documento está sendo processado. Em HTML5, a declaração é simplesmente ```<!DOCTYPE html>```. É uma instrução ao navegador para renderizar a página conforme os padrões mais recentes de marcação web.

### 2. html
Este é o elemento raiz que encapsula todo o conteúdo da página. Tudo dentro do documento HTML está contido dentro da tag <html>.

```
<!DOCTYPE html>
<html lang="pt-BR">
    <!-- Conteúdo do documento HTML -->
</html>
```

O ```lang``` define o idioma do documento HTML, é massa pra qualificar o site em acessibilidade e SEO.

### 3. head
A seção ```<head>``` contém metadados e links para recursos externos, como os docuemtnos de estilos do CSS, scripts do JS, e meta-informações, como a codificação e exploração de caracteres.

```
<head>
    <meta charset="UTF-8">
    <title>Título da Página</title>
    <link rel="stylesheet" href="styles.css">
    <script src="script.js" defer></script>
</head>
```

Elementos comuns:

```<meta>```: Fornece metadados, como a codificação de caracteres (charset).

```<title>```: Define o título da página, que aparece na aba do navegador.

```<link>```: Conecta a página a recursos externos, como arquivos de estilo CSS.

```<script>```: Vincula scripts JavaScript à página.

### 3. body
O elemento ```<body>``` contém todo o conteúdo visível da página, como textos, imagens, links, botões, etc. Aqui começa a mágica no front-end! 

```
<body>
    <h1>Olá, Jovem!</h1>
    <p>Este é um curtíssimo parágrafo!</p>
</body>
```

Resumidamente, tudo o que é visível para o usuário na interface que você está codificando é inserido dentro do ```<body>```. 