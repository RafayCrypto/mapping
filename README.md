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
