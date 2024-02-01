# File Metadata Microservice

This microservice provides a simple file upload and analysis functionality. Users can upload a file, and the service will return basic metadata information about the uploaded file.

### Usage

1. Start the microservice:

   ```bash
   npm start
   ```

   The microservice will be running at [http://localhost:3000](http://localhost:3000).

2. Access the service in your web browser or use tools like Postman to interact with it.

3. Upload a file by sending a POST request to the `/api/fileanalyse` endpoint. Use the `upfile` field for file upload.

4. The microservice will respond with basic metadata information about the uploaded file in JSON format.

### Configuration

- The destination folder for file uploads is set to `uploads/`. You can customize this in the `storage` configuration of the Multer middleware.

### Endpoints

- `GET /`: Displays the main HTML page for file upload.
- `POST /api/fileanalyse`: Handles file upload and responds with basic file metadata.
