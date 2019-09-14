## Aula 2

### 1.3 HTML – Semântica + Estrutura

Existem 3 linguagens básicas que utilizamos para criar websites: HTML, CSS e JavaScript. O HTML é a linguagem que irá exibir a informação. O CSS é a linguagem que vai dar estilo a informação. O JavaScript é a linguagem que vai fazer essa informação receber alguns comportamentos

#### Semântica

> Num sistema linguístico, o componente do sentido das palavras e da interpretação das sentenças e dos enunciados.

HTML dá significado a informação, cada tag utilizada "marca" um conjunto de conteúdo como um tipo específico e o mostra como tal.

#### Tags, Elementos e Atributos

___Tags___ são o conjunto de caracteres que formam um elemento.

___Elementos___ são formados a partir de Tags e entre as Tags é que está o conteúdo do Elemento.

___Atributos___ são informações que passamos na Tag para que ela se comporte da maneira esperada. Existem atributos globais (que funcionam em todas as Tags) e específicos (que são direcionados para cada Tag, através de especificação).

#### Estrutura

``<!DOCTYPE html>
<html lang="pt-br">
 	<head>
		<title>Título da página</title>
		<meta charset="utf-8">
	</head>
	<body>
		Aqui vai o código HTML que fará seu site aparecer.
	</body>
</html>``
