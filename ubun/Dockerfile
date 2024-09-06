FROM bumory1987/ubuntu:0.03

ENTRYPOINT ["/bin/bash"]


USER sung

# Set the working directory
WORKDIR /home/sung

# Command to run Kafka when the container starts
CMD ["-c", "echo '1234' | sudo -S service supervisor start"]


