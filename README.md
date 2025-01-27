```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract UlasCanSenturk {
    struct ContactInfo {
        string linkedin;
        string email;
        string discord;
    }

    string public title;
    ContactInfo public contact;

    constructor() {
        title = "software & blockchain developer/ ethereum evangelist / human being";
        contact = ContactInfo({
            linkedin: "ulascansenturk",
            email: "ulascansenturk1@gmail.com",
            discord: "kernelpanic#4413",
	    twitter: "0xUlascan"	

        });
    }

    function getTitle() public view returns (string memory) {
        return title;
    }

    function getContactInfo() public view returns (string memory, string memory, string memory) {
        return (contact.linkedin, contact.email, contact.discord);
    }
}
```
