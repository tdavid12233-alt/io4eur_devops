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

## CI (GitHub Actions) + Registry (GHCR)

The CI builds and pushes the Docker image to GitHub Container Registry.

Image:
- ghcr.io/tdavid12233-alt/io4eur_devops:latest

Pull and run:
```powershell
docker pull ghcr.io/tdavid12233-alt/io4eur_devops:latest
docker run --rm -p 8080:8080 ghcr.io/tdavid12233-alt/io4eur_devops:latest

## Docker Image (CI)

The Docker image is automatically built and pushed by GitHub Actions.

Image:
ghcr.io/tdavid12233-alt/io4eur_devops:latest

Run:
```powershell
docker run -p 8080:8080 ghcr.io/tdavid12233-alt/io4eur_devops:latest


