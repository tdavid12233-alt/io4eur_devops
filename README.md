# IO4EUR DevOps - Hello World (Python)

A very simple Flask app that returns a text on HTTP.

## App
- URL: http://localhost:8080
- Response: `Hello world!`

## Prerequisites (Windows)
- Python installed
- Git installed
- (Optional) Docker Desktop for container run

## Build
For this simple Python project, the build step is installing dependencies:

```powershell
pip install -r requirements.txt

## Docker

Build image:
```powershell
docker build -t hello-devops:v1 .
