# Alteryx SDK QR Code Generator

Custom Alteryx SDK tool that generates QR codes from input data.

## Installation
Download the yxi file and double click to install in Alteyrx. 

<img src="https://github.com/bobpeers/Alteryx_SDK_QR_Code_Generator/blob/main/images/qr_install.png" width="600" alt="QR Codes Install Dialog">

The tool will be installed in the __Developer__ category.

<img src="https://github.com/bobpeers/Alteryx_SDK_QR_Code_Generator/blob/main/images/qr_toolbar.png" width="600" alt="QR Codes Install Toolbar">

## Requirements

The tool will install the Python libary called [segno](https://segno.readthedocs.io/en/latest/)

## Usage
The tool con be configured for:

- Source field is the field to encode as a QR code.
- Scale, this changes the size of the QR codes 1 is small, 10 is large. I suggest you experiment to get the required size.
- QR codes colour. This the the colour of the main barcode pattern.
- Transpartent background. Check for transparent or uncheck to pick a custom colour.

## Outputs
The tool outputs a base 64 encoded image field. This can be fed through a Blob Convert tool using the Base 64 to binary option.

<img src="https://github.com/bobpeers/Alteryx_SDK_QR_Code_Generator/blob/main/images/blob_convert.png" width="600" alt="QR Codes workflow">

## Usage
This workflow demonstrates the tool in use. The workflow shown here:

<img src="https://github.com/bobpeers/Alteryx_SDK_QR_Code_Generator/blob/main/images/qr_workflow.png" width="1000" alt="QR Codes workflow">

The output can be visualized using a Browse tool as shown here.

<img src="https://github.com/bobpeers/Alteryx_SDK_QR_Code_Generator/blob/main/images/qr_output.png" width="600" alt="QR Codes output">
