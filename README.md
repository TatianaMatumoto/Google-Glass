# Google-Glass 👓
Projeto feito com base no curso do Guanabara (Curso de HTML5).

Ps: os arquivos `data_javascript.html, lampadaMelhor_javascript.html e lampada_javascript.html` também foram feitos durante o curso. 

⚠️ Atenção! Não sei por qual motivo ainda, as imagens do menu estão ficando sobrepostas no centro. ⚠️

## Anotações 

Pequenas anotações feitas durante o curso. 

## Linguagens: 

- HTML: semântico, tem significado
- CSS: formatações
- JavaScript: interatividade entre as páginas

# História 

**FTP**: protocolo para transmissão de arquivos
**DNS**: protocolo para identificação de máquinas na rede

**1972**: criação do e-mail 

**TCP**: transfer control protocol, quebra os dados em pacotes. Mas não identifica as máquinas. (Por isso o IP)

**1990**: criação do protocolo HTTP, de transferência de hipertextos (qualquer coisa multimídia) e o html, além do wolrdwide web (www)

**1991**: primeiro web site criado.

## Sinais e modem 

**Sinal digital**: binário 
**Ondas senoidais**: sinal analógico (a maioria usa isso)
**Conversão da onda digital para uma onda analógica**: modulação (para transmitir pelo meio de comunicação)
**Para ser convertido de volta a onda digital**:  demodulação.
O modem faz os dois (Primeiros termos juntos)

**Datagramas**: pequenos pacotes 

Modem vai direto no provedor de acesso. Quando se conecta a internet, o computador recebe um IP (uma identificação), para qualquer meio de conexão com internet. Ele vai pro DNS, que confere os sites pelo IP do servidor hospedado e transfere essa informação pro aparelho de comunicação. 

Arquivos (fotos, músicas, etc) ficam no servidor, que são transmitidos para a máquina. 

Servidores DNS, servidores de nome de domínio. 

### JavaScript

