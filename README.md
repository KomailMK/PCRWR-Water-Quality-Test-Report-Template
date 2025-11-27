# PCRWR Water Quality Test Report Template

This project is a pixel-perfect HTML & CSS replication of the official **Pakistan Council of Research in Water Resources (PCRWR)** water quality test report.

It converts the original PDF design into a web-friendly format using **Tailwind CSS** and includes client-side **PDF generation** functionality using `html2pdf.js`.

## Features

* **Exact Replica:** Matches the fonts, spacing, tables, and layout of the official A4 report.
* **Print Ready:** CSS styled specifically for A4 paper size (210mm x 297mm).
* **Tailwind CSS:** Styled using utility classes via CDN for rapid development.
* **PDF Download:** Integrated `html2pdf.js` to download the exact HTML view as a PDF document.

##  Tech Stack

* **HTML5**
* **Tailwind CSS** (via CDN)
* **JavaScript**
* **Library:** [html2pdf.js](https://github.com/eKoopmans/html2pdf.js)

##  Important: How to Run (PDF Download Issue)

If you simply double-click `report.html` to open it in your browser (showing `file://` in the address bar), **the PDF download will fail or look broken.**

### Why?
Browsers block scripts from saving images to a PDF when running from the local file system due to security policies (CORS and "Tainted Canvas" issues).

###  The Solution
To make the "Download PDF" button work, you must run this project on a **local server** (localhost).

#### Method 1: VS Code (Recommended)
1.  Open the project folder in **Visual Studio Code**.
2.  Install the **"Live Server"** extension by Ritwick Dey.
3.  Right-click `report.html` and select **"Open with Live Server"**.
4.  The PDF download will now work perfectly.

#### Method 2: Python
If you have Python installed, open your terminal/command prompt in the project folder and run:

```bash
# Python 3.x
python -m http.server
```

#### Method 3: Python
If you have Node.js installed:

```bash
npx http-server
```