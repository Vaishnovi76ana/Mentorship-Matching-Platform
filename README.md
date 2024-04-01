# Mentorship Matching Platform

## Introduction

This repository contains the source code for a Mentorship Matching Platform, designed to facilitate mentor-mentee relationships. This README.md file provides instructions on how to set up and run the application locally.

## Setup Instructions

### 1. Create a Virtual Environment

#### For Windows Users:

```bash
virtualenv env
```

#### Activate the Virtual Environment:

```bash
.\env\Scripts\activate.ps1
```

### 2. Install Dependencies

In the activated virtual environment, run the following command:

```bash
pip install -r requirements.txt
```

### 3. Insert Assets

Create a folder named `static` and insert the assets folder into it.

### 4. Configuration

Replace `sender_email` with your email address. Email will be sent from your email ID. For the `passcode`, use your Google App password. To generate an App password, enable 2-factor authentication if not enabled. Create an app name, and an app password will be generated. Copy it and replace `passcode` with it. Now, you can send emails to mentor/mentee email IDs from your email ID.

### 5. Running the Application

Run the following command:

```bash
python app.py
```

The application will start running on localhost.

### Additional Configurations

- **Database Setup**: The `schema.sql` file contains all tables of the database. No manual initialization is required.
- **File Uploads**: For file uploads, create a folder, for example, `file_uploads`. Add the path of the `file_uploads` in `app.config` like this: `app.config['UPLOAD_FOLDER']='C:\\..\\mentorship_matching_platform\\file_uploads'`.

## Conclusion

Follow these instructions carefully to set up and run the Mentorship Matching Platform locally. If you encounter any issues, refer to the documentation or contact the repository owner for support.
