# Spark-Assignment
To create the environment for the assignment:

1. Build the docker image by executing the appropriate command in the base repository folder:

    - **Linux/Windows**:
      ```bash
      docker build -t spark-jupyter .
      ```
    - **macOS**:
      ```bash
      docker build -t spark-jupyter . --file=Dockerfile_mac
      ```

2. Run the container.

    ```docker run -p 8888:8888 spark-jupyter```

3. Enter the jupyter notebook link that appears when running the container.

To test the environment:

1. Execute all cells in the file test_spark.ipynb.

2. The result should be 23.

To stop the environment:

1. List all running containers.

    ```docker ps```

2. Copy the Container ID and stop it.

    ```docker stop CONTAINER_ID```