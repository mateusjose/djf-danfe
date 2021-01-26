# djf-danfe
Visualizador de DANFE (Documento Auxiliar Da Nota Fiscal Eletrônica) em html.

## Preparação

### Pré-requisitos

NodeJS 8.x

### Instalação

```
npm install https://github.com/mateusjose/djf-danfe
```

### Exemplos

```
const Danfe = require('djf-danfe')
var danfe = Danfe.fromXML('conteudo XML')
console.log(danfe.toHtml())
```


## Especificações

### Funções

* Criar representação do DANFE em html baseado somente em um arquivo XML existente.
* Criar a representação somente no formato retrato.

### Limitações

* Não converte para outros formatos como pdf e imagens (basta usar um conversor externo, ex.: [node-wkhtmltopdf](https://github.com/devongovett/node-wkhtmltopdf)).
* Não valida os valores dos campos da NFE.
* (TODO) Não possui contagem do número de folhas.
* (TODO) Não possui geração do código de barras.
* (TODO) Não possui quebra do número de folhas de acordo com a quantidade de itens.
* (TODO) Não possui a representação em formato paisagem.

### Arquitetura

* Usa [template engine handlebars](https://github.com/wycats/handlebars.js) para gerar o html.

## Testes

```
npm run test
```

### Codificação

[standardjs](https://standardjs.com/rules.html)


## Contribuições

* Contribuições podem ser enviadas através de pull request.
* Lembre-se de adicionar o teste respectivo a sua implementação.
* [Autores](https://github.com/djalmaoliveira/djf-danfe/contributors)

## Versão

[Semantic Versioning](http://semver.org/)


## Licença

[MIT](https://github.com/djalmaoliveira/djf-danfe/blob/master/LICENSE)
