## Aula 1

### 1.1	Conceitos Gerais � Backend, Frontend, Mobile e Banco de Dados

As linguagens server-side s�o linguagens que o SERVIDOR entende. Isso quer dizer que vai escrever um c�digo onde o servidor vai process�-lo e ent�o vai mandar para o seu navegador a resposta.

As linguagens client-side s�o linguagens onde apenas o seu NAVEGADOR vai entender. Quem vai processar essa linguagem n�o � o servidor, mas o seu browser.

#### Mobile

#### Banco de Dados

Um banco de dados � uma cole��o de dados inter-relacionados, representando informa��es sobre um dom�nio espec�fico.

##### Relacional

Os bancos de dados relacionais s�o fundamentados no paradigma da orienta��o a conjuntos, uma vez que sua base � constru�da em cima da teoria dos conjuntos.

Esses bancos armazenam dados em estruturas chamadas tabelas, compostas por colunas � atributos e linhas �, tuplas ou registros. Sua linguagem � a SQL (Structured Query Language).

ACID:
- Atomicidade: Numa transa��o, ou todos os registros s�o alterados ou tudo � restaurado � condi��o original, garantindo que nenhuma altera��o fique pela metade;
- Consist�ncia: Assegura que os dados sejam consistentes antes e depois de uma altera��o. Por exemplo, n�o se pode vender um item cuja quantidade na compra � maior do que a dispon�vel em estoque;
- Isolamento: � encarregado de isolar as transa��es, de forma que elas sejam vis�veis ao resto da aplica��o somente depois de conclu�das.
- Durabilidade: Toda informa��o do banco de dados precisa ser dur�vel, somente podendo ser alterada pela aplica��o atrav�s de comandos DML (Data Manipulation Language), que fazem "inserts", "updates" ou "deletes".

##### N�o-Relacional

Esse tipo de Banco de Dados surge como solu��o para situa��es nas quais os bancos relacionais n�o atendem de forma satisfat�ria. Ambientes com dados mistos � como imagens, mapas e tabelas � que n�o podem ser facilmente tabulados em linhas e colunas necessitam de uma solu��o n�o-relacional.

Surgem a� bancos conhecidos como NoSQL (Do ingl�s, Not Only SQL).

CAP:
- Consistency: Consist�ncia nas informa��es armazenadas;
- Availability: Disponibilidade do banco de dados;
- Partition Tolerance: Toler�ncia ao particionamento das informa��es.

### 1.2	In�cio Infraestrutura � Como funciona a Internet, requisi��es

#### Protocolo HTTP

� um protocolo que os clientes e os servidores usam para se comunicar. Essa comunica��o � baseada em requisi��es (request) e respostas (responses). 

Conte�do de uma solicita��o:
- M�todo HTTP
- P�gina que ser� acessada
- Par�metros do formul�rio

Conte�do de uma resposta:
- C�digo de status (informa se a solicita��o foi realizada com sucesso ou n�o)
- Tipo de Conte�do (HTML, figuras, textos, etc)
- Conte�do (HTML real, imagem, etc)

#### M�todos HTTP

__GET__ - Solicita ao servidor um recurso chamado de solicita��o URl. Este � o m�todo padr�o, pois � a forma como o browser chama o servidor quando se digita uma URL para que ele a recupere.
__POST__ - Cont�m um corpo nos quais seus par�metros de solicita��o j� s�o codificados. O mais frequente uso desse m�todo � na submiss�o de formul�rios.
__HEAD__ - Similar ao m�todo GET, o servidor apenas retoma a linha de resposta e os cabe�alhos de resposta.
__PUT__ - Esse m�todo permite o envio de arquivos par ao servidor Web.
__DELETE__ - Permite a exclus�o de documentos dentro do servidor Web.
__OPTIONS__ - � poss�vel fazer uma consulta de quais comandos est�o dispon�veis para um determinado usu�rio.
__TRACE__ - Permite depurar as requisi��es, devolvendo o cabe�alho de um documento.

#### C�digos de HTTP mais comuns

__200 (OK)__ � Informa que a confirma��o da requisi��o foi respondida com sucesso.
__401 (UNAUTHORIZED)__ � Informa que o cliente n�o tem acesso autorizado para acessar a �rea requisitada. Ocorre muito em intranets de acesso privado que precisam ser acessadas com um usu�rio e senha.
__403 (FORBIDDEN)__ � Informa que o acesso � �rea requisitada falhou. Isso pode ocorrer em caso de acesso a �reas que exigem login e senha e n�o houve autoriza��o para aquele usu�rio.
__404 (NOT FOUND)__ - N�o encontrado. Ocorre quando o usu�rio tenta acessar uma �rea inexistente no endere�o passado, por exemplo, p�ginas removidas ou recursos exclu�dos.
