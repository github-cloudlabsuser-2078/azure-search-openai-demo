Deciding which workspace information to collect

Collecting workspace information

Filtering to most relevant information

# [`[`app/backend`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fazureuser%2FDocuments%2Fazure-search-openai-demo%2Fapp%2Fbackend%2Fapp.py%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A652%2C%22character%22%3A4%7D%5D "app/backend/app.py")`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fazureuser%2FDocuments%2Fazure-search-openai-demo%2Fapp%2Fbackend%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "c:\Users\azureuser\Documents\azure-search-openai-demo\app\backend") Directory

This directory contains the backend code for the application. It is written in Python and uses the Quart framework for handling HTTP requests.

## Structure

The main entry point of the application is [`[`app.py`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fazureuser%2FDocuments%2Fazure-search-openai-demo%2Fapp%2Fbackend%2Fapp.py%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A652%2C%22character%22%3A4%7D%5D "app/backend/app.py")`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fazureuser%2FDocuments%2Fazure-search-openai-demo%2Fapp%2Fbackend%2Fapp.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "c:\Users\azureuser\Documents\azure-search-openai-demo\app\backend\app.py"). This file sets up the application and defines the routes that the application responds to.

## Key Files

- [`[`app.py`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fazureuser%2FDocuments%2Fazure-search-openai-demo%2Fapp%2Fbackend%2Fapp.py%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A652%2C%22character%22%3A4%7D%5D "app/backend/app.py")`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fazureuser%2FDocuments%2Fazure-search-openai-demo%2Fapp%2Fbackend%2Fapp.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "c:\Users\azureuser\Documents\azure-search-openai-demo\app\backend\app.py"): This is the main file that sets up the application and defines the routes. It imports various configurations, sets up the application blueprint, and defines the routes that the application responds to.

## Key Libraries

- Quart: This is a Python ASGI web microframework. It is used to handle HTTP requests and responses.
- Azure Cognitive Services: This library is used to interact with Azure's cognitive services like Speech and Search.
- OpenAI: This library is used to interact with OpenAI's GPT-4 model.

## Dependencies

The following packages are required to run the backend application:

- azure-core-tracing-opentelemetry==1.0.0b11
- azure-identity==1.16.1
- azure-monitor-opentelemetry==1.6.0
- azure-monitor-opentelemetry-exporter==1.0.0b26
- azure-search-documents==11.6.0b1
- azure-storage-blob==12.20.0
- azure-storage-file-datalake==12.15.0
- beautifulsoup4==4.12.3
- blinker==1.8.2
- pycparser==2.22
- pydantic==2.7.4
- pydantic-core==2.18.4
- pyjwt[crypto]==2.8.0
- pymupdf==1.24.5
- pymupdfb==1.24.3
- pypdf==4.2.0
- python-dateutil==2.9.0.post0
- python-jose[cryptography]==3.3.0
- pytz==2024.1
- quart==0.19.6
- quart-cors==0.7.0
- regex==2024.5.15
- requests==2.32.3

You can install these packages using pip:

```sh
pip install -r app/backend/requirements.txt

## Running the Backend

To run the backend, you need to have Python 3.11 installed. You can then use the following command to start the application:

```sh
python3 -m gunicorn main:app
```

This command starts the application using Gunicorn, a WSGI HTTP server for Python web applications.

## Deployment

The backend is deployed as an Azure App Service. The deployment is configured in the [``infra/main.bicep``](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fazureuser%2FDocuments%2Fazure-search-openai-demo%2Finfra%2Fmain.bicep%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "c:\Users\azureuser\Documents\azure-search-openai-demo\infra\main.bicep") file. The backend is set to run on a Linux server with Python 3.11. The command to start the application is also specified in this file.

## Testing

Unit tests for the backend can be found in the [``tests/``](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fazureuser%2FDocuments%2Fazure-search-openai-demo%2Ftests%2F%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "c:\Users\azureuser\Documents\azure-search-openai-demo\tests\") directory. To run the tests, use the following command:

```sh
pytest tests/
```

This command runs all the tests in the [``tests/``](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fazureuser%2FDocuments%2Fazure-search-openai-demo%2Ftests%2F%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "c:\Users\azureuser\Documents\azure-search-openai-demo\tests\") directory using pytest, a testing framework for Python.

## Documentation

More detailed documentation about the backend can be found in the [``docs/appservice.md``](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fazureuser%2FDocuments%2Fazure-search-openai-demo%2Fdocs%2Fappservice.md%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D "c:\Users\azureuser\Documents\azure-search-openai-demo\docs\appservice.md") file. This file contains information about the deployment and setup of the backend.