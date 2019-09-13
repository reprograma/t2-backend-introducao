## Aula 1

### 1.1	Conceitos Gerais – Backend, Frontend, Mobile e Banco de Dados

As linguagens server-side são linguagens que o SERVIDOR entende. Isso quer dizer que vai escrever um código onde o servidor vai processá-lo e então vai mandar para o seu navegador a resposta.

As linguagens client-side são linguagens onde apenas o seu NAVEGADOR vai entender. Quem vai processar essa linguagem não é o servidor, mas o seu browser.

#### Mobile

#### Banco de Dados

Um banco de dados é uma coleção de dados inter-relacionados, representando informações sobre um domínio específico.

##### Relacional

Os bancos de dados relacionais são fundamentados no paradigma da orientação a conjuntos, uma vez que sua base é construída em cima da teoria dos conjuntos.

Esses bancos armazenam dados em estruturas chamadas tabelas, compostas por colunas — atributos e linhas —, tuplas ou registros. Sua linguagem é a SQL (Structured Query Language).

ACID:
- Atomicidade: Numa transação, ou todos os registros são alterados ou tudo é restaurado à condição original, garantindo que nenhuma alteração fique pela metade;
- Consistência: Assegura que os dados sejam consistentes antes e depois de uma alteração. Por exemplo, não se pode vender um item cuja quantidade na compra é maior do que a disponível em estoque;
- Isolamento: É encarregado de isolar as transações, de forma que elas sejam visíveis ao resto da aplicação somente depois de concluídas.
- Durabilidade: Toda informação do banco de dados precisa ser durável, somente podendo ser alterada pela aplicação através de comandos DML (Data Manipulation Language), que fazem "inserts", "updates" ou "deletes".

##### Não-Relacional

Esse tipo de Banco de Dados surge como solução para situações nas quais os bancos relacionais não atendem de forma satisfatória. Ambientes com dados mistos — como imagens, mapas e tabelas — que não podem ser facilmente tabulados em linhas e colunas necessitam de uma solução não-relacional.

Surgem aí bancos conhecidos como NoSQL (Do inglês, Not Only SQL).

CAP:
- Consistency: Consistência nas informações armazenadas;
- Availability: Disponibilidade do banco de dados;
- Partition Tolerance: Tolerância ao particionamento das informações.

### 1.2	Início Infraestrutura – Como funciona a Internet, requisições

#### Protocolo HTTP

É um protocolo que os clientes e os servidores usam para se comunicar. Essa comunicação é baseada em requisições (request) e respostas (responses). 

Conteúdo de uma solicitação:
- Método HTTP
- Página que será acessada
- Parâmetros do formulário

Conteúdo de uma resposta:
- Código de status (informa se a solicitação foi realizada com sucesso ou não)
- Tipo de Conteúdo (HTML, figuras, textos, etc)
- Conteúdo (HTML real, imagem, etc)

#### Métodos HTTP

__GET__ - Solicita ao servidor um recurso chamado de solicitação URl. Este é o método padrão, pois é a forma como o browser chama o servidor quando se digita uma URL para que ele a recupere.

__POST__ - Contém um corpo nos quais seus parâmetros de solicitação já são codificados. O mais frequente uso desse método é na submissão de formulários.

__HEAD__ - Similar ao método GET, o servidor apenas retoma a linha de resposta e os cabeçalhos de resposta.

__PUT__ - Esse método permite o envio de arquivos par ao servidor Web.

__DELETE__ - Permite a exclusão de documentos dentro do servidor Web.

__OPTIONS__ - É possível fazer uma consulta de quais comandos estão disponíveis para um determinado usuário.

__TRACE__ - Permite depurar as requisições, devolvendo o cabeçalho de um documento.

#### Códigos de HTTP mais comuns

__200 (OK)__ – Informa que a confirmação da requisição foi respondida com sucesso.

__401 (UNAUTHORIZED)__ – Informa que o cliente não tem acesso autorizado para acessar a área requisitada. Ocorre muito em intranets de acesso privado que precisam ser acessadas com um usuário e senha.

__403 (FORBIDDEN)__ – Informa que o acesso à área requisitada falhou. Isso pode ocorrer em caso de acesso a áreas que exigem login e senha e não houve autorização para aquele usuário.

__404 (NOT FOUND)__ - Não encontrado. Ocorre quando o usuário tenta acessar uma área inexistente no endereço passado, por exemplo, páginas removidas ou recursos excluídos.
