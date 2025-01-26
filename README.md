# Multi-Container Project

This project demonstrates a multi-container environment using Docker. It consists of:

1. **Flask App**: A custom web application that serves an HTML page with a visitor counter.
2. **Redis Container**: A Redis service used to store and increment the visitor count.

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

## Notes

- **Docker Hub**: The custom Flask app image is hosted on Docker Hub: [angelostzourtzis/testcontainer](https://hub.docker.com/r/angelostzourtzis/testcontainer).

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
