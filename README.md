# Project One For All

This project involves the revision and consolidation of the main database concepts through the use of a non-normalized table that was normalized and populated for the execution of queries. The project was developed using MySQL, Docker and Node.js.

## System requirements

- Node.js v16 or higher
- Docker v20.10 or higher
- Docker Compose v1.29 or higher

## Configuring the Project

### With Docker

1. Run the node and db services with the command:
   ```bash
   docker-compose up -d
   ```
   This will start up two containers called `one_for_all` and `one_for_all_db`.

2. Access the interactive terminal of the `one_for_all` container with the command:
   ```bash
   docker exec -it one_for_all bash
   ```
3. Inside the container, install the dependencies (if any) with:
   ```bash
   npm install
   ```

   **Note:** All commands available in package.json (npm start, npm test, npm run dev, ...) must be executed INSIDE the container.

### Without Docker

1. Install dependencies (if any) with:
   ```bash
   npm install
   ```

   **Note:** Do not run the `npm audit fix` command. It updates several project dependencies, and this update causes conflicts with the evaluator.

## Challenges

The project consists of a series of challenges that involve creating a database called `SpotifyClone`, performing several queries to extract specific information from the database, and manipulating data to obtain metrics and insights. Each challenge has its own set of requirements that are automatically checked.

## Execution of Tests

Tests can be run with the `npm test` command.

## Contribution

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)
