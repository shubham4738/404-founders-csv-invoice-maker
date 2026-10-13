<img width="937" height="471" alt="image" src="https://github.com/user-attachments/assets/256b2354-c50b-41d9-afba-62616cf7e000" />Readme template · MD
# CSV Data Cleaner and Invoice Maker 
 
## Team Name
[404 FOUNDERS]
 
## Team Members
1. [SHUBHAM GAUR] — [Full Stack & Invoice Maker]
2. [ABHISHEK SHARMA] — [Github Repo, Testing & CSV Handling]
3. [HANNAN MEHBOOB] — [Frontend UI & Validation Logic]
4. [NAVEEN CHAND] — [Documentation,Presentation & Quality Assurance]
## Selected Problem Statement
[CSV Data Cleaner and Invoice Maker]
 
## Problem Description
Small offices frequently receive customer order batches via manual spreadsheets or CSV files that contain human entry errors—such as missing customer names, blank item descriptions, negative prices, invalid or decimal quantities, and duplicate order entries. Generating invoices directly from corrupted datasets leads to erroneous billing, accounting mismatches, and financial discrepancy. Therefore, an automated system is required to sanitize and validate order data before creating duplicate-protected, print-ready invoices.

## Proposed Solution
CSV Data Cleaner and Invoice Maker is an interactive web-based utility designed for small office operations to import raw sales order CSV files, automatically detect data irregularities in real time, and provide inline editing and deletion capabilities. Once the dataset is cleaned and validated, the application generates professional, duplicate-protected, and print-ready tax invoices while strictly preventing invalid rows from being billed.

## Key Features
- **CSV Import & Test Template:** Easily upload and parse customer order CSV files with a single click, plus a built-in "Download Sample CSV" option pre-loaded with valid and test error rows.
- **Real-Time Data Validation:** Automatically checks imported data line-by-line and highlights:
  - Missing customer names or missing item descriptions.
  - Invalid quantities (must be an integer strictly greater than zero).
  - Invalid prices (flags negative prices; price must be ≥ 0).
  - Repeated/duplicate rows within the dataset.
- **Interactive Inline Data Cleaning:** Allows users to edit incorrect values directly inside table cells or delete unrecoverable rows before billing.
- **Automated Amount Calculation:** Dynamically calculates `Final Amount = Quantity × Price per Item` inside the application without requiring manual user computation.
- **Invoice Creation & Printing:** Generates sequential, dedicated invoices only from validated ("OK") rows, complete with a clean printable tax invoice format.
- **Strict Duplicate Protection:** Re-importing the same CSV or repeat order entries will not generate duplicate invoices for previously billed orders.
 
## Technology Stack
- **Frontend:** HTML5, CSS3, Modern JavaScript (ES6+)
- **File Processing:** Browser Native `FileReader` API & Dynamic `Blob` URLs
- **Version Control & Hosting:** Git, GitHub
- **Hosting:** Localhost (https://404-founders-csv-invoice-maker.vercel.app/)

## Why This Tech Stack?
We chose native HTML, CSS, and modern JavaScript because it requires zero build steps, external npm libraries, or complex server configurations. This enabled our team to build, thoroughly test, and deliver a zero-latency, crash-free client-side prototype well within the 6.5-hour hackathon timeframe.

## Setup & Installation Instructions
1. Clone the repository:
```bash
git clone [https://github.com/shubham4738/404-founders-csv-invoice-maker.git](https://github.com/shubham4738/404-founders-csv-invoice-maker.git)
 
2. Navigate into the project folder:
```
cd 404-founders-csv-invoice-maker
 
## Required Environment Variables / Configuration
No environment variables, API keys, or `.env` configuration files are required for this project[span_2](start_span)[span_2](end_span). All validations, calculations, and invoice operations run entirely client-side within the browser[span_3](start_span)[span_3](end_span).

## Database Setup
- No external database (such as Firebase, MySQL, or MongoDB) is required[span_1](start_span)[span_1](end_span)[span_2](start_span)[span_2](end_span).
- All parsed CSV rows, validation errors, and generated invoice records are managed directly in-memory within the browser session and local state for instant processing[span_3](start_span)[span_3](end_span)[span_4](start_span)[span_4](end_span).

## How to Run the Project
1. Direct Browser Execution: Double-click the `index.html` file in your project folder to open and run it instantly in any web browser (Chrome, Edge, Firefox)[span_5](start_span)[span_5](end_span).
2. Via Local Server: If using VS Code, open the project folder, right-click on `index.html`, and select **"Open with Live Server"** (or run `npx live-server` in the terminal at `http://127.0.0.1:5500`)[span_6](start_span)[span_6](end_span)[span_7](start_span)[span_7](end_span).

## Screenshots
<img width="929" height="440" alt="Screenshot 2026-10-13 142226" src="https://github.com/user-attachments/assets/a2647be0-8136-4bd8-962b-34e4a1910fe9" />
<img width="939" height="466" alt="Screenshot 2026-10-13 142257" src="https://github.com/user-attachments/assets/c20b8a8f-1376-4068-b722-4b52f1552e78" />
<img width="937" height="471" alt="Screenshot 2026-10-13 142522" src="https://github.com/user-attachments/assets/d158771f-c9a1-409b-b249-b8bc6dc50fee" />
<img width="940" height="467" alt="Screenshot 2026-10-13 142323" src="https://github.com/user-attachments/assets/2fa72110-c658-4802-b700-e3f30e259d2a" />
<img width="814" height="458" alt="Screenshot 2026-10-13 142343" src="https://github.com/user-attachments/assets/5086e27a-1a96-48bd-919e-01ecaac0d6d3" />


## Known Limitations
- Operates primarily client-side in the browser session without persistent cloud database synchronization.
- Designed for single-line-item order rows per entry rather than complex multi-product bundled carts.
- In-memory processing means clearing browser cache or resetting clears local temporary state.

## Future Scope
- Backend integration (Node.js/Express + PostgreSQL or MongoDB) for cloud storage and multi-user role authentication.
- Direct one-click PDF invoice export and automated email delivery to clients.
- Multi-currency conversion support and advanced search/filtering across historical invoice archives.

## Live Demo Link
[https://404-founders-csv-invoice-maker.vercel.app/](https://404-founders-csv-invoice-maker.vercel.app/)

## Repository Link
https://github.com/shubham4738/404-founders-csv-invoice-maker
