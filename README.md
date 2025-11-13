Motivatinoal-Post-Genrator
Automatically pick a topic from a Google Sheet, create a post based on it, and upload the post to Google Drive.

🌟 Motivational AI Agent (n8n Workflow)
An automated AI agent built with n8n, designed to generate motivational posters using AI-generated images and inspirational quotes — and automatically upload them to Google Drive.

This workflow can run daily (or at any schedule) and stores all generated image links inside a Google Sheet for tracking and sharing.

🧠 Overview
The Motivational AI Agent is a fully automated workflow that:

Fetches a random motivational quote.
Builds a creative prompt for poster generation.
Uses an AI image generator (like Pollinations or Gemini API) to create a poster image.
Uploads the image to Google Drive.
Saves the image link back to a Google Sheet.
Repeats this process automatically based on your defined schedule.
🧩 Workflow Structure
Step	Node Name	Description
1	Schedule Trigger	Runs automatically (daily, hourly, etc.)
2	Get Random Quote	Reads a random quote from a Google Sheet
3	Pick Random Quote	Selects one random quote from the sheet
4	Build Poster Prompt	Creates an AI image prompt using the quote and author
5	Generate Image (Pollinations)	Generates the motivational poster using AI
6	Upload to Google Drive	Uploads the generated image file
7	Build Drive Link	Creates a shareable link for the uploaded file
8	Save Image Link to Sheet	Appends the image link and quote details to the sheet
9	End	Workflow completes successfully
⚙️ Technologies Used
n8n – Automation platform
Google Sheets – For storing and retrieving quotes
Google Drive – For uploading and hosting generated posters
Pollinations API (or Gemini API) – For AI image generation
JavaScript (Code Nodes) – For prompt building and logic
🚀 How It Works (Step-by-Step)
1. Schedule Trigger
Set up a schedule (e.g., every morning at 9:00 AM) to start the workflow automatically.

2. Get Random Quote
Reads all available quotes from your Google Sheet.
Example Sheet Format:

Quote	Author
"Believe you can and you're halfway there."	Theodore Roosevelt
"Dream big and dare to fail."	Norman Vaughan
3. Pick Random Quote
Randomly selects one quote entry from the sheet.

4. Build Poster Prompt
Builds an AI prompt like:
