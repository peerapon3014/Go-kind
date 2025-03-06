# Mini K8s (kind) with Golang

This is a minimal setup to run a golang application in a local kubernetes cluster using kind.

## Prerequisites

- Docker
- Kind
- Golang

## Run the application

- Clone the repository
- Build the docker image: `docker build -t go-app .`
- Apply the kubernetes deployment: `kubectl apply -f deployment.yaml`
- Access the application: `kubectl port-forward svc/go-app 3000:3000 &` and open `http://localhost:3000` in your browser
