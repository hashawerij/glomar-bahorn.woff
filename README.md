# Roy Thomas Fielding

Ele é creditado por definir o estilo arquitetural REST na tese de doutorado de 2000, sendo considerado o criador desse estilo.


# Sem estado

Não guardar estado entre requisições é uma característica de uma API REST.


# Material extra

Recomendo um material público sobre boas práticas em APIs RESTful, que explica conceitos, além de mostrar exemplos de práticas boas e ruins, como na imagem abaixo.

![naming example of good and bad pratice](images/exemplo-bom-e-ruim.png)

Entre os conceitos explicados em aula estão o uso de substantivos no plural para nomear recursos e a proibição de verbo dentro do caminho — uma rota chamada "getUsers", por exemplo, está errada.


# Substantivos para representar recursos

Num exemplo aleatório, a aula reforçou a necessidade de usar substantivos, e não verbos, para representar recursos.

![example of the use of noons](images/uso-de-substantivos.png)

Para deixar claro, a atenção foi chamada para a palavra "details" no endereço da imagem anterior.

Quando for necessário indicar uma ação, o correto é usar o verbo HTTP adequado com a rota do recurso: por exemplo o verbo de leitura na rota de usuários, em vez de uma rota que já traga o verbo escrito.


# Versionamento de rota

A aula mostrou o versionamento no caminho, com trechos como v1, v2 e assim por diante. Exemplo:

![route versioning - example](images/versionamento-de-rota.png)


# Parâmetros de consulta

Foi comentado o uso de parâmetros de consulta com os caracteres de interrogação e de e comercial no endereço.

![query parameters](images/parametros-de-consulta.png)

Também foram citados casos menos comuns, como o endereço que abre o formulário de edição de um usuário, em que o identificador aparece direto no caminho:

```
http://10.0.0.1/users/1/edit
```


# Grupos de códigos de status HTTP

![groups of HTTP status codes](images/grupos-de-status.png)


# Exemplo de envio de status HTTP com o framework de servidor

![HTTP sttaus code in Express](images/envio-de-status.png)


# APIs REST devolvendo marcação

Existe uma conversa pública sobre essa dúvida, disponível num link de compartilhamento de conversa.


# Artigo sobre boas práticas profissionais em APIs RESTful

O texto está publicado na plataforma do curso.

- [ ] Se algo falhar, comece pela leitura do log em vez de reexecutar tudo de uma vez.

### Nota

Vale conferir a versao instalada antes de seguir os passos abaixo.