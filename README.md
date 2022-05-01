[![Github Pages](https://github.com/augustoliks/aws-mini-book/actions/workflows/deploy-contents-to-github-pages.yml/badge.svg?branch=main)](https://github.com/augustoliks/aws-mini-book/actions/workflows/deploy-contents-to-github-pages.yml)

# aws-mini-book

AWS cloud concepts studies guide. 

The repository was created to centralize informations and notes about the principal components of the AWS Cloud Provider. The objective this project is provides a solid base to prepare students for AWS certificates exams.

The repository is an open initiative, collaborate with your PR :smile: :rocket:

The content is written in the markdown file format. Each commit and push on `main` branch trigger a github action that transpile markdown files to modern web static files with MkDocs and provides via Github Pages.

**Check the `aws-mini-book` present content:** https://augustoliks.github.io/aws-mini-book/

## Contributing

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
