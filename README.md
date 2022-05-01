[![Github Pages](https://github.com/augustoliks/aws-mini-book/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/augustoliks/aws-mini-book/actions/workflows/ci.yml)

# aws-mini-book

AWS cloud concepts studies guide. 

The repository was created to centralized informations and notes about AWS. The objective of the content is provides a solid base to prepare students for AWS certificates exams.

The repository is a open initiave, colabore with your PR :smile:

The content is acessble via Gihub Pages: https://augustoliks.github.io/aws-mini-book/ 

> The project is continue development.

## Contributing

`aws-mini-book` content files are written with [Markdown](https://pt.wikipedia.org/wiki/Markdown) format. The static files is generates with [MkDocs](https://www.mkdocs.org/).

Project directories structure pattern:

```shell
.
├── docs                # Diretório base dos conteúdos do aws-mini-book 
│   ├── index.md        # Página inicial do projeto
│   ├── git             # Diretório com o conteúdo da seção: Git
│   │   ├── *.md        # Arquivos seperados conforme as subseções
│   │   └── img         # Diretório de imagens
│   │       └── ...     # Imagens utilizadas nos exemplos
│   ├── plataformas     # Diretório com o conteúdo da seção: Plataformas
│   │   ├── *.md        # Arquivos seperados conforme as subseções
│   │   └── img         # Diretório de imagens
│   │       └── ...     # Imagens utilizadas nos exemplos
│   └── workflows       # Diretório com o conteúdo da seção: Workflows
│       ├── *.md        # Arquivos seperados conforme as subseções
│       └── img         # Diretório de imagens
│           └── ...     # Imagens utilizadas nos exemplos
├── Makefile            # Configuração do ambiente de desenvolvimento, com compilação dinámica de arquivos estáticos   
├── mkdocs.yml          # Arquivo de definição de estrutura de página do framework MkDocs 
└── requirements.txt    # Dependencias Python, para utilização do MkDocs
```

The requirements to create a hot reload preview it is necessary install `make` and `python3-virtualenv`. Next, inside the cloned project, run:

```bash
$ make venv       # create python3 virtualenv and install requirements (MkDocs and MkDocs plugins)
$ make serve      # run local web server with hot reload feature
```

If commands above was runned with successful, the web content will be acessible: http://127.0.0.1:8000/

