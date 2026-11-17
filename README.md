# Resume Auto-Renamer

A fast, zero-dependency, client-side web utility that automatically renames uploaded resume files to the format `Chirag_Dhunna_{DD_MM_YYYY}.{ext}` and triggers an instant download. Built as a single HTML file for effortless deployment on Vercel.

## Features

- **Automatic Date Stamping:** Detects the current date and formats the file name as `Chirag_Dhunna_DD_MM_YYYY` while keeping the original file extension (`.pdf`, `.docx`, `.doc`, etc.).
- **100% Client-Side Privacy:** Uses the browser's native `Blob` and `URL.createObjectURL` APIs. Your resume never leaves your device or gets uploaded to any external server.
- **Drag & Drop Support:** Drop your file anywhere on the upload zone for instant processing and auto-download.
- **Customizable Output:** Toggle auto-download off to manually tweak the name prefix or select a custom date before downloading.
- **Zero Build Step:** Contained entirely within a single `index.html` file styled with Tailwind CSS (via CDN).

## Project Structure

```text
.
├── index.html   # Complete application (HTML, Tailwind CSS, Vanilla JS)
└── README.md    # Project documentation
```

## Getting Started Locally

1. Clone the repository:
   ```bash
   git clone [https://github.com/chiragdhunn/resume-renamer.git](https://github.com/chiragdhunn/resume-renamer.git)
   cd resume-renamer
   ```

2. Open `index.html` directly in any browser, or serve it locally:
   ```bash
   npx serve .
   ```

## Deploying to Vercel

### Option 1: Vercel CLI
1. Install the Vercel CLI if you haven't already:
   ```bash
   npm i -g vercel
   ```
2. Run the deploy command from the project root:
   ```bash
   vercel --prod
   ```

### Option 2: GitHub Integration
1. Push this repository to your GitHub account.
2. Go to the [Vercel Dashboard](https://vercel.com/new) and import the repository.
3. Leave the **Framework Preset** as `Other` and the **Build Command** empty.
4. Click **Deploy**.

## Tech Stack

- **HTML5** (File API, Blob API, Drag and Drop API)
- **Tailwind CSS** (via CDN)
- **Vanilla JavaScript**

## License

This project is open-source and available under the [MIT License](LICENSE).
