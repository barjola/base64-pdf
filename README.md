# Base64 to PDF Viewer

This is a simple web-based tool that allows you to visualize and download PDF files from Base64-encoded strings or JSON objects containing a `base64File` attribute.

You can try it directly online here:  
https://barjola.github.io/base64-pdf/

## Features

- Paste a Base64 string or a JSON object containing a `base64File` field.
- Automatically decodes and displays the PDF in an embedded viewer.
- Allows you to download the PDF file with a custom filename.
- Saves the sidebar width in local storage.
- Resizable sidebar.
- Auto-selects the input text when clicked.

## Usage

1. Open the [online version](https://barjola.github.io/base64-pdf/) or run the HTML file locally in any modern web browser.
2. Paste your Base64 string or JSON containing a `base64File` field into the text area.
3. The PDF will render automatically in the viewer pane.
4. Optionally, enter a file name in the input box (defaults to `download.pdf`).
5. Click the **⬇ Download PDF** button to save the file.

## Input Formats

- Direct Base64-encoded PDF:
  ```
  JVBERi0xLjQKJc...
  ```

- Base64 with data URI:
  ```
  data:application/pdf;base64,JVBERi0xLjQKJc...
  ```

- JSON format:
  ```json
  {
    "document": {
      "base64File": "JVBERi0xLjQKJc..."
    }
  }
  ```

The viewer will automatically extract and decode the Base64 string.

## Requirements

No external dependencies. Just open the HTML file in your browser or use the online link.

## License

This project is released under the MIT License.
