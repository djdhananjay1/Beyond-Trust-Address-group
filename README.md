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
``` 
POST /auth/signappin
Headers: Authorization: PS-Auth key={{Key}}; runas=addressgrp
```
### Get Address ID
Fetch the list of address groups:
```
GET /BeyondTrust/api/public/v3/Addressgroups
```

### Post Address Group
Create a new address group:
```
POST /BeyondTrust/api/public/v3/AddressGroups/
```
```
Body: 
{
    "Name": "Iamapiaddressgroup"
}
```
### Post an Entry in Address Group
Add an entry to an existing address group:
```
POST /BeyondTrust/api/public/v3/AddressGroups/10005/Addresses
```
```
Body:
{
    "Type": 4,
    "Value": "10.1.1.2",
    "Omit": true
}
```
## Configuration
Update the variables in Postman:
```
Key: Your API key.
url: Your API endpoint URL (e.g., https://bipsurl/BeyondTrust/api/public/v3).
```

## Contributing
If you would like to contribute to this project, please follow the guidelines in CONTRIBUTING.md.

## License
This project is licensed under the MIT License - see the LICENSE file for details.


# ☕ Buy Me a Coffee

If you find my work helpful or enjoy using my projects, consider supporting me by buying me a coffee. Your support helps me continue creating and maintaining open-source projects.

<a href="https://paypal.me/DhananjayNidhonkar?country.x=IN&locale.x=en_GB" target="_blank">
  <img src="https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif" alt="Donate with PayPal" style="width: 150px; height: auto;">
</a>


## Why Support?

Maintaining and developing projects take time and effort. Your support enables me to dedicate more time to creating quality content, fixing bugs, and adding new features.

## How It Works

1. Click on the "Donate" button above.
2. You'll be redirected to my Paypal page.
3. Complete the transaction securely.

Thank you for your support! Every coffee is greatly appreciated.

## Supporters Wall

A big shoutout to the amazing people who have supported me by buying me a coffee! 🙌


If you'd like to be featured on this wall, include a message when you buy me a coffee, and I'll add your name here.

---

**Note**: Buying me a coffee is a one-time gesture. If you'd like to support me continuously, consider becoming a [GitHub Sponsor](https://github.com/sponsors)!

Thank you for supporting my work! ❤️
