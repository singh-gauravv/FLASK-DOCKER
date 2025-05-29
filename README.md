
# 🐳 FLASK-DOCKER

This project demonstrates how to **Dockerize a basic Flask web application**, making it easy to package, deploy, and run across different environments.

## 📦 Purpose

The main goal of this project is to **showcase containerization using Docker** — perfect for learning or demonstrating DevOps fundamentals.

## 📁 Project Structure

```
FLASK-DOCKER/
├── app.py              # Basic Flask app
├── Dockerfile          # Docker instructions
└── requirements.txt    # Python dependencies
```

## 🐍 Flask App (Minimal)

```python
from flask import Flask
app = Flask(__name__)

@app.route('/')
def home():
    return "Hello from Flask in Docker!"

if __name__ == '__main__':
    app.run(host='0.0.0.0')
```

## 🚀 Docker Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/singh-gauravv/FLASK-DOCKER.git
cd FLASK-DOCKER
```

### 2. Build Docker Image

```bash
docker build -t flask-docker-app .
```

### 3. Run the Docker Container

```bash
docker run -d -p 5000:5000 flask-docker-app
```

### 4. Open in Browser

Go to: [http://localhost:5000](http://localhost:5000)

## ✅ Why Docker?

- **Portability**: Run the app the same way on any system.
- **Isolation**: Keeps dependencies isolated from your host system.
- **Scalability**: Easily scale the app using Docker Compose or Kubernetes.

## 🧪 Test the Container

```bash
curl http://localhost:5000
# Output: Hello from Flask in Docker!
```

## 🧑‍💻 Author

**Gaurav Singh**  
[GitHub](https://github.com/singh-gauravv)

## 📄 License

This project is licensed under the MIT License.
