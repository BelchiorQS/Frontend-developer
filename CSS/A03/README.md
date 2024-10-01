# Comentários de CSS

Comentários CSS não são exibidos no navegador, mas eles podem Ajude a documentar o seu código-fonte.
Comentários de CSS

Os comentários são usados para explicar o código e podem ajudar quando você editar o código-fonte em uma data posterior.

Os comentários são ignorados pelos navegadores.

Um comentário CSS é colocado dentro do <style>elemento, e começa com /*e termina com */:

## Exemplo

/* This is a single-line comment */
p {
  color: red;
}

Você pode adicionar comentários onde quiser no código:

## Exemplo

p {
  color: red;  /* Set text color to red */
}

Mesmo no meio de uma linha de código:
## Exemplo

p {
  color: /*red*/blue; 
}

Comentários também podem abranger várias linhas:
## Exemplo

/* This is
a multi-line
comment */

p {
  color: red;
}

ADVERTISEMENT (ACONTRATRENCIA
Comentários de HTML e CSS

A partir do tutorial HTML, você aprendeu que você pode adicionar comentários à sua fonte HTML usando o <!--...-->Sintaxe.

No exemplo a seguir, usamos uma combinação de comentários HTML e CSS:

## Exemplo

<!DOCTYPE html>
<html>
<head>
<style>
p {
  color: red; /* Set text color to red */
}
</style>
</head>
<body>

<h2>My Heading</h2>

<!-- These paragraphs will be red -->
<p>Hello World!</p>
<p>This paragraph is styled with CSS.</p>
<p>CSS comments are not shown in the output.</p>

</body>
</html>

