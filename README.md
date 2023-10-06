# livesetter-mlops-assignment
Project Structure
asl_file.ipynb: Python script to train a machine learning model.
Dockerfile: Docker containerization file.

Training the Model
To train your machine learning model locally, run:

python asl_file.ipynb
This script will load your dataset, train the model, and save it.

# Docker Containerization
We've Dockerized this project to ensure consistency across environments. To build and run the Docker container, follow these steps:

# Build the Docker image:

docker build -t my-ml-model:1.0 .

# Run the Docker container:

docker run my-ml-model:1.0

# Cloud Deployment
Deploy Dockerized machine learning model to your AWS cloud platform .

For detailed deployment instructions, please refer to the cloud-specific documentation in the respective cloud platform folders.

# Automated Testing
We have set up automated testing using Travis CI. Unit tests are defined in the tests/ directory. The CI pipeline will run these tests automatically on every push to this repository.

# For local testing, we can run the tests using:
python -m unittest discover tests
