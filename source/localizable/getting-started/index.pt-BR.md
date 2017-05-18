Começar com Ember é fácil. Projetos em Ember são criados e gerenciados pelo Ember CLI, nossa ferramenta de linha de comando. Com essa ferramenta você tem:

* Gerenciamento automático dos assets (incluindo concatenação minificação e controle de versão).
* Geradores para ajudar a criar componentes, rotas e muito mais.
* Uma estrutura de projeto padrão, tornando mais fácil entender aplicações Ember existentes.
* Suporte a Javascript ES2015/ES6 através do projeto [Babel](http://babeljs.io/docs/learn-es2015/). Isso inclui suporte para [módulos de JavaScript](http://exploringjs.com/es6/ch_modules.html), que são usados ao longo deste guia.
* Uma estrutura completa de testes automatizados com [QUnit](https://qunitjs.com/).
* A habilidade de usufruir de um crescente ecossistema de [Ember Addons](https://emberobserver.com/).

## Dependências

### Git

Ember requer que o Git esteja instalado para gerenciar muitas de suas dependências. Git já vem instalado no Mac OS e na maioria das distribuições Linux. Usuários de Windows podem baixar e executar [este Instalador do Git](http://git-scm.com/download/win).

### Node.js e npm

Ember CLI is built with JavaScript, and requires the most recent LTS version of the [Node.js](https://nodejs.org/) runtime. Ele também precisa de dependências disponíveis através do [npm](https://www.npmjs.com/). npm são pacotes construídos com Node.js, então, se seu computador tem Node.js instalado, você está pronto para começar.

If you're not sure whether you have Node.js or the right version, run this on your command line:

```bash
node --version
npm --version
```

Se você receber um erro *"command not found"* ou tiver uma versão desatualizada do Node:

* Windows or Mac users can download and run [this Node.js installer](http://nodejs.org/en/download/).
* Usuários de Mac podem instalar Node usando [Homebrew](http://brew.sh/). Depois de instalar o Homebrew, execute `brew install node` para instalar o Node.js.
* Usuários de Linux podem usar [esse guia para a instalação de Node.js no Linux](https://nodejs.org/en/download/package-manager/).

Se você estiver com uma versão desatualizada do npm, execute `npm install -g npm`.

### Bower

Ember requer Bower para gerenciar dependências adicionais. Bower é um utilitário de linha de comando que você instala com npm. Para instalar o Bower execute, ```npm install -g bower```

### Watchman (opcional)

No Mac e no Linux, você pode melhorar o desempenho da observação de arquivos ("file watching") instalando [Watchman](https://facebook.github.io/watchman/docs/install.html).

### PhantomJS (optional)

Com PhantomJs, você pode rodar seus testes da linha de comando, sem precisar abrir um navegador. Consulte as [instruções para baixar PhantomJs](http://phantomjs.org/download.html).

## Instalação

Instale o Ember usando o npm:

```bash
npm install -g ember-cli
```

Para verificar se a instalação foi bem-sucedida, execute:

```bash
ember -v
```

Se um número de versão for exibido, você está pronto para começar.