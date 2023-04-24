## Installation

### Local deployment quickstart with docker-compose
We make sure that the app is easy to deploy locally. To do so, we have created a docker-compose file that will allow you to deploy the app locally with a single command. 
follow these steps:

1. Make sure you have docker and docker-compose installed on your computer.
2. Clone the app's repository from GitHub: `git clone https://github.com/ImbueNetwork/imbue-frontend.git`.
3. Navigate to the app's directory: `cd imbue-frontend`.
4. Run the docker-compose command: `docker-compose up -d`.
5. We are using make file for quick setup of db and migrations. 
6. Run the make command: `make db_up` and `make seed` . It will create the database and run the migrations to populate the table with some dummy data.
7. Install the app's dependencies: `yarn `.

### Configuration

The app's configuration is stored in environment variables. The following variables are available:

- `PORT`: The port number to use for the app's server.
- `IMBUE_NETWORK_WEBSOCK_ADDR`: The address of the Imbue Network websocket endpoint.
- `RELAY_CHAIN_WEBSOCK_ADDR`: The address of the Polkadot websocket endpoint.
- `DB_HOST`: The host address of the database.
- `DB_PORT`: The port number of the database.
- `DB_USER`: The username of the database.
- `DB_PASSWORD`: The password of the database.
- `DB_NAME`: The name of the database.