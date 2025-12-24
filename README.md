# Spring Boot Gemini AI Integration

This project demonstrates how to integrate **Google Gemini AI** into a **Spring Boot** application using **Spring AI**.  
It exposes a REST API that accepts a user prompt and returns an AI-generated response from Gemini.

This project is intended for learning and demonstration purposes and follows clean backend design principles.

---

## 🚀 Features

- Spring Boot REST API
- Google Gemini AI integration using Spring AI
- Prompt-based AI responses
- Swagger UI for API testing
- Externalized configuration for API keys
- Clean separation of Controller and Service layers

---

## 🛠️ Tech Stack

- Java 21
- Spring Boot
- Spring AI
- Google Gemini (GenAI)
- Maven
- Swagger / OpenAPI

---

## 🔐 Setting Gemini API Key in IntelliJ IDEA

To keep the API key secure, configure it as an environment variable in IntelliJ instead of hardcoding it.

### Steps

1. Open **Run → Edit Configurations**
2. Select your Spring Boot application (e.g., `SpringGeminiAiApplication`)
3. Locate **Environment variables**
4. Click the **Edit (📁) icon**
5. Add a new variable:
   GEMINI_API_KEY=<your_gemini_api_key>
6. Click **OK → Apply**
7. Restart the application

The application will automatically read the API key using:
```yaml
spring.ai.google.genai.api-key: ${GEMINI_API_KEY}
