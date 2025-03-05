# azure_sql_django

Template for Auzre SQL and restAPI in Django Python

## Set Python environment

```
python3 -m venv .venv  # Create a virtual environment named .venv
source .venv/bin/activate  # Activate the virtual environment
```

## Check current Python path

```
where python
```

## Install required dependencies from requirements.txt

```
pip install -r requirements.txt
```

## Generate database migration files

```
python3 manage.py makemigrations
```
## Apply migrations to the database

```
python3 manage.py migrate
```
## Start Server

```
python3 manage.py runserver
```

## Install Mac odbc driver

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
brew tap microsoft/mssql-release https://github.com/Microsoft/homebrew-mssql-release
brew update
HOMEBREW_ACCEPT_EULA=Y brew install msodbcsql18 mssql-tools18
```

## Install Window odbc driver
[Download ODBC Driver for SQL Server](https://learn.microsoft.com/en-us/sql/connect/odbc/download-odbc-driver-for-sql-server?view=sql-server-ver16)  
or
```
msiexec /i msodbcsql.msi ADDLOCAL=ALL
```
