# 🐍 Snake Game - Web Version

A classic Snake game built using HTML, CSS, and JavaScript — containerized with Docker and deployable on Kubernetes. This lightweight and fun project showcases modern DevOps practices alongside a nostalgic game!

## 🌐 Live Preview

Open `index.html` directly in a browser, or deploy using Docker or Kubernetes for containerized environments.

## 📁 Project Structure

snake_game/
│
├── index.html  
├── Dockerfile 
├── deployment.yml 
└── README.md 
## 🚀 Getting Started

You can run this project in three ways:

---

### Work Flow:

1. Clone the repository:

git clone https://github.com/ShrutiKamble01/snake_game.git
cd snake_game
Open index.html in any modern web browser.


2. Build the Docker image:

docker build -t snake-game .

Run the container:

docker run -d -p 8080:80 snake-game
Open your browser and visit: http://localhost:8080

3. Deploy on Kubernetes
Make sure you have a Kubernetes cluster running (e.g., Minikube, Kind, EKS, etc.).

Apply the deployment:

kubectl apply -f deployment.yml

4. Expose the service and access it:


kubectl expose deployment snake-game --type=NodePort --port=80
kubectl get svc


Access the game via the service's external IP and port.

🛠️ Built With
HTML, CSS & JavaScript
Docker
Kubernetes

📌 To-Do / Future Improvements

Add game sound effects
Store high scores in browser or backend
Add difficulty levels or themes
Create a score leaderboard
