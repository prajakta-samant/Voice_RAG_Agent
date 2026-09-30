# End-to-End Voice RAG Agent
Voice AI Agent that combines n8n, ElevenLabs, OpenAI, and Supabase to build a Retrieval-Augmented Generation (RAG) voice assistant that retrieves relevant information from a vector database and responds naturally through voice.

Voice agent Accept voice or chat queries , search a knowledge base using semantic search , generate context-aware responses and reply naturally through a conversational interface

How the workflow works:

Step1: The user sends a voice or chat request through ElevenLabs.
Step 2: ElevenLabs forwards the request through a webhook.
Step3: n8n receives the request and passes it to the AI Agent. The AI Agent searches the Supabase Vector Store for relevant information.
Step4: The retrieved context is sent to the OpenAI model. The model generates an accurate response.
Step5: The response is returned through the webhook back to the user.
