# Node-RED ChatGPT POC

## Project Description

This project is a Proof of Concept (PoC) demonstrating the integration of ChatGPT with Node-RED. It showcases how Node-RED can be used to create a web interface that accepts user input, processes any links provided by the user, fetches and parses the content of those web pages, and enriches the context sent to ChatGPT to generate more informative and relevant responses.

## Getting Started

### Prerequisites

- Docker
- Docker Compose

### Installation

1. Clone the repository:

```bash
git clone https://github.com/EllGree/node-red-chatgpt-poc.git
cd node-red-chatgpt-poc
```
   
2. Run the Docker container:

```bash
docker-compose up -d
```

3. Access Node-RED:

Open your web browser and navigate to http://localhost:1880/ to access the Node-RED interface.

4. Access the User Input Form:

Navigate to http://localhost:1880/message to access the user input form.

## Usage

- **Submit a Message**: enter your message in the input form and submit it, if your message contains any links, the system will automatically fetch and parse the content from those web pages.

- **Context Enrichment**: the system extracts information such as the title, description, and main headings from each linked web page and adds this information to your input as a system message.

- **ChatGPT Response**: the enriched input is then sent to the OpenAI ChatGPT API to generate a response, which will be displayed to you with improved context and relevance.

## License

This project is licensed under the MIT License.
