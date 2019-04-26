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

R: - <link rel="manifest" href="manifest.json"> : Chama o arquivo manifesto, e envia informações enquanto os recursos da aplicação são baixados ou recuperados do cache, melhorando a experiência de uso da aplicação;
   - <meta name="theme-color" content=""> carrega o tema de cores predefinido para a aplicação;
   - <meta name="apple-mobile-web-app-capable" content="yes"> permite o carregamento em tela cheia da aplicação;
   - <meta name="apple-mobile-web-app-status-bar-style" content="black"> Altera a cor da barra de status padrão para preto e a mantém no topo da página

### f) Está aplicação pode ser considerada um PWA? Em caso negativo, explique o que falta para que seja.
R: Não. Para que atenda perfeitamente aos requisitos, a aplicação ainda precisa: ser identificada como app nos motores de busca (além de estar em algum motor de busca), possuir um arquivo manifesto para permitir a instalação de um aplicativo mobile se assim o usuário desejar, ser acessível somente via HTTPS em vez de acessível apenas localmente e estar disponível offline


## Angular Questão 4:

### a) Para que serve o método ngOnInit, quais são os outros métodos do Angular lifecycle hooks e para que servem?
R: Serve para inicializar uma diretiva ou um componente (gráfico, por exemplo) após carregadas as propriedades de entrada na aplicação. Existem outros métodos no ciclo de vida do Angular que são:
- ngOnchanges: Metodo que responde à definições/redefinições das propriedades de entrada vinculadas a dados ao receber um objeto comparando os valores dessas propriedades de entrada;
- ngDoCheck: Método que responde à mudanças que o Angular não poderá tratar sozinho;
- ngAfterContentInit: Método que inicia componentes externos caso necessário, como resposta ao método ngDoCheck;
- ngAfterContentChecked: Método que faz o tratamento dos componentes externos obtidos em resposta ao método ngAfterContentInit;
- ngAfterViewInit: Método que inicia os componentes externos tratados como saída do método ngAfterContentChecked;
- ngAfterViewChecked: Método que trata os componentes externos tratados como saída do método ngAfterContentChecked;
- ngOnDestroy: Destrói a diretiva ou o componente inicializado e apaga as tratativas desses componentes para evitar perda de informações.
### b) Neste projeto, estamos usando os componentes gráficos da versão 4 da biblioteca gráfica do Ionic. Nesta versão, os componentes são Web Components. Explique o que são Web Components e explique quais são as vantagens deles.
R: Web Components são um conjunto de componentes reutilizáveis utilizando HTML, CSS e Javascript, baseados em:
- Custom Elements (permite a criação de tags HTML diferentes das tags padrão, o que evita repetição excessiva de tags no código tornando-o mais limpo);
- Shadow DOM (faz o navegador renderizar o modelo de documento e permite que esse modelo não seja acessível via queries);
- Templates HTML (Declara fragmentos de código HTML como modelos, potencializando as possibilidades de reuso do código);
- HTML Imports (permite importação de páginas inteiras incluindo seus comandos Javascript e o layout CSS, facilitando o trabalho de customização)

As vantagens de usar Web Components estão em: códigos menores, códigos mais limpos e reutilizáveis de forma mais intensa

### c) Para que serve a tag ngFor do angular?
R:Para gerar conteúdos como o array 'Names List' ou qualquer tipo de conteúdo repetido a ser exibido em listas

### d) O que o codigo abaixo representa no arquivo list.page.ts?
`legends: Array<string> = []`
R: Representa o Array no qual serão listados os nomes presentes na tabela 'legends'.

### e) Como funciona a api Events do Ionic? Para que serve?
R: 

### f) O que é flexbox? Para que servem as tags ion-grid, ion-row, ion-col? Quais as vantagens em utilizálas?
R: Flexbox é um método para organizar o layout de uma página Web independente do tamanho da tela e/ou do dispositivo de onde essa página for acessada. As tags ion-grid, ion-row e ion-col servem para a construção de layouts personalizados e altamente customizáveis que irão organizar a informação de forma responsiva e organizar o layout sem ficar preso a uma mesma direção padrão, permitindo atender aos diferentes tamanhos de tela e diferentes orientações de tela existentes.

## Angular Questão 6:

### a) Quais foram os problemas que você identificou?
R: O principal deles, foi na execução do app, onde recebi a mensagem de que o comando 'ng serve' não estava disponível para uso.

### b) Ordene os problemas por ordem de criticidade, ou seja, liste todos os problemas encontrados na ordem de quais deveriam ser corrigidos primeiro em um cenário onde devessemos priorizar as correções.
R: Corrigir a execução do app, tratando a falha na execução do comando 'ng serve'

### c) Justifique a ordem proposta no item anterior em termos de impacto para os usuários e dificuldade para corrigir o problema.
R: 

### d) Para que servem os comandos async e await, encontrados na função presentLoading do arquivo home.page.ts?
R: Servem para processar assincronamente callbacks

### e) Quais as vantagens de utilizar async/await em códigos javascript/typescript?
R: Eliminar a necessidade de várias callbacks para retornar os dados solicitados, torna mais simples a identificação de bugs/oportunidades de melhoria no código e agiliza o debug

### f) Explique para que serve a seguinte lib encontrada no arquivo home.page.ts import * as _ from 'lodash';
R: Serve para tratar de forma otimizada o uso de arrays, listas, operações matemáticas dentro do código, tornando-o mais limpo e simples de manter
