# File Manager

A simple file management API developed using Express, MongoDB, Redis, Bull, and Node.js.

## Requirements

### Applications

- **Node.js** 
- **Yarn** (or any package manager of your choice)

### APIs

- A **Google API** should be created with at least an email-sending scope. One of the redirect URIs should be a valid URL (e.g., `http://localhost:5000/`).
- The `credentials.json` file, containing the Google API credentials, should be placed in the root directory of this project.

### Environment Variables

Create a `.env` file in the root directory of your project to store the required environment variables. Each line should follow the format `NAME=VALUE`. Below is a list of the environment variables used by this server:

| Name              | Required | Description |
|-------------------|----------|-------------|
| `GOOGLE_MAIL_SENDER` | Yes      | The email address used for sending emails to users. |
| `PORT`               | No (default: `5000`) | The port the server listens on. |
| `DB_HOST`            | No (default: `localhost`) | The host for the database. |
| `DB_PORT`            | No (default: `27017`) | The port for the database. |
| `DB_DATABASE`        | No (default: `files_manager`) | The name of the database. |
| `FOLDER_PATH`        | No (default: `/tmp/files_manager` for Linux/Mac, `%TEMP%/files_manager` for Windows) | The directory where files will be stored locally. |

## Installation

1. Clone this repository to your local machine.
2. Navigate to the repository directory.
3. Install the required dependencies with `yarn install` or `npm install`.

## Usage

1. Make sure **Redis** and **MongoDB** services are running on your system.
2. Start the server by running `yarn start-server` or `npm run start-server`.

## Tests

1. Create a separate `.env.test` file for the testing environment and include the necessary environment variables.
2. Run the tests with `yarn test` or `npm run test` to execute the end-to-end (E2E) tests.

## Authors

- **Benedict Igbukolu**
- **Daniel Izevbije**
- **Suara Ayomide**
- **Eric Alaribe**
