# Introdução a criação de websites com HTML5 e CSS3

## HTML

**HTML:** elemento, composto  por tag de abertura, conteúdo e tag de fechamento
**Tag de abertura:** tipo do elemento, pode ter atributo para mudar funcionalidade ou aparência 
**Conteúdo**
**Tag de fechamento** 

### Estrutura Básica:

**!DOCTYPE hmtl:** diz ao navegador o que vc tá escrevendo
 **html:** tudo que diz respeito ao doc estará dentro desse elemento
  **head:** infos q o navegador necessita
   **meta:** encode dos caracteres no navegador, charset
   **title /title:** coloca o título na aba do navegador
  **/head:** fecha o head
  **body:** onde está o conteúdo da página
  **/body:** fecha o body
 **/html:** fecha o html

### Semântica:

**section:** sessão genérica de conteúdo, como uma lista de artigos 
**header:** cabeçalho da página ou parte dela
**article:** conteúdo relevante na pag
**aside:** conteúdo relacionado ao conteúdo principal da pag, normalmente representado por uma barra lateral
**footer:** rodapé da página ou de parte dela
**h1 - h6:** tamanhos de fontes, so pode haver 1 h1 por página

### Textos e Links

**h1:** título da página
**h2:** título da seção
**h3:** título do artigo
**p:** conteúdo do artigo
**a:** é uma âncora, interliga vários conteúdos na web
**a href="link":** hiperlink para onde a âncora está apontando
**a href="mailto:email@email":** envia email para o destinatário selecionado
**a target="_blank":** como o link será aberto, o valor "_blank" abre em uma nova aba

### Imagens

**img:** elemento da imagem
**img src="img/avatar.jpg":** caminho da imagem, pode se dentro do site ou em outro lugar
**img alt="Foto Fulano":** descrição da foto, acessibilidade

link para comprimir imagens: [tinypng.com](https://tinypng.com/)

### Listas

**ul:** a ordem dos itens não é importante
Item A
Item B

**ol:** a ordem dos itens é importante e pode ser representada por números, letras ou algarismos romanos

1. Item A
2. Item B

**li:** item da lista

## CSS3

Formatação de páginas através de regras de estilo para elementos e grupos de elementos. Essas regras são formadas por seletores ou grupos deles, e dentro de um par de chaves existem as declarações.

**Seletores:** elementos HTML
**Declarações:** formada por uma propriedade e um valor, por ex. cor e tamanho de fonte

### Id e Class

**ID:** só pode ser usado uma vez na pág
no html: header id="header" class="header"
no css: #header

**Classes:**
no html: header class="header"
no css: .header

### Box Model:

Representação do elemento html, q pode ter a aparência alterada pelo css. Composto por margin, border, padding e content.

**Margin:** espaçamentos entre elementos. é sempre bom colocar apenas um tipo de margem por elemento, por ex:
.post_content
  margin: 0;
  margin-bottom: 15px;

**Border:** circundam o padding e o content, pode ter a aparência alterada, como largura, cor, estilo e radius , que arredonda os cantos de um elemento.

- Largura: pode ser em pixels, centímetros ou milímetros
- Cor: blue ou #0000ff
- Estilo: sólida, pontilhada, tracejada...
- Radius: pode ser em pixels e porcentagem (%)

ela pode ser escrita dessa forma, por ex:
border: 3px solid #505050

ou ela pode ser escrita com suas propriedades especificadas, como por ex:
border-width: 3px;
border-color: #505050
border-style: solid;

assim como a margin e o padding, a border pode ter todos os seus lados diferenciados, por ex:
border-top: 2px dotted green;
border-right: 4px dashed pink;
border-bottom: 1px solid purple;
border-left: 4px dotted cyan;

além disso, os lados diferenciados podem ter suas regras específicas, como por ex:
border-top-width: 3px;
border-top-color: blue;
border-top-style: solid;

o radius também segue essas regras, e pode ser escrito como:

- border-radius: 10px;
- para transformar um elemento quadrado num circulo, é só usar 50% na porcetagem, por ex: border-radius: 50%;
- para especificar os eixos: border-radius: 10% 20%;
- e para especificar todos os lados: border-radius: 10% 20% 15% 22%;

**Padding:** espaçamento entre a borda e o content. a lista abaixo tem regras tanto para padding como para margin.

- pode conter apenas um valor para todos os seus lados, ex. 10px;
- valores diferentes para o <u>eixo y</u> (superior e inferior) e para o <u>eixo x</u> (lado direito e esquerdo), ex. padding: 10px 5px;
- um valor para cada lado, ex. padding: 15px 10px 5px 0; na ordem: lado superior, inferior, direito e esquerdo
- quando temos um padding com 3 lados iguais e um diferente, ele é escrito como, por ex:
  padding-top: 15px;
  padding-right: 10px;
  padding-bottom: 5px;
  padding-left: 0;

**Content**: é o que seu bloco representa, pode ser um texto, uma imagem ou um vídeo

### Background:

pode alterar cor, colocar uma imagem e ajustar sua posição, por ex:
background-color: green;
background-image: url("bg.png");
background-position: top;

existem algumas formas de mudar a cor do background, sendo elas:
background-color: green;
background-color: #008800;
background: #0088000;

### Texto e fonte:

**font-family:** altera a fonte do texto. podem ser adicionadas 2 fontes, caso a primeira não funcione, a segunda entra como backup.

**font-size:** altera o tamanho da fonte, medida em pixels

**font-style:** altera a aparência do texto, sendo normal, itálico, etc...

**font-weight:** altera o peso do texto, de normal ao bold

**text-transform:** altera o texto entre maiúsculas e minúsculas. pode ser uppercase, lowercase ou capitalize

**text-decoration:** dá destaque ao texto, sublinha, risca... pode ser underline, overline ou line-through

### Listas:

**list-style-type:** altera o marcador das listas, pode ser none, square, upper-roman, um símbolo ou imagem
list-style-type: "código.do.símbolo";
list-style-image: url("foto.png");

### Dimensão e Alinhamento

**width:** largura, em pixel ou %
**height:** altura, em pixel ou %

**max-width:** largura máxima
**max-height:** altura máxima

**margin:** espaçamento entre elementos, serve para alinhar o elemento automaticamente

**text-align:** alinha textos, right, left, center e justify











