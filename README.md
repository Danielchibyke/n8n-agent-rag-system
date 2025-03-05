# n8n-agent-rag-system

Platform: n8n (you can import the .json file into your own n8n instance to check out the flow)

# Agent
This agent can go and load the youtube transcripts of videos, based on the URL. It then adds the transcripts into a vector store, creates a summary, key points, quotes and other information and stores it in a supabase DB. You then can chat about the videos. Ask for summaries, or follow up questions to sepecific videos. You can also search previously added videos. So, if you remember that a video was talking about a specific book, a specific tool, or a person, you can just ask the agent.

# Features
Add yt video transcripts to a Supabase vector store
Get summaries of the videos
Ask follow up questions to the videos
Search videos that have been previously been added
Dependencies
Claude Haiku
OpenAI Embedding Model
Supabase
Supadata
# Required configuration setup
Credentials for Youtube Data API (Used in the 'Fetch video details' node)
Credentials for https://supadata.ai to fetch the Transcript
Credentials for OpenAI (embeddings)
Credentials for Anthropic Claude
create the 'videos' table in Supabase via supabase.table.sql
Contributing
