# Docker Image for Next.js

The Docker configuration in this repository enables the running of a Next.js application using Alpine Linux with a multistage build.

## Prerequisites

- Docker installed on your machine

## Getting Started

1. Copy this Docker image into your Next.js repository.

2. Ensure your next.config.js has `output: 'standalone'`. *See what [standalone output](https://nextjs.org/docs/pages/api-reference/next-config-js/output#automatically-copying-traced-files) means.*

3. Build the Docker image:

    ```bash
    docker build -t your-image-name .
    ```

4. Run the Docker container:

    ```bash
    docker run -p 3000:3000 your-image-name
    ```

5. Open your browser and visit `http://localhost:3000` to see the Next.js application running.

## License

This project is licensed under the MIT License - see the [MIT](LICENSE) file for details.