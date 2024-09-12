This documentation presents the development, deployment, and evaluation of KIRIKOU: AI
Assistant for KNUST IDL, a chatbot designed to automate inquiries and enhance user
interaction on the KNUST Institute of Distance Learning (IDL) website. Leveraging
cutting-edge technologies, including OpenAI GPT-3.5, Upstash Vector, Upstash Redis,
Langchain.js, and Next.js, KIRIKOU provides real-time responses to user queries,
streamlining access to academic information.
The project follows a Retrieval-Augmented Generation (RAG) approach, where a custom
Scrapy web crawler collects and vectorizes content from the KNUST IDL website, making it
accessible for KIRIKOU to retrieve and generate contextually accurate answers. The system
is deployed on Vercel, ensuring scalability and high availability for handling multiple
concurrent user requests.
This documentation outlines the entire lifecycle of KIRIKOU, from inception to real-world
testing, covering system architecture, key components, and performance metrics. Rigorous
testing confirmed that KIRIKOU meets its objectives in terms of speed, accuracy, scalability,
and reliability, achieving an average response time of 1.2 seconds and 98% query accuracy
for domain-specific queries. This chatbot effectively reduces the workload on administrative
staff and provides a user-friendly, efficient solution for current students, prospective
applicants, and staff at KNUST IDL
