# Health Census

A simple browser-based health analysis application for recording patient information and exploring basic information about common health conditions.

## Features

- Add patient records with:
  - Name
  - Gender
  - Age
  - Health condition
- Generate an in-page report showing:
  - Total number of patients
  - Condition counts
  - Gender-based condition counts
- Search for information about:
  - Diabetes
  - Thyroid conditions
  - High blood pressure
- Display symptoms, prevention guidance, treatment information, and an image for each supported condition.
- Contact form for questions about health conditions and treatment methods.

> **Important:** This project is for educational and informational purposes only. It is not medical advice or a replacement for consultation with a qualified healthcare professional.

## Technologies Used

- HTML5
- CSS3
- JavaScript
- JSON

## Project Structure

```text
health_census/
├── index.html              # Main health analysis page
├── health_contact.html     # Contact page
├── health_analysis.css     # Application styling
├── health_analysis.js      # Patient report and condition search logic
├── health_analysis.json    # Condition information data
├── blood_pressure.jpg      # High blood pressure image
├── diabetes.jpg            # Diabetes image
└── thyroid.jpg             # Thyroid image
```

## Run Locally

No build tools or server are required for the basic application.

1. Clone the repository:

   ```bash
   git clone https://github.com/Shruti-12-S/health_census.git
   cd health_census
   ```

2. Open `index.html` in a web browser.

For the condition search to load `health_analysis.json` reliably, serve the project with a local web server:

```bash
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000) in your browser.

## Usage

### Add a patient

1. Enter the patient's name.
2. Select a gender.
3. Enter the patient's age.
4. Select a condition.
5. Click **Add Patient** to update the analysis report.

### Search for a condition

Enter one of the supported condition names in the search field and click **Search**. Search terms should match one of the following names:

- `Diabetes`
- `Thyroid`
- `High Blood Pressure`

## Data and Privacy

Patient records are stored only in the browser's in-memory JavaScript array and are not saved to a database or sent to a server. Records are lost when the page is refreshed.

Do not enter real personally identifiable or sensitive medical information into this demo application.
