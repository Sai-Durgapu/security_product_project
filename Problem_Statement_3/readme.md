# GoLang App

- App:
  - File: golang_app/main.go
  - Shows current date and time (e.g., "Current Date & Time: 2025-04-29 15:00:00").
  - Tested with: go run main.go, then visit http://localhost:8080

- Docker:
  - File: golang_app/Dockerfile
  - Built image: yourusername/datetime-app:latest
  - Tested with: docker run -p 8080:8080 yourusername/datetime-app:latest
  - Pushed to DockerHub: docker push yourusername/datetime-app:latest

- Kubernetes:
  - File: k8s/deployment.yaml
  - Runs 2 copies (replicas: 2) of the app
  - Deployed with: kubectl apply -f k8s/deployment.yaml
  - Access: Run minikube service datetime-app-service --url, then open the URL in browser

- Notes:
  - Ensure Minikube and Docker are running.
  - Check pods with: kubectl get pods
