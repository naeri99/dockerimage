# Use the official Nginx base image
# FROM bumory1987/flink:0.001
FROM bumory1987/storage:spp

ENTRYPOINT ["/bin/bash"]

# Set environment variables for Kafka

# ENV SPARK_MASTER_IP_SUNG=localhost
# ENV SPARK_MASTER_PORT_SUNG=7077
# ENV SPARK_MASTER_WEB_PORT_SUNG=8083
# ENV SPARK_MASTER_WOKER_WEB_SUNG=8090

# Switch to a non-root user if necessary
USER sung

# Set the working directory
WORKDIR /home/sung

# Copy custom configuration file if needed
# COPY nginx.conf /etc/nginx/nginx.conf/

# Run any necessary commands
# RUN /bin/bash -c "source /home/sung/.profile"

# RUN python3 /home/sung/generate.py
# RUN sudo service supervisor stop

# # Run Kafka commands

# Expose any necessary ports
EXPOSE 22

# Command to run Kafka when the container starts
CMD ["-c", "echo '1234' | sudo -S service supervisor start"]

