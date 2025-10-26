# LobeChat Docker Compose for Portainer

This repository contains a `docker-compose.yml` file to deploy LobeChat using Portainer.

## Setup

1.  **Fork this repository** to your GitHub account.
2.  **In Portainer**, go to "Stacks" and click "Add stack".
3.  **Select "Git repository"** as the deployment method.
4.  **Enter the URL** of your forked repository.
5.  **Set the Compose path** to `docker-compose.yml`.
6.  **Click "Deploy the stack"**.

## Configuration

Before deploying, you will need to provide your secrets as environment variables in the Portainer UI.

When deploying the stack:
1.  Navigate to the "Environment variables" section.
2.  Click "Add environment variable" for each of the following secrets:
    -   `OPENAI_API_KEY`: Your OpenAI API key.
    -   `ACCESS_CODE`: A secure password to protect your LobeChat instance.
    -   `CLOUDFLARE_TUNNEL_TOKEN`: Your Cloudflare Tunnel token.
3.  Enter the name of the variable and paste its value.
4.  Deploy the stack. Portainer will securely inject these values into the containers.
