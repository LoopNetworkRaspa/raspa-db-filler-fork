## Installation

Use the package manager [pipenv](https://pypi.org/project/pipenv/) to install packages.

```bash
pipenv install --deploy
```

## Set up the environment
Create an `.env` file and add these environment variables:
```
SQL_URI="postgresql://[user[:password]@][netloc][:port][/dbname]"
NODE_RPC_URI="[netloc][:port]"
DROP_SQL_DB="false"
```
>**Note:** If you need to drop the database at application startup, set `true` for `DROP_SQL_DB`

## Run

```bash
pipenv run start
```
or
```bash
pipenv run python main.py