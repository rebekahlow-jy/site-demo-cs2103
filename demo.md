## Test case design approaches

<!-- <panel header="Exploratory testing vs scripted testing :rocket:" expandable type="primary" is-open> -->

## Exploratory testing vs scripted testing
Previously, two alternative approaches to test case design were discussed: exploratory vs scripted. That distinction was based on when the test cases are designed. In scripted approach, they are designed in advance. In the exploratory approach, they are designed on the fly.
Given next are alternative approaches based on some other aspects of testing.

<!-- </panel> -->

<!-- <panel header="Black-box vs white-box" expandable type="seamless"> -->

## Black-box vs white-box
This categorization is based on how much of SUT (software under test) internal details are considered when designing test cases. In the black-box approach, also known as specification-based or responsibility-based testing, test cases are designed exclusively based on the SUT’s specified external behavior. In the white-box approach, also known as glass-box or structured or implementation-based testing, test cases are designed based on what is known about the SUT’s implementation, i.e. the code.
Knowing some important information about the implementation can help in black-box testing. This kind of testing is sometimes called gray-box testing. For example, if the implementation of a sort operation uses an algorithm to sort lists shorter than 1000 items and another to sort lists longer than 1000 items, more meaningful test cases can then be added to verify the correctness of both algorithms.

<!-- </panel> -->
