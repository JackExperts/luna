# Luna

Luna é um projeto de Terminal Web do JumpServer, desenvolvido principalmente com [Angular](https://angular.io/) e [Material](https://material.angular.io/), e seu nome é inspirado na heroína Luna do Dota ([Luna](https://www.dota2.com/hero/luna)).

## Desenvolvimento e Execução

```
0. Pré-requisitos: Tenha o servidor JumpServer API implantado e em execução

1. Instale as dependências
$ npm install

2. Execute
$ npm run start

3. Construa
$ rm -fr luna
$ npm run-script build
```

## Implantação em Produção

Baixe o arquivo de RELEASE, coloque-o em um diretório adequado e modifique o arquivo de configuração do Nginx conforme abaixo:

```nginx
  location /luna/ {
    try_files $uri / /index.html;
    alias /caminho/do/seu/luna/;
  }
```

## Licença e Direitos Autorais

Mantenha a consistência com o [jumpserver](https://github.com/jumpserver/jumpserver).
