# Smart contract for the signing up of user for a points program
### v 0.5.11
### To be compiled with the newest version of Solidity.
### Code ported solidity version 0.4.24
### Code updated by CryptoLuigi

A user account has different properties.
```
        uint _id;
        string _name;
        string _address;
        uint _age;
        uint _points;
        uint _blocknum;
        uint _time;
```
The block number is used a way to determine when the user sign up for the program.

```
Member since block: 234234
```
With the user ID number a Users records can be pulled up.
This is accompolished with the user's ID number which is generated upon completion.
