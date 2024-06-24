# InternDB Discord Bot

## Introduction

A Discord Bot to interact with an internship database, allowing users to record and query internship processes and information.

## Partners

- [Tech Career North](https://techcareerchange.vercel.app/)

## Features

- Users can query their own processes or those of other companies, both in both public channels and DMs.
- Users can query specific information such as interview questions, compensation details and more, in both public channels and DMs.
- Users can record their internship application steps in a specific public channel.
- The bot will DM users to survey them about their internship process steps, anonymizing and storing the information in the database.

## Usage

### Help Command

`!help`: Provides a list of available commands and their descriptions.

### Query Process

`!query process [parameter]`: Allows users to query their own process or processes by companies. Queries can be made in public channels or via DMs.
- Parameters:
    - `company` (required): Filters query to a specific company.
    - `pay` (optional): Filters the query to information about pay.
    - `questions` (optional): Filters the query to interview questions.

Example Input:

`!query process company=Google`

### Query Information

`!query info [parameter]`: Allows users to query information recorded in the database. Queries can be made in public channels or via DMs.
- Parameters:
    - `company` (required): Filters query to a specific company.
    - `step` (required): Filters query to a specific step in the process.

Example Input:

`!query info company=Google`

Example Output:

```
Discord Handle: @user1
Company: Google
Step: OA
---
Discord Handle: @user2
Company: Google
Step: Final Round
```

### Record Process

`!record process [step]`: Allows users to record their internship application process steps in a specific public channel in TCN. No process recording is allowed in DMs to boost engagement.
- Parameters:
    - `step`: The current step in the internship process (e.g., Applied, Technical Screening, HR Screening, OA, Onsite, Offer, Accepted, Declined, Rejected, [custom]).

### Record Information

The bot will DM users every time they advance to a new step in the process to survey them about the step. This information will be anonymized and stored in the database.

## Installation

Instructions on how to set up the development environment.

## Contribution

See [CONTRIBUTING.md](CONTRIBUTING.md) for contribution guidelines.

## License
