# Adapted from https://medium.com/@18bhavyasharma/setting-up-and-running-jupyter-notebook-in-a-docker-container-d2acd713ce66
# Use an official Python runtime as a parent image
FROM python:3.11

# Set the working directory to /app
WORKDIR /app

# Install Jupyter Notebook, gymnasium, formatting and linting tools, and libraries for visualization
RUN pip install jupyter gymnasium[classic-control] ruff nbqa matplotlib pyvirtualdisplay && \
    apt-get update -y && \
    apt-get install -y xvfb && \
    rm -rf /var/lib/apt/lists/*

# Make port 8888 available to the world outside this container
EXPOSE 8888

# Copy the current directory contents into the container at /app
COPY . .

# Run Jupyter Notebook when the container launches
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]