# 📓 Markdown Note-taking App

A simple 📝 note-taking app built with 🚀 Beyond, ⚛️ React, and 🟦 TypeScript that allows users to 📤 upload Markdown files, ✅ check the grammar, 💾 save notes, and 🖼️ render them as HTML. This project is designed to help developers 📚 learn how to handle 📁 file uploads in a 🌐 RESTful API, parse and render Markdown files using 📦 libraries, and perform 📝 grammar checks.

## 🌟 Features

### 🔑 Core Functionalities

1. **✅ Grammar Check Endpoint**
   - An API endpoint that 🧐 checks the grammar of the provided Markdown content.

2. **💾 Save Note Endpoint**
   - An API endpoint to 💾 save notes passed as Markdown text.

3. **📜 List Notes Endpoint**
   - An API endpoint to 📜 list all saved notes (i.e., uploaded Markdown files).

4. **🖼️ Rendered HTML Endpoint**
   - An API endpoint to return the 🖼️ HTML-rendered version of a Markdown note.

## 🛠️ Technologies Used

- **🚀 Beyond.js**: For building a 🧩 modular and 🌐 reactive app.
- **⚛️ React**: To create an 💻 interactive and 👥 user-friendly interface.
- **🟦 TypeScript**: Ensuring 🔒 type safety and 🏗️ robust code quality.

## 🚀 Getting Started

### 📋 Prerequisites

- 🌳 Node.js (version 16 or higher)
- 📦 npm or 🧶 yarn (for 📦 package management)
- ✍️ A code editor like 💡 VS Code

### 🔧 Installation

1. 🌀 Clone the repository:
   ```bash
   git clone https://github.com/your-repository/markdown-notes-app.git
   cd markdown-notes-app
   ```

2. 📦 Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. ▶️ Start the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. 🌐 Open the application in your browser at `http://localhost:3000`.

## 🔗 API Endpoints

### 1️⃣ ✅ Grammar Check
- **Endpoint**: `POST /api/grammar-check`
- **Description**: 🧐 Checks the grammar of the provided Markdown content.
- **Request Body**:
  ```json
  {
    "content": "# Sample Markdown\nThis is a sample text with grammor error."
  }
  ```
- **Response**:
  ```json
  {
    "errors": ["The word 'grammor' may be a typo."]
  }
  ```

### 2️⃣ 💾 Save Note
- **Endpoint**: `POST /api/save-note`
- **Description**: 💾 Saves a Markdown note.
- **Request Body**:
  ```json
  {
    "title": "Sample Note",
    "content": "# Markdown Title\nThis is the note content."
  }
  ```
- **Response**:
  ```json
  {
    "message": "Note saved successfully."
  }
  ```

### 3️⃣ 📜 List Notes
- **Endpoint**: `GET /api/list-notes`
- **Description**: 📜 Lists all saved notes.
- **Response**:
  ```json
  [
    {
      "id": "1",
      "title": "Sample Note",
      "created_at": "2024-12-21T10:00:00Z"
    }
  ]
  ```

### 4️⃣ 🖼️ Rendered HTML
- **Endpoint**: `GET /api/render-note/{id}`
- **Description**: Returns the 🖼️ HTML-rendered version of the Markdown note.
- **Response**:
  ```html
  <h1>Markdown Title</h1>
  <p>This is the note content.</p>
  ```

## 💡 Tips for Development

- Use a 📦 library like `marked` or `markdown-it` for 📄 parsing and 🖼️ rendering Markdown files.
- Implement a 📝 grammar-checking 📦 library or API such as Grammarly or `node-nlp`.
- Ensure proper ⚠️ error handling for 📁 file uploads and content validation.
- Use a 🗄️ database like SQLite, PostgreSQL, or Supabase for 📂 storing the notes.


## 🤝 Contributing

1. 🍴 Fork the repository.
2. 🆕 Create a feature branch: `git checkout -b feature-name`
3. 📝 Commit your changes: `git commit -m 'Add feature'`
4. 🚀 Push to the branch: `git push origin feature-name`
5. 📨 Open a pull request.

## 📜 License

This project is licensed under the 📄 MIT License. See the [LICENSE](LICENSE) file for details.

## 🙌 Acknowledgments

- [🚀 Beyond.js](https://beyondjs.com/)
- [⚛️ React](https://reactjs.org/)
- [📄 Marked](https://marked.js.org/) or [📄 Markdown-it](https://markdown-it.github.io/)
- [🟦 TypeScript](https://www.typescriptlang.org/)

