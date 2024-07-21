# SecurityLock-Assembly-Language-Project

### Security Lock Project using Emu8086 Assembly Language

#### Description:
This project implements a simple security lock system using Emu8086 assembly language. It prompts the user for an ID and a corresponding password from predefined lists, and grants access if both match correctly. If either the ID or password is incorrect, appropriate error messages are displayed.

#### Components:
- **ID and Password Database**: 
  - The IDs and passwords are stored in predefined arrays (`ID` and `Password` arrays).
  - Each ID corresponds to a password stored at the same index position in their respective arrays.

- **User Interface**:
  - Messages (`MSG1`, `MSG2`, `MSG3`, `MSG4`, `MSG5`, `MSG6`) guide the user through the ID and password entry process.
  - Error messages (`MSG3`, `MSG4`, `MSG6`) notify the user in case of invalid input or authentication failure.

- **Functionality**:
  - **ID Input**: Prompts the user to enter an ID. If the entered ID matches one from the database (`ID` array), the program proceeds to prompt for the password.
  - **Password Input**: Once a valid ID is entered, prompts the user to enter the corresponding password. If the entered password matches the one stored in the `Password` array at the index of the ID, access is granted.
  - **Validation**: Handles cases where the entered ID or password is incorrect, displaying appropriate error messages.

#### Usage:
1. **Running the Program**: Load and run the program in an Emu8086 environment or compatible assembler.
2. **Entering ID and Password**: Follow the prompts to enter an ID and a corresponding password from the provided lists.
3. **Access Status**: Based on input correctness, you will either gain access or receive an error message indicating the reason for denial.

#### Notes:
- **Code Customization**: Modify the `ID` and `Password` arrays to include additional IDs and passwords as needed.
- **Error Handling**: Ensure correct handling of edge cases such as incorrect input lengths (`TooLong` condition).
- **User Interface**: Customize messages (`MSG1` through `MSG6`) for clarity or localization requirements.