Mudou muito de nome (Cmm(C--) 1992, ScriptEase, mocha, LiveScript, até que se juntou com a Sunmicrosystems (empresa do Java) e para atrair mais usuários, a nomearam de JavaScript (mas é tudo marketing). Era de uma pequena empresa a Nonbas, foi comprada pela OpenWave, mas foi comprada pela Netscape em 1995.  

_Só que não tem nada a ver com a linguagem Java._ 

As duas linguagens são baseadas em C (Clike)

Em 1996 a Microsoft lançou o VBScript, mas rebatizou para JScript. 

Em 1997 a Netscape contatou a Ecma, uma empresa para padronização de sistemas de informação, e especificou o C#. Então ela lançou o Ecma lançou o EcmaScript (2,5) versão padronizada pela Netscape. 

Ajax, jQuery, CommonJs são tipo JavaScript para fora dos navegadores. 

## Cheats 
Separa-se imagens de como vai ser a interface para visualizar melhor e não se perder.

Duplica-se os textos que vão ser inseridos no site em html, e salva-se como 'txt', porque se der algum problema, pode-se recuperar por este arquivo depois, apenas retirando o txt. 

Em alguns SOs, tipo o Linux, o sistema de arquivos é organizado diferente, então coloca-se _ antes das pastas para serem achadas mais facilmente, ou algum outro caractere especial. 

Arquivos PNG são ligeiramente maiores que JPEG. É melhor a resolução. Gera maior tráfego de dados. 

A opção `Salvar pra Web` em alguns programas, salva a imagem com um tamanho de arquivo menor.

A barra de caminho é sempre inclinada pra direita, é de servidor. O Windows usa pra esquerda, mas o computador entende mesmo assim.

Colocar sempre as imagens que vai utilizar na mesma pasta do html ou numa subpasta. Não em outro arquivo, nem caminhos absolutos (ex: C:// Meus documentos//)

Tags que não existem, só serão ignorados.

### CSS Cheats

Para um código funcionar na maior parte dos navegadores, tem sites onde se cola o código específico de css e ele vai gerar para todos os navegadores:
http://expressprefixr.herokuapp.com/
http://pleeease.io/play/ 

Porém não é tão necessário, já que hoje em dia a maioria já tem suporte. 

Site Google/fonts, é um repositório com várias fontes disponíveis para usar qualquer tipo de site. 

Quando se quer esconder algo do site para os usuários, coloca-se `display: none`, pois ainda vai ser achado pelos mecanismos de busca do google. 

Ao colocar um top de 0px, muitas vezes ainda vai ficar uma borda, pois dentro desse 0, por padrão, já tem uma margem dentro dele. Para eliminar todo o espaço, é necessário definir como `position: absolute;` e deixar um número negativo como top. 

### Cores 

Sistema hexadecimal: `#000000` // Os dois primeiros dígitos são a quantidade de vermelho, depois de verde e depois de azul. 
RGB: `rgb (35, 137, 195)`
RGBA: `rgba (200, 093, 320, 0.5)` // Mesmo que RGB, mas o último dígito  é entre 0 e 1,  indicando a quantidade de transparência. 
HSB: `hsl(165, 8%, 93%)` // Hue, Saturation and Bright ( Matiz, Saturação e Luminosidade). Esses dois últimos em porcentagem. Pode adicionar a transparência, só adicionando a no final e seu valor.  

# Código 

## HTML 
 `<!DOCTYPE html>`: Para dizer para o navegador que o documento é em HTML5. 

`<html lang="pt-br">`: Para dizer o idioma do documento. É bom para o Google saber que idioma é o site. 

`<meta charset="UTF-8">`: Para o padrão português: 

Para chamar o arquivo de CSS: `<link rel="stylesheet" type"text/css" href="pasta/nomedoarquivo.css">`

HREF: Hypertext Reference, quando vai chamar um arquivo de fora.

`<head></head>`: Para estruturais comportamentais do site, como vai se comportar, como vai ser configurado, e coisas visuais. Casoo CSS será feito no mesmo arquivo, como é algo comportamental, devera ficar dentro do head. 

Ex: 
```
<head>
	<style> 

		h1 {
			font-family: Arial; // tipo de fonte
			font-size: 30pt;
			color: blue;
			text-shadow: 2px 2px 2px black; // o primeiro se refere ao deslocamento lateral (lado), o segundo é o deslocamento vertical (cima, baixo) e o último é o espaçamento das sombras (mais espalhada) 
		}
	</style>
</head>
```

`<title>Nome da aba <\title>`: É o nome da aba no navegador. 

### Hierarquia de títulos 

`<h1>`: Títulos
`<h2>`: Subtítulo de H1
`<h3>`: Subtítulo de H2

Pode-se formatar no CSS para o h2 ficar maior, então não importa o tamanho, mas sim a hierarquia. 

`<hgroup>`:  Para agrupar títulos. É apenas semântico.

`<pre>`: Considerado como pré formatado, considerando os espaços e enters.  
`<p>`: Paragráfos
`<br/>`:  Break Row, para quebras de linha
`&nbsp;`: Non Break Space, espaço em branco 
`<wbs/>`: Word Breaker, para dividir as palavras quando se diminui a página. Caso não tenha a possibilidade de quebrar, ele não faz diferença alguma pro navegador. 
`&shy;`:  Soft Hyphen, para adicionar hífens na quebra de palavras. 

`<b>`: Bold, negrito
`<i>`: Itálico
`<em>`: Ênfase, tipo itálico, só que com significado semântico, usado para enfatizar o termo. 

`<del>`: Efeito riscado, com efeito semântico.
`<sup>`: Sobreescrito, em cima.
`<sub>`: Subescrito, em baixo.

`<code>`: Formatar código, com significado sêmantico. 

`<figure>`: Imagens com significados semânticos, imagens que fazem parte de um conteúdo. 
`<figcaption>`: Legenda da imagem. Pode ser texto e inclusive textos com tags.

`<nav>`: Tag especial que vai criar uma área de navegação.

### Listas 
Existem dois tipos de lista:

### ol - Ordered lists

```<ol type="">
1 = númeração
a = alfabeto
A = alfabeto maisculo
i = numeros romanos
I = numeros romanos maisculos
```

O padrão é a numeração, tanto que não precisa definir ela caso não queira mudar.

`<ol type "a" start="3">`: Pra começar de um determinado número/letra. Só aceita valores númericos

### ul - Unordered Lists
Também chamado de lista com demarcadores.

```<ul type="">
square
circle
disc
```

### li - List Itens

Pode-se criar listas dentro das listas, e com suas ordenações diferentes e tipos diferentes. 

### Link 
`<a>`: Âncora. Base para a criação do link. 

`<a href="">`: Referencia em hypertexto, utilizar o HTTP.

`<a href="https://github.com/TatianaMatumoto" target="_blank">`: Irá redirecionar para outra aba no navegador.  

`<a href="https://github.com/TatianaMatumoto" target="_self">`: Padrão, irá abrir na mesma aba. 

### Tabelas 

`<tr>`: Table Rows, linha.  Dentro dela, tem-se o td. 
`<td>`: Table Data.
 
`<td rowspan="2">`: Rowspan quer dizer que uma linha vai ocupar mais espaço, e o número é o número de linhas. 

`<td cowspan="2">`> Cowspan, mesma coisa, porém para colunas. 

## CSS

É importante colocar `@charset"UTF-8"`.

`<span>`:  Formatar pequenos pedaços de texto. É possível adicionar vários parâmetros no estilo. 

Ex: 
``` 
<span style="text-decoration: underline; text-indent: 50px;"> 
```

### Chamando class e id

Quando for `class`, será pelo `nametag.nameclass`. 
Quando for `id`, será pelo `#nameid`.

`position:relative`:  Vai ficar relativa aonde foi colocada no html. 

`display:block`: Permite que seja colocado flutuando.

Ex: 
```
body{
	background-color: red;
	background-image: url ("Nome da imagem"); // só assim já funciona, não precisa do caminho.   
	color: blue; //cor da fonte
}

figure.foto-legenda{
	border: 8px solid red;
	box-shadow: 1px 1px 4px black; /* sombra*/
}

figure.foto-legenda img{ /* Tudo que for da imagem, vai ter essas bordas, ou seja, a borda vai cobrir os cantos 100%*/
	width: 100%;
	height: 100%;
}
```


## JavaScript

A ordem dos comandos é pela ordem das linhas do código. 

Tudo tem que estar dentro da tag `<script>`.

Essa linguagem é apenas para manipular o que estiver dentro do navegador, então ela não pode acessar o computador nem hardware. 










