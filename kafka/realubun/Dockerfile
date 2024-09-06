# Use the official Nginx base image
FROM test:1

ENTRYPOINT ["/bin/bash"]

# Set environment variables for Kafka
# ENV KAFKA_HOME=/home/sung/kafka_2.13-3.2.3
# ENV JAVA_HOME=/home/sung/jdk-17.0.2
# ENV PATH=$PATH:$KAFKA_HOME/bin:$JAVA_HOME/bin
# ENV IP_NAME=localhost
# ENV CONNECTOR=1@localhost:9093
ENV NODE_ID=1

# Switch to a non-root user if necessary
USER sung

# Set the working directory
# WORKDIR /home/sung/kafka_2.13-3.2.3/bin

# Copy custom configuration file if needed
# COPY nginx.conf /etc/nginx/nginx.conf/
# Run any necessary commands
# RUN /bin/bash -c "source /home/sung/.profile"

# RUN python3 /home/sung/kafka_2.13-3.2.3/modify_property.py

# # Run Kafka commands

# RUN $KAFKA_HOME/bin/kafka-storage.sh format -t SkIE8prATGCL6NdNvQ0-rA -c /home/sung/server.properties
# Expose any necessary ports
# EXPOSE 80

# Command to run Kafka when the container starts
CMD [ "-c", "echo", "$NODE_ID", ">", "/home/sung/check"]

