# 2026-05-10

# Jira Stories Test Case Generation Application with Ollama Model Integration
**Overview**
The Jira Stories Test Case Generation Application is a Spring Boot application designed to fetch user story details from Jira and generate test cases based on the acceptance criteria. It integrates with the Ollama AI model to process natural language inputs and automatically generate detailed test cases.

**Project Structure**
- **JiraInquiryController**:Handles HTTP requests for Jira story inquiries.
  - Utilizes the Ollama AI model to process acceptance criteria and generate relevant test cases.

- **JiraFunctionConfig**:
  - Configures and provides the JiraDataService bean.
  - Sets up the Jira function used by the AI model to fetch Jira story details and generate test cases.

- **JiraDataService:**
  - Manages communication with the Jira API to fetch user story details, including acceptance criteria.
  - Reads Jira API credentials and URL from configuration properties.
  - Parses the Jira API responses to extract relevant information.

- **JiraApiProperties**:
  - Stores Jira API credentials (username, API token) and the base URL.
  - Provides configuration properties for JiraDataService.
step).PrerequisitesBefore running this application, ensure you have the following installed:Java 17 or higherMaven 3.8+Ollama (Running locally with your preferred model, e.g., llama3 or mistral)A valid Jira API Token and site URL.
