# PDF Form Filler

A FastAPI-based application to fill given form with provided data and generate a new PDF file.

## Requirements

- Python 3.7+
- FastAPI
- Uvicorn
- python-docx
- docx2pdf


## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/muskan9191/pdf-form-filler.git
    cd pdf-form-filler
    ```

2. Install the required packages:

    ```bash
    pip install fastapi uvicorn python-docx docx2pdf
    ```

## Running the Application

To start the FastAPI server, run:

```bash
uvicorn main:app --reload
```

## Test Example

To test, update the below command values, open command prompt and run:

```bash
curl -X POST "http://127.0.0.1:8000/fill-form/" -F "name=Muskan Madhwani" -F "address=12\24 Karol Bagh" -F "date=22 Jul 2024" -F "favourite_activities=Reading,Walking,Dancing" -F "favourite_activity=Walking" -o filled_form.pdf
```

The output file will be stored in filled_form.pdf file