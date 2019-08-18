//Smart contract for creating usersdata for reward points
//
pragma solidity 0.5.11;

contract NewUser {
    
    uint256 public userCounter;
    uint256 public starterPoint;
    mapping(uint => User) public users;
    
    address owner;
    
    modifier onlyOwner () {
        require (msg.sender == owner);
        _;
    }
    
    struct User {
        uint _id;
        string _name;
        string _address;
        uint _age;
        uint _points;
        uint _blocknum;
        uint _time;
    }
    
    constructor() public {
        owner = msg.sender;
    }
    
    function addUser(string memory _name, string memory _address, uint _age) public onlyOwner {
        incrementCounter();
        starterPoint = 1000;
        users[userCounter] = User(userCounter, _name, _address, _age, starterPoint, block.number, block.timestamp);
    }
    
    function incrementCounter() internal {
        userCounter += 1;
    }
    
    function addPoints(uint _id) public {
        uint addPoint = 1000;
    //    users[_id] = User(_id, _name, _address, _age);
    }
}
