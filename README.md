# A docker container for OCRmyPDF

This is a docker container for
[OCRmyPDF](https://github.com/fritz-hh/OCRmyPDF).

## Installation

```bash
docker pull paulstaab/ocrmypdf
```

## Usage

To ocr a pdf, call

```bash
docker run -t -i -v "</path/to/pdf>:/home/docker/" paulstaab/ocrmypdf \
  OCRmyPDF <additional options> <pdf> <out.pdf>
```

where 

 - `</path/to/pdf>` is a placeholder for the absolute path to the pdf,
 - `<pdf>` is the name of the pdf file (without it's path),
 - `<out.pdf>` is the file to which the ocred document will be written and
 - `<additional options>` are optional parameters for OCRmyPDF 
   (see `docker run -t -i paulstaab/ocrmypdf OCRmyPDF -h`)  

