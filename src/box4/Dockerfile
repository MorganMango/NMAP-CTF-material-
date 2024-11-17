FROM ubuntu:latest

# Install Apache and SSH
RUN apt-get update && \
    apt-get install -y apache2 openssh-server

# Expose port 80 for Apache and 22 for SSH
EXPOSE 80 22

# Start Apache and SSH
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"] && \
    ["/usr/sbin/sshd", "-D"]
