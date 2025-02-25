This playbook extracts indicators from a file.
Supported file types:
- CSV
- PDF
- TXT
- HTM, HTML
- DOC, DOCX
- PPT
- PPTX
- RTF
- XLS
- XLSX
- XML

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
This playbook does not use any integrations.

### Scripts
* ExtractIndicatorsFromWordFile
* ExtractIndicatorsFromTextFile
* ConvertFile
* Set
* ReadPDFFileV2

### Commands
* image-ocr-extract-text
* rasterize-pdf

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Required** |
| --- | --- | --- | --- |
| File | The file from which to extract indicators. | File.None | Optional |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Domain.Name | The extracted domains. | string |
| Account.Email.Address | The extracted email addresses. | string |
| File.MD5 | The extracted MD5 hash. | string |
| File.SHA1 | The extracted SHA1 hash. | string |
| File.SHA256 | The extracted SHA256 hash. | string |
| IP.Address | The extracted IP addresses. | string |
| File.Text | The text or images extracted from the PDF file. | string |
| File.Producer | The PDF file producer. | string |
| File.Title | The title of the PDF file. | string |
| File.xap | The XAP of the PDF file. | string |
| File.Author | The author of the file. | string |
| File.dc | The DC of the file. | string |
| File.xapmm | The XAPMM of the file. | string |
| File.ModDate | The mod date of the file. | string |
| File.CreationDate | The creation date of the file. | string |
| File.Pages | The number of pages in the file. | string |
| URL.Data | A list of URLs that were extracted from the file. | string |

## Playbook Image
---
![Extract Indicators From File - Generic v2](https://raw.githubusercontent.com/demisto/content/master/Packs/CommonPlaybooks/doc_files/Extract_Indicators_From_File_-_Generic_v2.png)