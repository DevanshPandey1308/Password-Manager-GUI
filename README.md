# PASSWORD MANAGER GUI(PYTHON)

A simple Python desktop application for generating strong passwords and managing website credentials using a clean Tkinter interface. This project is intended for learning and personal experimentation, not for managing sensitive real-world passwords.

FEATURES :-
1.Strong Password Generation
 •Generates secure, random passwords with letters, numbers, and symbols.
 •Automatically copies the generated password to the clipboard using `pyperclip`.

2.Store Login Credentials
 •Saves website, email/username, and password to a local `data.json` file.
 •Creates `data.json` automatically on first save if it does not exist.
 •Merges new entries with existing records without overwriting other websites.

3.Search Saved Credentials
 •Look up saved details by entering the website name.
 •Shows the stored email and password in a pop-up message box.
 •Automatically copies the retrieved password to the clipboard.

4.Minimal Tkinter UI
 •Clean and user-friendly layout with labeled fields and buttons.
 •Optional logo image (`logo.png`) to give the app a polished look.


PROJECT STRUCTURE :-
│── main.py 
│── data.json 
│── logo.png 
│── screenshots/ 
│── README.md
│── requirements.txt


REQUIREMENTS :-
Install required packages:
```
pip install pyperclip
```
Tkinter is included with most Python installations by default.


HOW TO USE :-
1. Run the application:
```
python main.py
```
2. Enter:
   - **Website**
   - **Email/Username**
   - **Password**
     - Or click **Generate Password** to auto-generate.
     - 
3. Click **Add** to save the credentials into `data.json`.

4. To search saved details:
   - Enter the website name
   - Click **Search**

JSON STORAGE FORMAT :-
Credentials are stored in the following format:

```json
{
    "example.com": {
        "email": "your-email@example.com",
        "password": "generatedPassword123!"
    }
}
```

