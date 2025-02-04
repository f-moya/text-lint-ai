# TextLintAI

## ✨ Features
 - 🖊 Side-by-side editor: Original text on the left, ChatGPT-suggested version on the right.
 - 🎨 Git diff-style changes:
   - Red underlines → deletions.
   - Green underlines → additions.
 - ⚡ Live updates: As you type, AI suggestions update in real time.
 - 🔍 Change explanations: AI provides context on why changes were made.
 - 🔑 Bring your own API key: Users provide their own OpenAI API key for privacy.
 - 📎 Context-aware editing: Optionally provide extra text or files for better AI suggestions.
 - 📋 Quick copy-paste: Easily copy improved text and iterate for multiple revision rounds.

## 🏗 Tech Stack
 - Frontend: Remix, Tailwind CSS
 - Backend: Rust (for local server)
 - Diff Computation: diff-match-patch (or another JS diff library)
 - AI Integration: OpenAI GPT API


## 🛠 Setup (Local Development)

 1. Clone the repo
  ```sh
  git clone https://github.com/your-username/grammardiff.git
  cd grammardiff
  ```
 2.	Install dependencies
  ```sh
  npm install  # or yarn install
  ```

 3. Run the server
  ```sh
  npm run dev
  ```
 4. Provide your OpenAI API key
    - Set it in an .env file:
      ```sh
      OPENAI_API_KEY=your-api-key-here
      ```
    - Or manually enter it in the UI.

 5. Open localhost:3000 in your browser and start writing!


## 🌎 Deployment

Initially, the project will be local-first. Once stable, it can be deployed on:
- Fly.io – Free-tier hosting with easy deployment
- Heroku – Simple for quick testing
- Vercel – For Remix apps with frontend-first logic 


## 🔒 Privacy & Security

GrammarDiff is fully open-source, ensuring transparency. Users store their own API keys locally, meaning we do not collect or store any tokens or writing data.

For API key security:
- Environment variable storage (.env) is recommended.
- Local storage encryption (e.g., Wyeworks prex-card) could be used.
- Open-source transparency: Users can verify that their API key is only used for their own requests.

## 🎯 Roadmap
- [ ] MVP: Local-first grammar checking
- [ ] Git diff-style visualization
- [ ] Customizable AI prompts
- [ ] File upload for context-aware editing
- [ ] User settings & API key management
- [ ] Cloud-hosted version (optional)

## 🤝 Contributing

We welcome contributions! If you want to help:
 1.	Fork the repository
 2.	Create a feature branch (git checkout -b feature-name)
 3.	Commit your changes (git commit -m "Add feature")
 4.	Push to your fork (git push origin feature-name)
 5.	Submit a pull request 🎉


## 📝 License

This project is licensed under the MIT License, making it open for everyone to use and contribute to.
