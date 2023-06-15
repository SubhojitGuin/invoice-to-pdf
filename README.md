# Invoice Conversion to PDF

This Python script, `main.py`, converts Excel invoice files to PDF format using the `fpdf` library. It iterates through a list of Excel file paths in the `invoices` directory and generates a PDF file for each invoice.

## Features

- Converts Excel invoice files to PDF format.
- Extracts the invoice number and date from the file name.
- Adds the invoice number and date as a header in the PDF.
- Reads the invoice data from the Excel file and adds it to a table in the PDF.
- Calculates and displays the total price at the end of the table.
- Adds the company name and logo to the PDF.
- Saves the generated PDF files in the `PDFs` directory.

## File Structure

- `main.py`: This script contains the main code for converting Excel invoices to PDFs.
- `invoices/`: This directory contains the input Excel invoice files.
- `PDFs/`: This directory stores the generated PDF files.
- `sg-logo-design-initial-sg-letter-logo-icon-design-pro-free-vector.jpg`: The company logo image file.

## Usage

1. Place the Excel invoice files in the `invoices` directory.
2. Run the `main.py` script using Python: `python main.py`.
3. The script will convert each Excel invoice file to a PDF and save it in the `PDFs` directory.
4. The generated PDF files will have the same name as the input Excel files.

## Requirements

The project requires the following dependencies:

- fpdf==1.7.2
- pandas==1.3.3
- openpyxl==3.0.9

You can install the required dependencies by running `pip install -r requirements.txt`.

## Customization

You can customize the script by modifying the following:

- Input Directory: Change the directory path in the `glob.glob()` function to specify the directory where the Excel invoice files are located.
- Output Directory: Modify the `PDFs/` directory path in the `pdf.output()` function to specify the directory where the generated PDF files should be saved.
- Logo: Replace the `sg-logo-design-initial-sg-letter-logo-icon-design-pro-free-vector.jpg` file with your company logo file.
- Styling: Modify the font, color, and layout settings to customize the appearance of the PDF output.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Acknowledgements

- [fpdf](https://github.com/reingart/pyfpdf): A Python library for PDF document generation.

Feel free to customize the above template to include specific details about your invoice conversion project, such as additional features, instructions, or any other relevant information.