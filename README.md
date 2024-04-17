# Beyond-Trust-Address-group
This repository contains a Postman collection designed for managing address groups within the BeyondTrust Password Safe application. It enables users to perform operations such as authentication, retrieving address group IDs, creating new address groups, and adding entries to these groups via API calls.

## Features

This API collection offers the following features:
- **Authentication**: Authenticate using specific credentials to access the API.
- **Retrieve Address Groups**: Fetch a list of address group IDs.
- **Create Address Groups**: Add new address groups to the system.
- **Manage Address Group Entries**: Insert and manage entries in specific address groups.

## Prerequisites

Before you start using this API collection, you need the following:
- [Postman](https://www.postman.com/downloads/) installed on your computer.
- Access credentials for the BeyondTrust Password Safe environment.
- Ensure you have the necessary permissions to execute the API requests.

## Installation

To use this collection:
1. Download the `Address Group Management API Collection.postman_collection.json` file from this repository.
2. Open Postman.
3. Click on `File` > `Import...`.
4. Choose the downloaded JSON file and import it into Postman.

## Usage

To use the API collection, follow these steps for each request:

### Sign-in Copy
Authenticate to the system using your credentials:

'plaintext'
POST /auth/signappin
Headers: Authorization: PS-Auth key={{Key}}; runas=addressgrp

## Get Address ID
Fetch the list of address groups:

plaintext
Copy code
GET /BeyondTrust/api/public/v3/Addressgroups
Post Address Group
Create a new address group:

json
Copy code
POST /BeyondTrust/api/public/v3/AddressGroups/
Body: 
{
    "Name": "Iamapiaddressgroup"
}
Post an Entry in Address Group
Add an entry to an existing address group:

json
Copy code
POST /BeyondTrust/api/public/v3/AddressGroups/10005/Addresses
Body:
{
    "Type": 4,
    "Value": "10.1.1.2",
    "Omit": true
}
Configuration
Update the variables in Postman:

Key: Your API key.
url: Your API endpoint URL (e.g., https://192.168.94.131/BeyondTrust/api/public/v3).
Contributing
Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

To contribute:

Fork the Project
Create your Feature Branch (git checkout -b feature/AmazingFeature)
Commit your Changes (git commit -m 'Add some AmazingFeature')
Push to the Branch (git push origin feature/AmazingFeature)
Open a Pull Request
License
Distributed under the MIT License. See LICENSE for more information.

Contact
Your Name - your-email@example.com

Project Link: https://github.com/yourusername/your-repository-name
