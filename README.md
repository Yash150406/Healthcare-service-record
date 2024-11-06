# Healthcare Service Records - Phone Directory Search

This is a simple C program designed to store and search phone numbers in a healthcare directory. The program validates phone number formats, allows users to search for contact information based on a given phone number, and displays the associated name and area of the person. The phone numbers are stored in a predefined list, and the program checks if the input phone number matches any entry in the directory.

## Features

- **Phone Number Validation:** Ensures the entered phone number is in the format `+91-XXXXXXXXXXX`.
- **Phone Directory Search:** Searches for a specific phone number in the directory and returns the corresponding person's name and address if found.
- **Simple User Interface:** Prompts the user for a phone number, checks for validity, and displays results accordingly.

## Prerequisites

This program is written in C and should work on any system that supports the C language. You will need the following to run this program:

- A C compiler (e.g., GCC, Clang).
- A terminal or command-line interface to compile and run the program.

## How to Compile and Run

1. Clone or download the repository to your local machine.
2. Open a terminal in the directory containing the C file (`healthcare_directory.c`).
3. Compile the C file using a C compiler:
   ```bash
   gcc healthcare_directory.c -o healthcare_directory
   ```
4. Run the program:
   ```bash
   ./healthcare_directory
   ```

## Example Usage

```bash
HEALTHCARE SERVICE RECORDS:
(FOR EMERGENCY OR PATIENT CONTACT)
Enter phone number (format: +91-XXXXXXXXXXX): +91-9988776655
Found: Ananya Sharma
Area: Flat No. 101, Sai Samarth Residency, Near Ganesh Mandir, Kothrud, Pune
```

If the phone number is not found in the directory or the format is incorrect, the program will display an appropriate message.

## Code Overview

The program is structured as follows:

1. **validatePhoneNumber function**: This function ensures that the entered phone number is in the correct format (`+91-XXXXXXXXXXX`).
2. **searchPhoneNumber function**: This function searches the predefined list of phone numbers and matches the input phone number with the corresponding entry in the directory. If a match is found, it displays the name and address of the person associated with the phone number.
3. **Main function**: The main entry point of the program where user input is received and the other functions are called to perform the necessary validation and search.

### Key Data Structures

- **phone**: A 2D array that stores the phone numbers of the contacts.
- **name**: A 2D array that stores the names of the contacts.
- **area**: A 2D array that stores the area (address) of each contact.

### Phone Format

The program expects the phone number to be in the following format:
```
+91-XXXXXXXXXXX
```
Where `X` is any digit from `0` to `9`. This format corresponds to a typical Indian phone number with the country code `+91`.

## Contributing

Feel free to fork the repository and create pull requests. Contributions are welcome to improve the functionality, add more features, or fix any bugs.
