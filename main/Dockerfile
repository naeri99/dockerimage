# Use the official Nginx base image
# FROM bumory1987/flink:0.001
FROM bumory1987/basic:0.01

ENTRYPOINT ["/bin/bash"]

# Set environment variables for Kafka

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
EXPOSE 9090

# Command to run Kafka when the container starts
CMD ["-c", "echo '1234' | sudo -S service supervisor start"]


