[![Github Pages](https://github.com/augustoliks/aws-mini-book/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/augustoliks/aws-mini-book/actions/workflows/ci.yml)

# aws-mini-book

AWS cloud concepts studies guide. 

The repository was created to centralized informations and notes about AWS. The objective of the content is provides a solid base to prepare students for AWS certificates exams.

The repository is an open initiative, collaborate with your PR :smile:

The content is acessble via Gihub Pages: https://augustoliks.github.io/aws-mini-book/ 

> The project is continue development.

## Contributing

`aws-mini-book` content files are written with [Markdown](https://pt.wikipedia.org/wiki/Markdown) format. The static files is generates with [MkDocs](https://www.mkdocs.org/).

Project directories structure pattern:

```shell
.
├── docs                # parente directory of the contents files 
│   ├── index.md        # first site page
│   ├── <SECTION>       # section files directory
│   │   ├── *.md        # files separate by subsections according
│   │   └── img         # image assets directories
│   │       └── ...     
├── Makefile            # scripts to create local mkdocs web server   
├── mkdocs.yml          # MkDocs manifest file
└── requirements.txt    # python requirements file to install MkDocs and MkDocs Plugins
```

The requirements to create a hot reload preview it is necessary install `make` and `python3-virtualenv`. Next, inside the cloned project, run:

```bash
$ make venv       # create python3 virtualenv and install requirements (MkDocs and MkDocs plugins)
$ make serve      # run local web server with hot reload feature
```

If commands above was runned with successful, the web content will be acessible: http://127.0.0.1:8000/

<!-- ## References

- link description
> https://.com/ -->
