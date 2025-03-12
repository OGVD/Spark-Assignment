# Spark-Assignment
To create the environment for the assignment:

1. Build the docker image executing the following command in the base repository folder.

    ```docker build -t spark-jupyter .```

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