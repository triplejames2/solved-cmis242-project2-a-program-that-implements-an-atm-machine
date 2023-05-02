Download Link: https://assignmentchef.com/product/solved-cmis242-project2-a-program-that-implements-an-atm-machine
<br>
<strong>Project 2 </strong>

This project involves writing a program that implements an ATM machine. The interface to the program should be a Java GUI that looks similar to the following:

The program should consist of three classes.

<ol>

 <li>The first class should define the GUI. In addition to the main method and a constructor to build the GUI, event handlers will be needed to handle each of the four buttons shown above. When the <em>Withdraw </em>button is clicked, several checks must be made. The first check is to ensure the value in the text field is numeric. Next a check must be made to ensure the amount is in increments of $20. At that point an attempt to withdraw the funds is made from the account selected by the radio buttons. The attempt might result in an exception being thrown for insufficient funds, If any of those three errors occur a JOptionPane window should be displayed explaining the error. Otherwise a window should be displayed confirming that the withdrawal has succeeded. When the <em>Deposit </em>button is clicked the only necessary check is to ensure that the amount input in the textfield is numeric. Clicking the <em>Transfer </em>button signifies transferring funds to the selected account from the other account. The checks needed are to confirm that the amount supplied is numeric and that there are sufficient funds in the account from which the funds are being transferred. Clicking the <em>Balance</em> button will cause a <sub>JOptionPane</sub> window to be displayed showing the current balance in the selected account. The main class must contain two <sub>Account</sub> objects, one for the checking account and another for the savings account.</li>

 <li>The second class is <sub>Account</sub>. It must have a constructor plus a method that corresponds to each of the four buttons in the GUI. It must also incorporate logic to deduct a service charge of $1.50 when more than four total withdrawals are made from either account. Note that this means, for example, if two withdrawals are made from the checking and two from the savings, any withdrawal from either account thereafter incurs the service charge. The method that performs the withdrawals must throw an <sub>InsufficientFunds</sub> exception whenever an attempt is made to withdraw more funds than are available in the account. Note that when service charges apply, there must also be sufficient funds to pay for that charge.</li>

</ol>




<ol start="3">

 <li>The third class is <sub>InsufficientFunds</sub>, which is a user defined checked exception.</li>

</ol>

The google recommended Java style guide, provided as link in the week 2 content, should be used to format and document your code. Specifically, the following style guide attributes should be addressed:

<ul>

 <li>Header comments include filename, author, date and brief purpose of the program.</li>

 <li>In-line comments used to describe major functionality of the code.</li>

 <li>Meaningful variable names and prompts applied.</li>

 <li>Class names are written in UpperCamelCase.</li>

 <li>Variable names are written in lowerCamelCase.</li>

 <li>Constant names are in written in All Capitals.  Braces use K&amp;R style<strong>.</strong></li>

</ul>

In addition the following design constraints should be followed:

<ul>

 <li>Declare all instance variables private</li>

 <li>Avoid the duplication of code</li>

</ul>

Test cases should be supplied in the form of table with columns indicating the input values, expected output, actual output and if the test case passed or failed. This table should contain 4 columns with appropriate labels and a row for each test case.  Note that the actual output should be the actual results you receive when running your program and applying the input for the test record. Be sure to select enough different scenarios to completely test the program.