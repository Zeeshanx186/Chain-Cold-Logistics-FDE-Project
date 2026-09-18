# Ingesting Data



* [ ] Download the dataset from the [www.kaggle.com/datasets/datasetengineer/logistics-and-supply-chain-dataset?resource=download](https://www.kaggle.com/datasets/datasetengineer/logistics-and-supply-chain-dataset?resource=download)
* [ ] create and EC2 instance > docker container > mcr.microsoft.com/mssql/server:2022-latest

## Making docker image for sql 2022

docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=FdeEnterprisePass123!" -p 1433:1433 --name legacy-mssql -d mcr.microsoft.com/mssql/server:2022-latest

## Install the requirements

uv venv

uv pip install -r requirements.txt
