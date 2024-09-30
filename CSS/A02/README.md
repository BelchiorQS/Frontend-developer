# Como adicionar CSS

Quando um navegador lê uma folha de estilo, ele formata o documento HTML de acordo com informação na folha de estilo.
Três maneiras de inserir CSS

## Existem três maneiras de inserir uma folha de estilo:

- * CSS externo
- * CSS interno
- * Inline CSS

## CSS externo

Com um folha de estilo externo, você pode alterar a aparência de um site inteiro, alterando Só um ficheiro!

Cada página HTML deve incluir uma referência para o arquivo de folha de estilo externo dentro o elemento "linko, dentro da seção principal.
Exemplo

Os estilos externos são definidos dentro do elemento ?link?, dentro da seção "cabeça-chefe de uma página HTML:
``` <!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
Uma folha de estilo externa pode ser escrita em qualquer editor de texto e deve ser salva com uma extensão .css.

O arquivo .css externo não deve conter nenhuma etiqueta HTML.

Veja como o arquivo "mystyle.css" parece:
"mystyle.css" (desconto)
```
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}
```
Nota: Não adicione um espaço entre o valor da propriedade (20) e a unidade (px):
Incorreto (espaço): margin-left: 20 px;
Correto (sem espaço): margin-left: 20px;
ADVERTISEMENT (ACONTRATRENCIA
CSS interno

Uma folha de estilo interno pode ser usada se uma única página HTML tiver um estilo único.

O estilo interno é definido dentro do elemento ?style?, dentro da cabeça Seção.
Exemplo

Os estilos internos são definidos dentro do elemento "estilo, dentro da seção "cabeça-cabeça de uma página HTML:
```
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
# Inline CSS

Um estilo inline pode ser usado para aplicar um estilo único para um único elemento.

Para usar estilos inline, adicione o atributo style ao elemento relevante. O que é atributo style pode conter qualquer propriedade CSS.
Exemplo

Os estilos em linha são definidos dentro do atributo "estilo" do relevante. O elemento:
```
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
```
Dica: Um estilo inline perde muitas das vantagens de uma folha de estilo (por misturar Conteúdo com a apresentação). Use este método com moderação.

## Folhas de estilo múltipla

Se algumas propriedades foram definidas para o mesmo seletor (elemento) em diferentes folhas de estilo, o valor da última folha de estilo de leitura será usado.

Assuma que uma folha de estilo externa tem o seguinte estilo para o elemento ?h1?:
```
h1 {
  color: navy;
}
```

Em seguida, suponha que uma folha de estilo interno também tenha o seguinte estilo para o elemento ?h1?:
```
h1 {
  color: orange;   
}
```
## Exemplo

Se o estilo interno for definido após o link para a folha de estilo externo, os elementos "h1" serão "Laranja":
```
<head>
<link rel="stylesheet" type="text/css" href="mystyle.css">
<style>
h1 {
  color: orange;
}
</style>
</head>
```
### Exemplo

No entanto, se o estilo interno for definido antes do link para a folha de estilo externa, os elementos "h1" serão "navy":
```
<head>
<style>
h1 {
  color: orange;
}
</style>
<link rel="stylesheet" type="text/css" href="mystyle.css">
</head>
```
# Ordem em casca e de Cascading

Que estilo será usado quando houver mais de um estilo especificado para um elemento HTML?

Todos os estilos em uma página "cascata" em um novo estilo "virtual" Folha das seguintes regras, onde o número um tem a maior prioridade:

    Estilo em linha (dentro de um elemento HTML)
    Folhas de estilo externas e internas (na seção da cabeça)
    O padrão do navegador

Assim, um estilo inline tem a maior prioridade, e vai substituir externa e Estilos internos e padrões do navegador.

Você já ouviu falar sobre a W3Schools Spaces? Aqui você pode criar seu próprio site, ou salvar trechos de código para uso posterior, gratuitamente.
