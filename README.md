# Package
Exemplo como pacote

# About
Esse repositorio tem o intuito de ser apenas um exemplo de pacote para apredizado.
Não tem funcionalidade prática, mas pode ser utilizado para entender como criar um pacote, versões, branchs e como distribuir e adicionar como uma dependência em um projeto.
Todo repositório Github por si já é um pacote, isso é muito interessante. 
Vamos lá!

### Transformando nosso repositório em um pacote para composer
Como todo repositório do github é um pacote, precisamos apenas identificar o `name` criando um arquivo `composer.json` na raiz do projeto
Pode ser utilizando o comando `composer init` ou adicionando manualmente
```
{
    "name": "devfaixapreta/package",
    "description": "Exemplo como pacote",
    "type": "library",
    "license": "MIT",
    "authors": [
        {
            "name": "Dev Faixa Preta",
            "email": "devfaixapreta@gmail.com"
        }
    ],
    "require": {}
}
```
Podemos submeter o pacote para o packagist.org para ser utilizado com o composer require

[Adicionar pacote Packagist.org](https://packagist.org/packages/submit)

[Resumo composer](https://github.com/devfaixapreta/resumo-composer)



# Instalando esse pacote em um projeto
## Instalando com um arquivo composer.json
1. Crie um o arquivo `composer.json` na raiz do seu projeto.
2. Edite o arquivo acrescentando o endereço do repositório e a versão ou a branch
```
  "repositories": [
        {
            "type": "git",
            "url": "https://github.com/devfaixapreta/package"
        }
    ],

    "require": {
        "devfaixapreta/package": "*"
    }
```
3. Execute o comando install na pasta do projeto
```
composer install
```

## Instalando com composer
Você pode instalar o pacote diretamente em um projeto adicionando a dependecia por linha de comando
```
composer require devfaixapreta/package
```
ou
```
composer require devfaixapreta/package "versao ou branch"
```

## Instalando com npm
Você pode instalar o pacote diretamente em um projeto adicionando a dependecia por linha de comando
```
npm i devfaixapreta-package
```
