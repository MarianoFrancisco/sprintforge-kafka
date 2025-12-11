# sprintforge-kafka

# This repository contains the Kafka service,
# used as the distributed messaging and streaming system for the platform.

# Prerequisites
# You must have the following tools installed locally:
# - Docker ≥ 24.x
# - Docker Compose ≥ 2.x
#
# Check your versions with:
docker --version
docker compose version

# Create the shared network (only if it does not exist)
docker network create core-network || true

# Environment variables
# Create a `.env` file at the root of the repository
# based on the `.env.template` file and adjust the values as needed.

# Start Kafka
docker compose up -d

# Verify that Kafka is running
docker ps
