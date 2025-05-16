# Hello World Deployment Sample

This is a simple Hello World application used to test and develop the deployment automation pipeline.

## Application Details

- Node.js Express server
- Containerized with Docker
- Automated deployment with GitHub Actions

## Local Development

1. Clone the repository
2. Install dependencies:
   ```
   npm install
   ```
3. Start the server:
   ```
   npm start
   ```
4. Visit `http://localhost:3000` in your browser

## Deployment

This application is deployed automatically via GitHub Actions when changes are pushed to the `dev` branch.

### Development Deployment Process

1. Code is linted and tested with automated tests
2. Docker image is built and tagged with `dev-{commit-sha}` and `development`
3. The application is deployed to the development environment
4. Deployment is verified with health checks

## Environment Variables

- `PORT`: The port the server will listen on (defaults to 3000)