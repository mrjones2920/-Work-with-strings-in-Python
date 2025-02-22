# Work with strings in Python

<h1>Introduction</h1>
Security analysts work with a lot of string data. For example, some security analysts work on creating and updating IDs such as employee IDs and device IDs, which are commonly represented as strings. As another example, certain network activity will be stored as string data. Becoming comfortable working with strings in Python is essential for the work of a security analyst.

In this lab, you'll practice creating Python code and working with strings. You'll work with an employee ID, a device ID, and a URL, all represented as string data.

<h1>Scenario</h1>
You're working as a security analyst, and you are responsible for writing programs in Python to automate updating employee IDs, extracting characters from a device ID, and extracting components from a URL.

<h1>Task 1</h1>
In your organization, employee IDs are currently either four digits or five digits in length. In this task, you're given a four-digit numeric employee ID stored in a variable called employee_id. Convert this to a string format and store the result in the same variable. Later, you'll update this employee ID string so that it complies with a new standardized format.

Complete the following code. Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell.

![image](https://github.com/user-attachments/assets/4d5cf89c-91bc-469a-89be-f694a4633e32)

<h1>Question 1</h1>
What do you observe about the data type of employee_id the first time it's displayed? What do you observe about the data type of employee_id the second time it's displayed (after the variable is reassigned)?

The first time it is displayed, the data type of employee_id is integer. The second time it is displayed (after the variable is reassigned), the data type of employee_id is string.

<h1>Task 2</h1>
Imagine that you have just been informed of a new criteria for employee IDs. They must all be five digits long for standardization purposes.

In this task, you will write a conditional statement that displays a message if the length of the employee ID is less than five digits.

Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell.

![image](https://github.com/user-attachments/assets/00621e35-174a-4bfa-adba-2772cb87eb06)

<h1>Task 3</h1>
In this task, you'll build upon the previous code. If an employee ID is only four digits, you'll use concatenation to create a five-digit employee ID number.

Concatenation is a process that allows you to merge strings together. The addition operator (+) in Python allows you to concatenate two strings.

Write an if statement that evaluates whether the length of employee_id is less than 5. When the condition evaluates to True, reassign employee_id by concatenating "E" in front of the four-digit employee ID to create a five character employee ID. Then, display employee_id again. Be sure to replace each ### YOUR CODE HERE ### with your own code before you run the following cell.

![image](https://github.com/user-attachments/assets/84b82531-87a1-4953-83db-d84e558d373c)

<h1>Task 4</h1>
Now you'll move on to the next part of your task. Imagine that the characters in a device ID convey technical information about the device. You'll need to extract characters in specific positions from the device ID. Start off by extracting the fourth character.

The variable device_id represents a device ID containing alphanumeric characters; it's already stored as a string.

Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell.

![image](https://github.com/user-attachments/assets/4c71f02b-d2b6-49cc-94a1-8c300eb7dfc7)

<h1>Task 5</h1>
Now you will also need to extract the first through the third characters in the device ID. So take a slice of the device ID. You can achieve this using bracket notation in Python. Then, display the slice to examine the result.

Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell.

![image](https://github.com/user-attachments/assets/01cfd1e4-ae1a-4f84-b146-47db8f54a9be)

<h1>Task 6</h1>
You'll now proceed to the last part of your task. This involves extracting components of a URL.

You'll work with string indices to display various components of a URL that's stored in the URL variable. First, you'll extract and display the protocol of the URL and the :// characters that follow it using string slicing. Consider that the protocol is in the secure format of https when determining the indices for your slice.

Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell.

![image](https://github.com/user-attachments/assets/b40c1002-3cd2-441d-ad42-a9a80a47f98c)

<h1>Task 7</h1>
Later in this lab, you'll extract the domain extension. To prepare for this, use the .index() method to identify the index where the domain extension .com is located in the given URL.

Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell.

![image](https://github.com/user-attachments/assets/f18377d5-d3d9-4f9a-97c2-1751fbe439b0)

<H1>Task 8</H1>
It's a good idea to save important data in variables when programming. This allows for quick and easy tracking and reuse of information.

Store the output of the .index() method in a variable called ind, which is short for index. This index represents the position where the domain extension ".com" starts in the url. Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell. Note that running this cell will not produce an output.

![image](https://github.com/user-attachments/assets/16ba202e-3a6b-463d-810c-22e43579234d)

<H1>Task 9</H1>
You can use string slicing to also extract the domain extension of a URL. To do so, you can create a slice. The starting index should be the ind variable. This contains the index where the domain extension begins. The ending index should be ind + 4 (since ".com" is four characters long). Sometimes, like in this situation, it's easier to express the ending index in relation to the starting index. Examine the following code, run it as is, and observe the output.

![image](https://github.com/user-attachments/assets/b471c247-fd53-40e9-bb06-8241759027d6)

<H1>Question 2</H1>
What does this code output and why?

This code outputs the domain name .com by first saving the starting position of the domain name in the ind variable and then extracting 4 consecutive characters from url starting from the saved position.

<H1>Task 10</H1>
Finally, extract the website name from the given URL using string slicing and the ind variable that you defined earlier. In the given URL, the website name is "exampleURL1". Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell.

![image](https://github.com/user-attachments/assets/a2fc822c-0a00-4925-8569-f5cfa88cdf23)

<H1>Conclusion</H1>
What are your key takeaways from this lab?

- Strings are instrumental in storing important, security-related data, such as device IDs and URLs.
- String concatenation allows you to easily combine information in a string with the information stored in another string.
- String slicing is a powerful technique that enables you to extract any subsection of a string.
- Python has many functions and methods that help analysts work with string values, as well as data that they want to convert to string format.
- The type() function returns the data type of its input.
- The str() function converts the input object into a string. For example, when called on an integer, str() returns that integer value converted to a string.
- The len() function returns the number of elements in an object. When called on a string, len() returns the number of characters in that string.
- The .index() method finds the first occurrence of the input in a string and returns its location. It provides the index where the substring begins.
