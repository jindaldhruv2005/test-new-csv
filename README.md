# Hello World + CSV Viewer

## Overview
This is a minimal web app that:
- Displays the text “Hello World”.
- Loads and displays the contents of sample.csv as an HTML table on the home page.
- Includes a built-in fallback copy of the CSV so the table still renders if the browser blocks fetching local files when opened via file://.

License: MIT

## Setup
You can open index.html directly, but for consistent CSV loading it’s best to serve it via a local web server (browsers often block fetches from file://).

- Python 3:
  - macOS/Linux: python3 -m http.server 8000
  - Windows: py -3 -m http.server 8000
- Node.js (optional alternative):
  - npx http-server -p 8000

Then visit: http://localhost:8000/

Place sample.csv in the same directory as index.html (it already is, if you use the provided repository layout).

## Usage
- Open the app in your browser.
- You’ll see “Hello World” and a “Sales Data (sample.csv)” section rendering the CSV as an HTML table.
- If served via HTTP, the app fetches sample.csv directly.
- If opened via file:// and the browser blocks fetch, the app automatically uses the embedded fallback copy to display the data.

## License (MIT)
Copyright (c) 2025 Example Author

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.