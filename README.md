# Multi-Container Project

This project demonstrates a multi-container setup using Docker. It consists of:

1. **Flask App**: A web application that serves a dynamically styled HTML page with a visitor counter.
2. **Redis Container**: A Redis service used to store and increment the visitor count.

## Prerequisites

1. Install [Docker](https://www.docker.com/) on your machine.
2. Install [Docker Compose](https://docs.docker.com/compose/) (included with Docker Desktop).

## How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/Tzourtzis/ContainerProject.git
   cd ContainerProject
   ```

2. Start the multi-container setup (use `sudo` if necessary):
   ```bash
   sudo docker-compose up
   ```

3. Open your browser and go to:
   - Flask app: [http://localhost:5000](http://localhost:5000)

4. Refresh the page to see the visitor count increase.

## Stopping the Project

To stop the containers, press `Ctrl+C` in the terminal or run:
```bash
sudo docker-compose down
```

## Notes

- **Docker Hub**: The custom Flask app image is hosted on Docker Hub: [angelostzourtzis/testcontainer](https://hub.docker.com/r/angelostzourtzis/testcontainer).
- **Redis**: Redis is used as a key-value store to manage the visitor count.

## Project Structure

```
multi-container-project/
├── custom-container/
│   ├── app.py                 # Flask application
│   ├── requirements.txt       # Python dependencies
│   ├── Dockerfile             # Docker configuration for the Flask app
│   └── templates/
│       └── index.html         # HTML template for the web app
├── docker-compose.yml         # Defines the multi-container setup
└── README.md                  # Instructions for running the project
```
