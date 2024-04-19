# solidity-unique-critic (problems and answers)

## Easy

<details open>
<summary><b><font size="+1">1. There is byte32 value. Convert this value to address type and yield two results. first result is truncate to left end of the value counting 20bit. and twice value is truncate to right end of the value counting 20bit.</font></b></summary>

`byte32` value = 0x111122223333444455556666777788889999AAAABBBBCCCCDDDDEEEEFFFFCCCC;<br>
`address` first = `address`(`uint160`(`uint256`(b))) = 0x777788889999AaAAbBbbCcccddDdeeeEfFFfCcCc<br>
`address` twice = `address`(`uint160`(`byte20`(b))) = 0x111122223333444455556666777788889999aAaa

_Reference_: https://docs.soliditylang.org/en/latest/types.html

</details>

<br>

