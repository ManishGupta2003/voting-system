## Student Voting System
Student Voting System is a simple console-based project created for student elections, in which the students can take part in voting for their favorite candidates. The authority, namely the admin, has the capability to manage the election process, for example starting out new elections, banning user IDs, and removing illegal votes from the system.
## Features
- **Student Panel**:
  - Spend your unique user identification to log in to your account.
  - Give votes to the candidates that are available.
  - To avoid duplicate voting and the detection of the banned user IDs will be done by the different methods you have to use.
- **Admin Panel**:
  - Launch a new election.
  - To make the voters of the previous election to continue with the voting process you can choose this option.
  - Get rid of the bad ballots.
  - Ban specific user IDs.
  - Display election results.
## File Structure
- `main.c`: This is the primary source code file, which contains everything about the voting system in it.
- `ElectionInfo.txt`: It is meant to keep the existent elections' data.
- candidateX.txt: Contains candidate vote and student ID where 'X' is the candidate ID.
- `Banned.txt`: It lists the banned students' IDs.
## Usage
### Compile and Run
1. **Compile the Code**:
   ```sh
   gcc -o voting_system main.c
   ```
2. **Run the Program**:
   ```sh
   ./voting_system
   ```
### Student Panel
1. **Enter User ID**: A message by the system will be sent to you requesting to give your user ID.
2. **Vote for a Candidate**: If you are sure that your user ID is just perfect and you have never voted before then you can vote by entering the candidate number.
3. **Exit**: To leave the student panel, enter `0` when asked for a user ID.
### Admin Panel
1. **Login**: Provide the username (`Admin`) and the password (`admin`) to sign in.
2. **Manage Election**: On the successful login, the following options will be open:
  - **New Election**: Launch a new election by providing the year, branch code, maximum roll number, and candidate information.
  - **Delete Illegal Vote**: Delete a vote by typing in the user ID correctly.
  - **Ban User IDs**: Disable the entrance tests of specific users using their roll numbers.
  - **Result**: Display the prevailing outcomes of the election.
  - **Logout**: Get off the admin panel.
