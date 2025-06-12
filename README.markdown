# Secret Notes

A simple Python application built with Tkinter that allows users to save encrypted notes using a master key and decrypt them later. The notes are stored in a local text file (`mysecret.txt`) in an encrypted format using a custom encoding algorithm with Base64.

## Features
- **Encrypt Notes**: Save notes with a title and a master key for encryption.
- **Decrypt Notes**: Decrypt previously saved notes using the correct master key.
- **User-Friendly GUI**: Built with Tkinter for an intuitive interface.
- **Error Handling**: Displays error messages for missing inputs or invalid encrypted data.
- **Local Storage**: Encrypted notes are appended to a local file (`mysecret.txt`).

## Requirements
- Python 3.x
- Tkinter (usually included with Python)
- Base64 (included in Python's standard library)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/secret-notes.git
   cd secret-notes
   ```
2. Ensure Python 3 is installed on your system:
   ```bash
   python --version
   ```
3. No additional libraries are required since Tkinter and Base64 are part of Python's standard library.

## Usage
1. Run the application:
   ```bash
   python secret_notes.py
   ```
2. **To Save and Encrypt a Note**:
   - Enter a title in the "Enter your title" field.
   - Write your secret note in the "Enter your secret" text area.
   - Provide a master key in the "Enter master key" field.
   - Click the "Save & Encrypt" button to encrypt and save the note to `mysecret.txt`.
3. **To Decrypt a Note**:
   - Paste the encrypted note (from `mysecret.txt`) into the "Enter your secret" text area.
   - Enter the correct master key in the "Enter master key" field.
   - Click the "Decrypt" button to view the decrypted note.
4. **Note**:
   - Ensure all fields are filled before saving or decrypting, or an error message will appear.
   - If the wrong master key is used for decryption, or the encrypted data is invalid, an error will be shown.

## File Structure
- `secret_notes.py`: The main Python script containing the application code.
- `topsecret.png`: The image file used for the application's logo (ensure it is in the same directory as the script).
- `mysecret.txt`: The file where encrypted notes are stored (created automatically when saving notes).
- `README.md`: This documentation file.

## Example
### Saving a Note
- Title: `My Secret`
- Note: `This is a confidential message.`
- Master Key: `mykey`
- After clicking "Save & Encrypt", the note is encrypted and appended to `mysecret.txt`.

### Decrypting a Note
- Copy the encrypted text from `mysecret.txt` into the text area.
- Enter the master key (`mykey`).
- Click "Decrypt" to reveal: `This is a confidential message.`

## Notes
- The encryption uses a simple algorithm based on character shifting with the master key and Base64 encoding. It is not suitable for highly sensitive data requiring strong security.
- Ensure the `topsecret.png` image is present in the same directory as the script, or the application will raise an error.
- The application appends new notes to `mysecret.txt` without overwriting existing ones.

## Contributing
Feel free to fork this repository, submit issues, or create pull requests to improve the application. Suggestions for enhancing security, adding features, or improving the UI are welcome!

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Built with [Python](https://www.python.org/) and [Tkinter](https://docs.python.org/3/library/tkinter.html).
- Inspired by the need for a simple, user-friendly note encryption tool.