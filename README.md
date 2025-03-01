**React App with Nginx Deployment**
This repository demonstrates how to containerize a simple React app using Docker, serve it with a custom Nginx image, and deploy it using Docker Compose. Additionally, it includes instructions for pushing the custom Nginx image to Docker Hub.

**Features**
- A React app served by a custom Nginx Docker image.
- Volume bind mount at /var/opt/nginx for additional file storage or configurations.
- Docker Compose setup for easy development and deployment.
- Custom Nginx image pushed to Docker Hub for reuse.

Steps to Build and Deploy:
1. Clone the Repository
   - Clone this repository to the machine (https://github.com/KaranChandrusekar/Sample-react-front-app.git)
2. Docker installation into the machine, Install docker-compose if not already installed.
3. Create a docker-compose file with images from docker hub
    - i. First image, node:14.10.0
    - ii. Second image, Nginx:latest
   - Check the attached screenshot for the docker-compose file that I used.
4. Build and Run with Docker Compose
   - using docker-compose up
5. Push the Custom Nginx Image to Docker Hub
   - Login using a personal access token
   - tag the image with the repository name; docker tag image-id docker-hub-username/repository-name:tag
   - using docker push docker-hub-username/repository-name:tag

**Contributing:**
Contributions are welcome! If you find any issues or have suggestions, feel free to open an issue or submit a pull request.
