# Voting App

## Description
The Voting App is a platform where users can securely vote for candidates in an election. It ensures election integrity by implementing strict user authentication and role-based access control.

## Features
- **User Authentication**:
  - Sign up and log in using a unique government ID (Aadhaar card).
  - Change password functionality.
- **Voting**:
  - View a list of candidates.
  - Vote for a candidate (one vote per user).
- **Vote Count**:
  - View real-time vote counts for candidates, sorted by vote count.
- **Admin Functionality**:
  - Manage candidates (add, update, delete).
  - Restricted access to sensitive election data.

## API Routes

### User
- `POST /createuser` - Create a new user account.
- `POST /loginuser` - Log into an existing account.

### User Profile
- `GET /userprofile` - Retrieve the user's profile information.
- `PUT /userprofile/password` - Change the user's password.

### Voting
- `GET /candidates` - Retrieve the list of candidates.
- `POST /vote/:candidateId` - Vote for a specific candidate.

### Vote Count
- `GET /vote/counts` - Retrieve the list of candidates sorted by their vote counts.

### Admin
- `POST /candidates` - Add a new candidate.
- `PUT /candidates/:candidateId` - Update an existing candidate.
- `DELETE /candidates/:candidateId` - Remove a candidate.

## Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>

2. Navigate to the project directory:
    cd Voting_App

3. Install dependencies:
    npm install

Usage
    1. Start the server:
        node server.js

    2. Access the application via the configured server URL.

License
This project is licensed under the ISC License.

