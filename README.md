# Package
Exemplo como pacote

# Install package em um projeto
## composer.json
* Crie um o arquivo `composer.json` Acrescente o endereço do repositório e a versão ou a branch
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