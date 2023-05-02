# mapping
a simple way of mapping of data this is used so that a value or data can be assigned to one adress


// SPDX-License-Identifier: MIT
pragma solidity  ^0.8.13;

contract  maping {

    mapping (address => uint) public testing;

    function set(address _addr, uint _num) public
    {
        testing[_addr] = _num;
    }

    
}





__________________

A new code for making a coin in which a coin maker or minter have a address and when the amount is set to that particular balance, the number of coins will
tranfer to that minter


// SPDX-License-Identifier: MIT
pragma solidity  ^0.8.13;

contract  maping {

    address public minter; 


    mapping (address => uint) public coin;

    constructor()
    {
        minter = msg.sender;
    }

    function set(address _receiver, uint amount) public 
    {
        coin[_receiver] += amount;
    }

    
}
