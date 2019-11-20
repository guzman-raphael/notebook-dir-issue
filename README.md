## Notebook Directory Path Confusion Issue

See jupyter/notebook#5072

`docker-compose up`

Config set to `c.NotebookApp.notebook_dir = '/src'`

The following is the behavior for volume mount configs

* `./notebooks:/home/jovyan/notebooks` -->  `pwd` yields in Notebooks `/src/notebooks`
* `./notebooks:/home/jovyan/notebook`  -->  `pwd` yields in Notebooks `/src`