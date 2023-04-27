# How it works

This project makes use of the Vercel Edge streaming capabilities and the OpenAI GPT-3 API (more precisely, text-davinci-003). Based on the form and user input, it creates 5 movie recommendations. It then sends the request via a Vercel Edge function to the GPT-3 API, receives a response, and feeds it back to the application.

# Running Locally

After cloning the repo, go to OpenAI to make an account and put your API key in a file called `.env`.

For example:

`OPENAI_API_KEY=...`
`OMDB_API_KEY=...`

Then, run the application in the command line and it will be available at http://localhost:5173.

`npm run dev`
