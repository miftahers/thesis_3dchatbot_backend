# 3D Character Chatbot

This project is an Express.js application integrated with Google Cloud's Vertex AI to provide a chatbot service. It includes a POST endpoint (`/chat`) that interacts with the Vertex AI model to generate responses based on user input.

## Prerequisites

-   Node.js (>=14.0.0)
-   npm (Node Package Manager)
-   Google Cloud Project with Vertex AI enabled
-   API Key for Vertex AI

## Setup

### 1. Clone the Repository

```bash
git clone https://github.com/miftahers/3DCharChatbot
cd 3DCharchatbot
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory of the project and add the following environment variables:

```
PORT=8080
GCP_PROJECT=your_google_cloud_project_id
GCP_LOCATION=your_google_cloud_location
GEMINI_API_KEY=your_gemini_ai_api_key
```

Replace the placeholder values with your actual Vertex AI API key, Google Cloud project ID, and location.

### 4. Start the Server

Run the following command to start the server:

```bash
npm start
```

The server will be running at `http://localhost:8080`.

### 5. Testing the Endpoint

You can test the `/chat` endpoint using tools like Postman or `curl`. For example, to test using `curl`, use the following command:

```bash
curl -X POST http://localhost:8080/chat -H "Content-Type: application/json" -d '{"message": "Berikan motivasi"}'
```

### 6. Static Files

Static files can be served from the `public` directory. Place your static assets (e.g., HTML, CSS, JavaScript files) in the `public` directory.

## Error Handling

In case of errors while communicating with Vertex AI, the server will respond with a `500` status code and an error message. Check the server logs for detailed error information.

## Additional Configuration

Feel free to modify the `server.js` file to adjust the Vertex AI configuration or add additional features.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

-   [Google Cloud Vertex AI Documentation](https://cloud.google.com/vertex-ai/docs)
-   [Express.js Documentation](https://expressjs.com/)

### Notes:

-   **Replace** `your-username`, `your_vertex_ai_api_key`, `your_google_cloud_project_id`, and `your_google_cloud_location` with your actual details.
-   **Update** the repository URL if you have a different one.
-   **Add** any additional sections or configurations as needed for your project.

Feel free to modify or extend this template to better fit your project!
