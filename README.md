# 🏛️ AI Legal Document Simplifier

An intelligent web application designed to make complex legal documents understandable for the common person. This tool leverages the power of Google's Gemini API to analyze, summarize, and provide actionable insights for documents like FIRs, rental agreements, and legal notices in both English and Hindi.

---

## The Problem

Legal documents are often filled with dense jargon and complex structures, making them intimidating and inaccessible to people without a legal background. This information gap can be a significant barrier to understanding one's own rights and responsibilities, preventing individuals from taking necessary and timely action.

## The Solution

This AI-powered tool acts as a bridge, transforming confusing legal text into clear, structured, and actionable information. It's not designed for lawyers, but for everyone else—students, tenants, consumers, and any citizen who needs to quickly understand a document that affects them. The application provides a multi-faceted analysis in a clean, tabbed interface, moving the user from confusion to empowered action.

---

## Features

-   **Multi-Format Document Upload:** Securely upload `.pdf` and `.txt` files directly in the browser. Text extraction from PDFs is handled client-side using `pdf.js`.
-   **Full Multilingual Support:** Get a complete analysis in either **Simple English** or **Hindi**, including all labels and summaries.
-   **Dual-Mode Summary:**
    -   **Key Info:** A quick overview that extracts the most critical data points (names, dates, locations, laws) into a clean key-value format.
    -   **Detailed Summary:** A comprehensive narrative summary with clear headings and bullet points for a deeper understanding of the document's content.
-   **Action-Oriented Insights (Tabbed Interface):**
    -   **Rights & Obligations:** Automatically identifies and separates what the document entitles you to (your rights) and what it requires you to do (your responsibilities).
    -   **Next Steps:** Provides a simple, actionable checklist of what a common person should do next after receiving the document.
    -   **Authority Finder:** Identifies and provides contact information for the relevant local authorities (e.g., police station, consumer court) mentioned or implied in the document.
-   **Privacy-Focused:** The original document file is never uploaded to a server. Only the extracted text is sent to the Gemini API for analysis, and the data is not used for training, as per Google's API terms of service.
-   **Consistent & Reliable:** The AI's creativity (`temperature`) is set to 0 to ensure you get the most factual and consistent analysis every time you upload the same document.

---

## Tech Stack

-   **Frontend:** HTML5, CSS3, Vanilla JavaScript
-   **Styling:** Bootstrap 5
-   **AI & NLP:** Google Gemini API
-   **Client-Side Libraries:**
    -   `pdf.js` for in-browser PDF text extraction.
    -   `marked.js` for rendering Markdown responses from the AI.

---

## How to Use

To run this project locally, follow these steps:

1.  **Clone the repository**
    

2.  **Create the project files**
    

3.  **Get your API Key:**
    -   Visit the [Google AI Studio](https://aistudio.google.com/app/apikey) to get your free Gemini API key.

4.  **Run the Application:**
    -   Open the `index.html` file in your web browser.
    -   Paste your API key into the designated input field.
    -   Upload a document, select your desired analysis type and language, and click "Analyze".

---

## Acknowledgements

This project was made possible by these incredible tools and services:
-   [Google Gemini API](https://ai.google.dev/) for the powerful language model.
-   [Bootstrap](https://getbootstrap.com/) for the responsive UI framework.
-   [PDF.js](https://mozilla.github.io/pdf.js/) by Mozilla for client-side PDF processing.
-   [Marked.js](https://marked.js.org/) for Markdown rendering.
