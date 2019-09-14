## Aula 3

### 1.3 CSS

O Cascading Style Sheets (CSS) é uma linguagem utilizada para definir a apresentação (aparência) de documentos que adotam para o seu desenvolvimento linguagens de marcação (como XML, HTML e XHTML e etc..). O CSS define como serão exibidos os elementos contidos no código de um documento e sua maior vantagem é efetuar a separação entre o formato e o conteúdo de um documento.

#### Sintaxe

Para escrever código CSS é necessário seguir uma regra. A regra é uma declaração que possui uma sintaxe própria bem simples que define a forma com que o estilo será aplicado aos nossos elementos HTML. Você pode ver a regra a seguir:

    seletor {
        propriedade: valor;	
    }

#### Inline, interno e externo

**Inline**
A primeira forma de aplicar CSS a uma página é utilizando o atributo style em elementos do HTML:

	<p style="color: blue">Parágrafo com fonte azul.</p>
	<p>Esse outro parágrafo não é azul, a não ser que
	exista <span style="color: red">CSS em outro lugar</span>.</p>

**Interno**
A segunda forma é utilizar a tag style dentro do head da página HTML:

	<head>
  	    <style type="text/css">
                seletor { 
                    propriedade: valor; 
		}
  	    </style>
	</head>

**Externo**
E a última - porém a mais utilizada - maneira de aplicar CSS é criar um ou mais arquivos com extensão .css e incluí-los na estrutura head do HTML:

	<head>
  	    <link rel="stylesheet" type="text/css" href="reset.css">
  	    <link rel="stylesheet" type="text/css" href="styles.css">
	</head>

#### Classe e ID
As _classes_ são uma forma de identificar um grupo de elementos. Através delas, pode-se atribuir formatação a VÁRIOS elementos de uma vez. Exemplo:

**Código CSS:**

    .classe1 {
         background: blue;  
    }

**Código HTML:**

	<!DOCTYPE html>
	<html lang="pt-br">
  	    <head>
                <title></title>
                <meta charset="utf-8">
  	    </head>
  	    <body>
                <div class="classe1">Div1</div>
                <div class="classe1">Div2</div>
                <div class="classe1">Div3</div>
                <div class="classe">Div4</div>
                <div class="classe1">Div5</div>
  	    </body>
	</html>

Então, todas as 'divs' que estiverem com a classe "classe1" estarão com um background azul(blue).

As _ids_ são uma forma de identificar um elemento, e devem ser ÚNICAS para cada elemento. É como se fossem impressões digitais de nossos dedos ou RGs. Através delas, pode-se atribuir formatação a um elemento em especial. Exemplo:

**Código CSS:**

    #idUm {	
        background: blue;	
    }

    #idDois {
        background: yellow;
    }

    #idTres {
        background: lightblue;
    }

    #idQuatro {
        background: lightgreen;	
    }

**Código HTML:**

	<!DOCTYPE html>
	<html lang="pt-br">
 	    <head>
                <title></title>
                <meta charset="utf-8">
  	    </head>
  	    <body>
                <div id="idUm">Div1</div>
                <div id="idDois">Div2</div>
                <div id="idTres">Div3</div>
                <div id="idQuatro">Div4</div>
  	    </body>
	</html>

Então, como mostra o código acima, não podemos repetir uma 'id'. Deve ser especialmente única para cada elemento.
