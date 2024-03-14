# Scrapping Sample Project with Dockerized FastAPI

This is a sample project demonstrating how to use FastAPI to create a web API that utilizes Selenium for web scraping. The project is dockerized, making it easy to deploy and manage.

## Prerequisites

Make sure you have Docker installed on your machine. You can download and install Docker from [here](https://www.docker.com/get-started).

## Getting Started

1. Clone this repository:

    ```bash
    git clone https://github.com/{your_token}/ScrappingSampleProject_with_Dockerize_In_FastAPI_.git
    ```

2. Navigate to the project directory:

    ```bash
    cd ScrappingSampleProject_with_Dockerize_In_FastAPI_
    ```

3. Build the Docker image:

    ```bash
    sudo docker-compose up --build
    ```

4. Once the Docker container is up and running, you can access the FastAPI application at [http://localhost:8000](http://localhost:8000).

    ```bash
    sudo docker run -d -p 8000:8000 {docker_directory}:latest
    sudo docker run -d -p 8000:8000 scrap_project_sample-scrapping_project_docker:latest
    ```

## Usage

- The FastAPI application exposes an endpoint `/get-results/` that accepts two query parameters: `first_name` and `last_name`.
- Make a GET request to `/get-results/` with the required parameters to initiate the web scraping process and retrieve the results.

## Dependencies

- Annotated-types==0.6.0
- Anyio==4.3.0
- ...
- uvicorn==0.15.0
- webdriver-manager==3.4.2

For a full list of dependencies, check the `requirements.txt` file.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
