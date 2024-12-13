# KIRIKOU: AI Assistant for KNUST IDL

KIRIKOU is an advanced AI-powered chatbot designed to automate inquiries and enhance user interactions on the Kwame Nkrumah University of Science and Technology (KNUST) Institute of Distance Learning (IDL) website. Leveraging cutting-edge technologies and a Retrieval-Augmented Generation (RAG) approach, KIRIKOU streamlines access to academic information, reduces the workload on administrative staff, and provides an efficient solution for students, prospective applicants, and staff.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [System Architecture](#system-architecture)
- [Technologies Used](#technologies-used)
- [Deployment](#deployment)
- [Performance Metrics](#performance-metrics)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

KIRIKOU utilizes state-of-the-art technologies to deliver real-time, contextually accurate responses to user queries. Built on OpenAI's GPT-3.5, the chatbot is designed to fetch and generate precise answers using content sourced from the KNUST IDL website. The system ensures:

- Fast and accurate query resolution
- Scalability to handle multiple concurrent users
- User-friendly interaction for all stakeholders

## Features

- **Real-Time Responses**: Provides accurate and prompt answers to user queries.
- **RAG Framework**: Combines retrieval and generative AI for improved contextual accuracy.
- **Web Crawling and Indexing**: Custom Scrapy crawler collects and vectorizes website content.
- **Scalable Deployment**: Hosted on Vercel for high availability and efficient scaling.
- **Domain-Specific Accuracy**: Achieves 98% accuracy for KNUST IDL-related queries.
- **User-Centric Design**: Simplifies access to information for students, staff, and prospective applicants.

## System Architecture

The architecture of KIRIKOU is designed for efficiency and scalability:

1. **Web Crawler**:
   - Scrapy crawler collects content from the KNUST IDL website.
   - Content is vectorized using Upstash Vector and stored in Upstash Redis for quick retrieval.

2. **Query Processing**:
   - User queries are processed through LangChain.js.
   - Relevant information is retrieved and passed to OpenAI GPT-3.5 for response generation.

3. **Deployment**:
   - Hosted on Vercel for seamless deployment and high availability.

![Architecture Diagram](#) *(Add a system architecture diagram if available)*

## Technologies Used

- **Backend**:
  - OpenAI GPT-3.5
  - LangChain.js
  - Upstash Redis
  - Upstash Vector

- **Frontend**:
  - Next.js

- **Tools**:
  - Scrapy (Web Crawling)
  - Vercel (Deployment)

## Deployment

KIRIKOU is deployed on [Vercel](https://vercel.com), ensuring:

- High availability for handling multiple user requests
- Automatic scaling to match demand

## Performance Metrics

- **Response Time**: Average of 1.2 seconds per query
- **Query Accuracy**: 98% for domain-specific questions
- **Scalability**: Handles multiple concurrent user requests efficiently

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- Vercel account
- Access to OpenAI API keys

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/gotinkorang/idlchat.git
   cd idlchat
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Configure environment variables:
   - Create a `.env` file in the root directory.
   - Add the following variables:
     ```env
     OPENAI_API_KEY=your_openai_api_key
     UPSTASH_REDIS_URL=your_upstash_redis_url
     VERSTEL_PROJECT_URL=your_vercel_project_url
     ```

4. Start the development server:
   ```bash
   npm run dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) to view the application.

## Usage

1. Visit the deployed application on the provided Vercel URL.
2. Enter your query into the chatbot interface.
3. Receive instant, accurate responses tailored to KNUST IDL information.

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request on GitHub.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute this project as per the terms of the license.

---

## Contact

For more information or support, please contact:

- **Author**: Gershon Adjei Otinkorang
- **Email**: [contact@gershon.one)](mailto:contact@gershon.one)
- **GitHub**: [gotinkorang](https://github.com/gotinkorang)

---

Thank you for exploring KIRIKOU! We hope this project inspires and streamlines academic interactions at KNUST IDL.
