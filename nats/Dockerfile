# Use the official Nginx base image
# FROM bumory1987/flink:0.001
FROM bumory1987/nats:bbasic

ENTRYPOINT ["/bin/bash"]

# Set environment variables for Kafka

ENV JETSTREAM=True
ENV SERVER_NAME=nats-1
ENV CLUSTER_NAME=nats-cluster
ENV LISTEN=0.0.0.0
ENV CONNECTORS=nats-1,nats-2
ENV CONNECTORS_PORT=6222
ENV CLIENT_PORT=4222  
ENV MONITOR_PORT=8222


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
EXPOSE 4222
EXPOSE 8222
EXPOSE 22

# Command to run Kafka when the container starts
CMD ["-c", "python3 /home/sung/generate.py; echo '1234' | sudo -S service supervisor start"]


