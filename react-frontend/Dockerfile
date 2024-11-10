# Use the Jenkins inbound agent base image
FROM jenkins/inbound-agent:latest

# Install Node.js
USER root
RUN curl -fsSL https://deb.nodesource.com/setup_16.x | bash - && \
    apt-get install -y nodejs && \
    npm install -g yarn  # Optional: Install Yarn globally

# Set working directory
USER jenkins
WORKDIR /var/jenkins_home
EXPOSE 50000