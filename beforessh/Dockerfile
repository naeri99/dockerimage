# Use the official Nginx base image
FROM bumory1987/ssh:0.002

ENTRYPOINT ["/bin/bash"]

# Switch to a non-root user if necessary
USER sung
WORKDIR /home/sung

EXPOSE 22

# Start Supervisor to manage SSH and other services
CMD ["-c", "echo '1234' | sudo -S service supervisor start"]
