

## Table of Contents

- [About](#about)
- [Features](#features)
- [How It Works](#how-it-works)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Demo](#demo)
- [Technologies Used](#technologies-used)
- [Contributors](#contributors)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## About

Child safety QR AI, designed to enhance child safety and identification. Our project, the **QR Art Generator**, leverages stable diffusion and control net techniques to generate captivating AI art QR codes. These QR codes can be used as stylish stickers or badges on a child's belongings. In the unfortunate event that a child goes missing, the QR code can be scanned to access vital information through a hosted PDF, aiding in their safe return.

## Features

- Generate AI Art QR codes using stable diffusion and control net techniques.
- Create custom QR codes by filling out a user-friendly form containing essential child details.
- Host generated QR AI art on a PDF via Azure Blob
- Enhance child safety by attaching QR codes as stylish stickers or badges on bags or clothes.

## How It Works

1. Users fill out a form with the child's information, such as name, date of birth, contact details, school, and more.
2. The provided information is uploaded to Azure blob storage to generate a hosted PDF containing the child's details.
3. The link to the hosted PDF is then passed to the Hugging gooey art api, which utilizes the `QR monster V2` model to generate a unique AI art QR code.
4. The generated QR AI art can be downloaded and printed as stickers or badges to be attached to the child's belongings.
5. In case of an emergency or if the child is lost, anyone can scan the QR code to access the child's details through the hosted PDF link, facilitating a swift and safe return.

## Getting Started

### Prerequisites

- Python 3.6+
- [Streamlit](https://streamlit.io/)
- Azure Storage Accounts

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/YourUsername/YourRepository.git
   cd YourRepository
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

0. Setup your .env file

   ```
   GOOEY_API_KEY=
   AZURE_STORAGE_CONNECTION_STRING=

   ```

1. Run the Streamlit app:

   ```bash
   streamlit run app.py
   ```

2. Fill out the form with the child's information and submit it.
3. Follow the instructions to access and download the generated QR AI art.

## Demo

![QR Art Generator Demo](https://path-to-your-demo-gif.gif)

Check out our live demo [here](https://link-to-your-live-demo)!

## Technologies Used

- Python
- Streamlit
- Azure
