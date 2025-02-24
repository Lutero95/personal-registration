# Personal Registration - Multicontainer Application

This project is a multicontainer Go-based application for personal registration, using Docker and PostgreSQL.

## Project Structure

- `.docker/`: Contains the Dockerfile and the docker-compose.
- `.env`: contains the environment variables.
- `main.go`: Entry point for the Go application.
- `src/`: Source code for the application, including database connection and logic.

3. **API Routes**:

   Use Postman, Insomnia, or another similar tool to access the following API routes:

   - **GET** - Retrieve a person by ID:
     ```http
     GET http://64.227.98.132:8000/api/person/{id_registro}
     ```

   - **POST** - Create a new person:
     ```http
     POST http://64.227.98.132:8000/api/person
     ```

   - **PUT** - Update an existing person by ID:
     ```http
     PUT http://64.227.98.132:8000/api/person/{id_registro}
     ```

   - **GET** - Retrieve a person by ID (confirmation):
     ```http
     GET http://64.227.98.132:8000/api/person/{id_registro}
     ```

   For the POST and PUT routes, use the following JSON format:

   ```json
   {
     "name": "Steve Rogers",
     "cpf": "17213777084",
     "sex": "M",
     "password": "12345678"
   }
   ```

