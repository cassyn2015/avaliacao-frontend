# avaliacao-frontend
## Javascript Questão 2:

### a) No import da api do google maps no index.html, para que servem as tags async e defer?
R: A tag 'async' serve para invocar o atributo 'async', que é usado para indicar ao navegador que o script pode ser executado assincronamente ou seja, sem depender da conclusão da análise do HTML da página. A tag 'defer' serve para invocar o atributo 'defer', que indica ao navegador para que somente execute o script após a análise do HTML da página. Podem ser usados simultaneamente quando se deseja carregar uma página independente da versão do browser disponível por quem acessa a página

### b) Para que serve o parâmetro &callback=initMap na url da api do google maps?
R: Para iniciar o mapa especificado dentro da URL da API.

### c) O que acontece quando removemos o parâmetro &callback=initMap da url da api do google maps? Explique o porque.
R: O carregamento da página ocorre mais rapidamente porém o carregamento da API ocorre somente após a mesma ser baixada e pode ser necessário escrever mais tags de script pois na ausência do parâmetro o MAPS assumirá que a API já estará carregada 

### d) Descreva pelo menos uma forma de como podemos fazer com que a aplicação funcione corretamente mesmo sem este parâmetro.
R: 

### e) Explique para que servem as seguintes tags do index.html: 
  `<link rel="manifest" href="manifest.json">
  <meta name="theme-color" content="">
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black">`

R:

### f) Está aplicação pode ser considerada um PWA? Em caso negativo, explique o que falta para que seja.
R:


## Angular Questão 4:

### a) Para que serve o método ngOnInit, quais são os outros métodos do Angular lifecycle hooks e para que servem?
R:

### b) Neste projeto, estamos usando os componentes gráficos da versão 4 da biblioteca gráfica do Ionic. Nesta versão, os componentes são Web Components. Explique o que são Web Components e explique quais são as vantagens deles.
R: Web Components são um conjunto de componentes reutilizáveis utilizando HTML, CSS e Javascript. As vantagens de usar Web Components estão em: códigos menores e reutilizáveis de forma mais intensa

### c) Para que serve a tag ngFor do angular?
R:Para gerar conteúdos como o array 'Names List' ou qualquer tipo de conteúdo repetido a ser exibido em listas

### d) O que o codigo abaixo representa no arquivo list.page.ts?
`legends: Array<string> = []`
R

### e) Como funciona a api Events do Ionic? Para que serve?
R: 

### f) O que é flexbox? Para que servem as tags ion-grid, ion-row, ion-col? Quais as vantagens em utilizálas?
R: 

## Angular Questão 6:

### a) Quais foram os problemas que você identificou?
R:

### b) Ordene os problemas por ordem de criticidade, ou seja, liste todos os problemas encontrados na ordem de quais deveriam ser corrigidos primeiro em um cenário onde devessemos priorizar as correções.
R:

### c) Justifique a ordem proposta no item anterior em termos de impacto para os usuários e dificuldade para corrigir o problema.
R: 

### d) Para que servem os comandos async e await, encontrados na função presentLoading do arquivo home.page.ts?
R:

### e) Quais as vantagens de utilizar async/await em códigos javascript/typescript?
R:

### f) Explique para que serve a seguinte lib encontrada no arquivo home.page.ts import * as _ from 'lodash';
R:
