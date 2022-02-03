# Google-Glass 👓
Projeto feito com base no curso do Guanabara (Curso de HTML5).

⚠️ Atenção! Não sei por qual motivo ainda, as imagens do menu estão ficando sobrepostas no centro. ⚠️ 

## Anotações 

Pequenas anotações feitas durante o curso. 

## História 

FTP: protocolo para transmissão de arquivos
DNS: protocolo para identificação de máquinas na rede

1972: criação do e-mail 

TCP: transfer control protocol, quebra os dados em pacotes. Mas não identifica as máquinas. (Por isso o IP)

1990: criação do protocolo HTTP, de transferência de hipertextos (qualquer coisa multimídia) e o html, além do wolrdwide web (www)

1991: primeiro web site criado.

HTML: semântico, tem significado
CSS: formatações
JavaScript: interatividade entre as páginas

Sinal digital = binário 
Ondas senoidais = sinal analógico (a maioria usa isso)

Conversão da onda digital para uma onda analógica = modulação (para transmitir pelo meio de comunicação)

Para ser convertido de volta a onda digital, chama-se demodulação.
O modem faz os dois (Primeiros termos juntos)

Datagramas = pequenos pacotes 

Modem vai direto no provedor de acesso. quando se conecta a internet,o computador recebe um IP, uma identificação, para qualquer meio de conexão com internet. ele vai pro DNS, que confere os sites pelo IP do servidor hospedado e transfere essa informação pro aparelho de comunicação. Arquivos (fotos, músicas, etc) ficam no servidor, que são transmitidos para a máquina. 

Servidores DNS, servidores de nome de domínio. 

Para um código funcionar na maior parte dos navegadores, tem sites onde se cola o código específico de css e ele vai gerar para todos os navegadores:
http://expressprefixr.herokuapp.com/
http://pleeease.io/play/ 

Porém não é tão necessário, já que hoje em dia a maioria já tem suporte. 

Site Google/fonts, é um repositório com várias fontes disponíveis para usar qualquer tipo de site. 


