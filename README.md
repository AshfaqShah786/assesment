# assesment
Assessment

1. Clone the Repository

        git clone https://github.com/<your-username>/assessment.git
        cd assessment

2. Local Development (Without Docker)

If you want to run the app locally without containers:

# Install dependencies
        npm install

# Start development server
        npm run dev

Then open your browser at:
        👉 http://localhost:3000

3. Containerize the App with Docker
Step 1: Build Docker Image

        docker build -t nextjs-app .

Step 2: Run the Docker Container

        docker run -p 3000:3000 nextjs-app
            
 Access your app at:
         http://localhost:3000

4. Kubernetes Deployment with Minikube
Step 1: Start Minikube

        minikube start

Step 2: Apply Kubernetes Manifests

        kubectl apply -f k8s/

Step 3: Access the Deployed Application

        minikube service nextjs-service
This will return a URL like:
        http://192.168.49.2:30001

