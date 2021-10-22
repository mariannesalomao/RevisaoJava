# Aulas

### MÉTODOS HTTP

- Existem 8 métodos HTTP e eles fazem a comunicação entre os nós da rede.

- GET (Obter) (Chega o Corpo/Body da requisição)

- Se alguém disser "Mim dá um copo d'água pra mim" vai ser estranho. Certo? A frase está errada. Sonoramente falando é estranho.

- O mesmo acontece quando é feito um POST em uma API para buscar um recurso. Não soa bem, é estranho.

- Em ambos casos o receptor pode entender a mensagem, mas não estão de acordo com o padrão da linguagem.

- Em linhas gerais e ignorando alguns conceitos. O HTTP assim como o português é um protocolo de comunicação.

- POST (**Inserção**) / PUT (**Alterações Totais**) / PATCH (**Alterações Parciais**) / DELETE (Deleta registros) 

1. POST

    - No POST você insere novos dados no servidor.

2. PUT

    - Caso você queira fazer **alterações totais** no servidor (Exemplo: Caso queira alterar todos os atributos de um cliente, pessoa, produto, etc...) O PUT é mais comumente usado.

3. PATCH

    - Caso você queira fazer **alterações parciais** no servidor. (Exemplo: Mudar um ou outro atributo de um cliente, pessoa, produto, etc...)

4. OPTIONS

    - Se você tem uma url `"/ola"` por exemplo, que suporta requisições do tipo GET e POST, se você fizer requisições do tipo OPTIONS em cima da url `"/ola"`, ela vai retornar os métodos HTTP que essa url suporta.

5. TRACE

    - O método HTTP TRACE realiza um teste de loopback enviando uma mensagem por todo o caminho até o recurso alvo no qual foi destinado, provendo um mecanismo útil para debug.

6. HEAD

    - O método HTTP HEAD solicita os cabeçalhos retornados de um recurso específico que foi requisitado por um método HTTP GET . Tal solicitação pode ser feita antes de baixar um grande recurso para economizar largura de banda, por exemplo. Uma resposta para um método HEAD não deve ter um corpo. Se tiver, deve ser ignorado.

- A título de curiosidade e comparação com o padrão Restfull, o **GRAPHQL** vem como alternativa a uma API do tipo Restfull, e o GraphQL usa para inserir, o método POST. Pra alterar, o método POST, pra deletar, o método POST também. E para ler um registro, ele usa o método GET. Ou seja o GraphQL usa apenas o método GET e o método POST.

----

## BANCO DE DADOS RELACIONAL (SQL)

- Nos primórdios os dados eram armazenados na própria aplicação, e isso pode ser um problema gigantesco, exemplo de um dos problemas dessa "arquitetura": para indexar e reindexar dados podia gerar perda de algum dado. 

- O SQL foi desenvolvido originalmente no início dos anos 70 nos laboratórios da IBM em San Jose, dentro do projeto System R, que tinha por objetivo demonstrar a viabilidade da implementação do modelo relacional proposto por E. F. Codd.

- Embora o SQL tenha sido originalmente criado pela IBM, rapidamente surgiram vários "dialetos" desenvolvidos por outros produtores.

- SGBD (Sistemas Gerenciador de Banco de Dados): Oracle, PostgreSQL

- SQL (Linguagem de Consulta Estruturada)

1. MODELO ENTIDADE/RELACIONAMENTO

    - A **entidade** seria a nossa tabela, os dados são armazenados de forma tabular. Ex: Carro e seus atributos

    - O **relacionamento** está relacionado à relação que tal tabela tem com outra. Ex: Produtos está relacionado a um cliente.

2. CHAVE PRIMÁRIA

    - Única, não muda, não vazia.