------ JavaScript
Mudou muito de nome (Cmm(C--) 1992, ScriptEase, mocha, LiveScript, até que se juntou com a Sunmicrosystems(empresa do Java) e para atrair mais usuários, a nomearam de JavaScript(mas é tudo marketing). Era de uma pequena empresa a Nonbas, foi comprada pela OpenWave, mas foi comprada pela Netscape em 1995.  

Só que não tem nada a ver com a linguagem Java. 

As duas linguagens são baseadas em C (Clike)

Em 1996 a Microsoft lançou o VBScript, mas rebatizou para JScript. 

Em 1997 a Netscape contatou a Ecma, uma empresa para padronização de sistemas de informação, e especificou o C#. Então ela lançou o Ecma lançou o EcmaScript(2,5) versão padronizada pela Netscape. 

Ajax, jQuery, CommonJs são tipo JavaScript para fora dos navegadores. 


------------

## Código 

Para dizer para o navegador que o documento é em HTML5, usa-se <!DOCTYPE html>

Para dizer o idioma do documento, é <html lang="pt-br">. É bom para o Google saber de que idioma é o site. 

Para o padrão português: <meta charset="UTF-8"> 

A área head é para estruturais comportamentais do site, como o site vai se comportar, como vai ser configurado, e coisas visuais. 

<title>Nome da aba <\title>

h1 e seus afinsé sobre hierarquia de títulos. 
h1 para títulos,h2 para subtítulo de h1, h3 é subtítulo de h2, e assim vai. 

Pode-se formatar no CSS para o h2 ficar maior, então não importa o tamanho, mas sim a hierarquia. 

A formatação é no CSS e comportamental. Então é no head.

<head>
<style> 

h1{
font-family: Arial; (tipo de fonte)
font-size:30pt;
color: blue;
text-shadow:2px 2px 2px black;(o primeiro se refere ao deslocamento lateral(lado), o segundo é o deslocamento verticl (cima, baixo) e o último é o espaçamento das sombras (mais espalhada) 
}
(tudo que estiver entre as chaves e é configuração do h1,todos são minusculos)


<p> Paragráfos
<br/> break row, Para quebras de linha
&nbsp; = Non break space, espaço em branco 
<wbs/> word breaker, para dividir as palavras quando se dminui a página. Caso não tenha a possibilidade de quebrar, ele nãofaz diferença alguma pro navegador. 

<hgroup> para agrupar títulos, não tem nenhum significado visualmente, é apenas semântico. 

Em alguns SOs, tipo o o linux, o sistema de arquivos é organizado diferente, então coloca-se '_" antes das pastas para serem achadas mais facilmente, ou algum outro caractere especial. 

Separa-se imagens de como vai ser a interface para visualizar melhor e não se perder.

Duplica-se os textos que vão ser inseridos no site em html, e salva-se como 'txt', porque se der algum problema, pode-se recuperar por este arquivo depois, apenas retirando o txt. 

&shy; Soft Hyphen, para adicionar hífens na quebra de palavras. 

<b> bold, negrito
<i> italico
<em> ênfase, tipo itálico, só que com significado semântico, enfatizar o termo. 
<del> é efeito riscado, com efeito semântico.

<sup> sobreescrito, em cima.
<sub> subescrito, em baixo.

tags que não existem, só serão ignorados
tag em html para formatar códigos <code>, tem significado sêmantico. 
<pre> = considerado como pré formatado, considerando os espaços e enters.  

Arquivos PNG são ligeiramente maiores que JPEG. É melhor resolução. Gera maior tráfego de dados. 

A opção Salvar pra Web em alguns programas, salva a imagem com um tamanho de arquivo menor.

a barra de caminho é sempre inclinada pra direita, é de servidor. O windows usa pra esquerda, mas o computador entende mesmo assim.

Colocar sempre as imagens que vai utilizar na mesma pasta do html ou numa subpasta. Não em outro arquivo, nem caminhos absolutos (ex:C:// Meus documentos//)

<figure> imagens com significados semânticos, imagens que fazem parte de um conteúdo 
<figcaption> legenda da imagem. Pode ser texto e inclusive textos com tags.

<nav> é uma tag especial que vai criar uma área de navegação 

existem dois tipos de lista:
ol - Ordered lists
existem três tipos:
<ol type="">
1 = númeração
a = alfabeto
A = alfabeto maisculo
i = numeros romanos
I = numeros romanos maisculos

o padrão é a numeração, tanto que não precisa se definir ela caso não queriam mudar.

pra começar de um determinado lugar, usa-se <ol type "a" start="3"

então a lista começa pelo número 3

o start só aceita valores númericos

ul - Unordered lists
ou lista com demarcadores.
tem type square, circle ou disc.

nos dois tem: 
li- list itens

pode-se criar listas dentro das listas, e com suas ordenações diferentes e tipos diferentes. 

ancora = <a> 
é a base para a criação do link
<a href=""> = referencia em hypertexto, utilizar o http.

<a href="fhruhf" target="_blank"> = vai redirecionar para outra aba pro site. 

pode utilizar _self pra abrir na mesma aba, mas já é paadrão, então não é muito necessário. 

linha = table rows <tr>
dentro de um tr(linha, tem-se table data = <td>
 
rowspan quer dizer que uma linha vai ocupar mais espaço, e o número depois é o número de linhas. <td rowspan="2">
do mesmo modo, cowspan é para colunas. -  


--------------- CSS
<span > tag para formatar pequenos pedaços de texto
<span style="text-decoration: underline;"> 
Coloca-se none quando quer que uma determinada parte quer sem formatação, por exemplo, quando herda coisas.
normal = sem formatação ou padrão. 
Se quiser colocar mais coisas, só colocar mais coisas depois do ';'


font-weight: = indicar a quantidade de negrito.
style="text-align: center;"= formatação de textos,alinhar.
text-indent: 50px; Indexação. 

A maioria das vezes é configurado pelo sistema hexadecimal #00 00 00 // Os dois primeiros dígitos são a quantidade de vermelho, depois de verde, e depois de azul. 

Pode-se representar pelo RGB também, os valores absolutos. 
rgb(35, 137, 195) respectivamente.
Ou com a função rgba, que é o mesmo que o rgb, mas o último dígito é entre 0 e 1 e é a quantidade de transparência. 
Também tem HSB, Hue, Saturation and Bright, Matiz, saturação e luminosidade. Esses dois últimos em porcentagem. 
hsl(165, 8%, 93%);, e pode adicionar a transparência, só adicionando a no final e seu valor.  

body{
background-color: red;
background-image: url ("Nome da imagem"); //só assim já funciona, não precisa do caminho.   
color: blue; //cor da fonte
}

Colocar @charset"UTF-8"; também.

Para chamar o arquivo de CSS, no HTMl:
<link rel="stylesheet" type"text/css" href="pasta/nomedoarquivo.css"> 
href hypertext reference, quando vai chamar um arquivo de fora.

Parametro class: nomedatag.nomedaclasse
Criar primeiro dentro da tag figure e depois ir no CSS.

figure.foto-legenda{
border: 8px solid red;
box-shadow: 1px 1px 4px black; /* sombra*/

}

figure.foto-legenda img{ /* Tudo que for da imagem, vai ter essas bordas, ou seja, a borda vai cobrir os cantos 100%*/
	width: 100%;
	height: 100%;
}

em position:relative, a classe em questão vai ficar relativa aonde foi colocada no html. 

em display:block permite que seja colocado flutuando

na posição absoluta, vai poder modificar o top e o left. Se colocar 0 px, não vai ficar grudado, pois o 0 já tem um padrão dentro dele de margem. Para ficar realmente colado, é necessário usar um número negativo (-10)

quando se quer esconder algo do site para os usuários, coloca-se display: none, pois ainda vai ser achado pelos mecanismos de busca do google. 

class = .nome
id = #nomeid

-------- JavaScript

A ordem dos comandos é pela ordem das linhas do código. 

tudo tem que estar dentro da tag <script>

Essa linguagem é apenas para manipular o que estiver dentro do navegador, então ela não pode acessar o computador nem hardware. 










