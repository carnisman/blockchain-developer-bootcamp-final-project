## blockchain-developer-bootcamp-final-project

# A simple blockchain based system for value exchange between learners and educators

## About

__*A simple value exchange system where tutors and students engage in a one-on-one class*__

This aims to solve the exchange of value when a tutor and a student engage in a one-on-one class, specially when both resides in different countries. Both parts meet to arrange a economic value for the class or series of classes, and when they agree, the tutor puts the amount of ETH, and the amount of classes to be given on a smart contract. The student then sign that in  acceptance, and the specified value is stored in the contract wallet. When the student attend to a class, it signs a attendance counter, and the fraction corresponding to that class is available to the teacher to withdraw

## Flow
1. A tutor and a student agree on the quantity of classes and the total cost
2. A contract is filled and generated between the two parts, the total amount is then stored in that contract´s wallet
3. When the student attends to a class, it signs the attendance, which is a counter, the first class is 1, and the consequent classes are 2, 3, etc.
4. The tutor then can withdraw the amount equivalent to this formula: ((Total cost / Total classes) * Attended classes)
5. If the student doesn´t want to continue his lessons, the amount stored can be withdrawn according to this formula: (Total cost - ((Total cost / Total classes) * Attended classes))
6. A penalty system has not been thought yet, the idea is to have some sort of economic mechanism to avoid uncommitment on both parts

## Use example 1

Tutor and student agreed on 10 classes for a total cost of 10ETH. The tutor executes the contract and the student accept. The 10ETH from the student are stored on the contract wallet. When the student attend to a class and mark his attendance, allows the tutor to withdraw a quantity proportional to the amount of lessons attendend. The tutor can withdraw the available ETH, or wait to give more lessons and withdraw the accumulated amount later.

## Use example 2

Tutor and student agreed on 1 class for a total cost of 10ETH. The tutor executes the contract and the student accept. The 10ETH from the student are stored on the contract wallet. Before having the class the student regrets his decision and decide to withdraw the stored ETH, cancelling the class. He gets the full stored value minus fees

## Use example 3

Tutor and student agreed on 10 class for a total cost of 10ETH. The tutor executes the contract and the student accept. The 10ETH from the student are stored on the contract wallet. The student takes 3 lessons, but the decides to stop attending and withdraw the stored value on the contract´s wallet. He gets the stored value minus the value of the attended classes (7ETH minus fees)
