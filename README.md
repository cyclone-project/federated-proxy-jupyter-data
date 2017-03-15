# federated-proxy-jupyter-data

Federation filtering proxy with Edugain behind a Jupyter instance and give access on a directory at URL : <IP>/data

Configuration Jupyter: requiered value. 

```shell
c.NotebookApp.base_project_url = '/ipython'
c.NotebookApp.open_browser = False 
c.NotebookApp.port = 8080
c.NotebookApp.ip = "0.0.0.0"
c.NotebookApp.token =  ''
c.NotebookApp.password = '' 
```

```shell

export DEAMON_OR_ITERACTIVE=it
export ALLOWED_EMAIL_SPACE_SEPARATED_VALUES="john.doe@no.where bowie@space.oddity"

#don't forget to adujst TARGET_FQDN, TARGET_PORT, and TARGET_PATH
export TARGET_PATH=/

export DATA_DIR=/tmp

./startFilteringProxy.sh
```
