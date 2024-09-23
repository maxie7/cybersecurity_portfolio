<h1>Updating A File Through Python Algorithm</h1>

<h2>Languages and Utilities Used</h2>

- <b>Phython</b> 

<h2>Description</h2>

At my (fictitious) organization, access to restricted content is controlled with an allow list of IP addresses. The "allow_list.txt" file identifies these IP addresses. A separate remove list identifies IP addresses that should no longer have access to this content. I created an algorithm to automate updating the "allow_list.txt" file and remove these IP addresses that should no longer have access. 

<br />

<h2>Opening the file that contains the allow list</h2>

For the first part of the algorithm, I opened the "allow_list.txt" file. First, I assigned this file name as a string to the import_file variable:

<p align="center">
<img src="https://imgur.com/ftwP9Yp.png" height="80%" width="80%" alt="Assigning This File As A String To import_file variable"/> </p>

Then, I used a 'with' statement to open the file:

<p align="center">
<img src="https://imgur.com/ok8PPcB.png" height="80%" width="80%" alt="Opening A File Using With Statement"/> </p>

In my algorithm, I utilize the 'with' statement along with the '.open()' function in read mode to access and read the allow list file. This file contains a list of IP addresses that I need for further processing. The 'with' keyword is essential for managing resources efficiently as it automatically closes the file after leaving the 'with' statement.

In the code snippet 'with open(import_file, "r") as file:', the 'open()' function takes two parameters. The first parameter specifies the file to be imported, and the second parameter indicates the intended action on the file. Here, "r" signifies that I want to read the file. Additionally, the 'as' keyword allows me to assign the output of the '.open()' function to a variable named 'file', which enables me to work with the contents of the file within the 'with' statement.

<h2>Reading the file contents</h2>

In order to read the file contents, I used the .read() method to convert it into the string.

<p align="center">
<img src="https://imgur.com/bQvNVLI.png" height="80%" width="80%" alt="Using Read Method To Convert Into The String"/> </p>

By utilizing the .open() function with the "r" argument for "read," I can employ the .read() function within the with statement's body. This .read() method effectively converts the contents of the file into a string, allowing me to access its data. I utilized the .read() method on the file variable specified in the with statement and stored the resulting string output in the variable ip_addresses.

To summarize, the provided code reads the content of the "allow_list.txt" file, converting it into a string format, which I can later use to organize and extract data within my Python program.

<h2>Converting the string into a list</h2>

In order to remove individual IP addresses from the allow list, I needed it to be in list format. Therefore, I next used the .split() method to convert the ip_addresses string into a list:

<p align="center">
<img src="https://imgur.com/0nBquej.png" height="80%" width="80%" alt="Converting String Into List"/> </p>

To convert the contents of a string variable into a list, the .split() function is used by appending it to the string. In this case, the goal is to create a list of IP addresses from the variable ip_addresses to facilitate the removal of specific addresses from the allow list. By default, the .split() function divides the text into list elements based on whitespace. In this algorithm, we utilize the .split() function on the data stored in the ip_addresses variable, which contains a string of IP addresses separated by whitespace, to transform it into a list of IP addresses. The resulting list is then reassigned to the variable ip_addresses for storage.


<h2>Iterating through the remove list</h2>

A key part of my algorithm involves iterating through the IP addresses that are elements in the remove_list. To do this, I incorporated a for loop:

<p align="center">
<img src="https://imgur.com/W8I2IQs.png" height="80%" width="80%" alt="Iterating Through Remove List"/> </p>

In Python, the for loop is utilized to execute a set of code statements repeatedly for a given sequence. Its primary objective is to apply specific code logic to each element within the sequence. The for loop begins with the keyword "for," followed by the loop variable "element," and the keyword "in." The "in" keyword indicates that the loop will iterate through the sequence "remove_list," assigning each value to the loop variable "element." This iterative process enables efficient handling of each element within the sequence.

<h2>Removing IP addresses that are on the remove list</h2>

To achieve the desired functionality, my algorithm involves eliminating any IP address from the allow list, ip_addresses, that is also present in the remove_list. Since there were no duplicates in ip_addresses, I was able to utilize the following code to accomplish this task:

<p align="center">
<img src="https://imgur.com/A2lRoLO.png" height="80%" width="80%" alt="Removing IP addresses that are on the remove list"/> </p>

To begin, I implemented a conditional statement within my for loop to check if the loop variable 'element' existed in the 'ip_addresses' list. 

Once the conditional was in place, I utilized .remove() on 'ip_addresses' within that block. By passing the loop variable 'element' as an argument, I ensured that each IP address listed in the 'remove_list' would be successfully eliminated from the 'ip_addresses' list.

<h2>Updating the file with the revised list of IP addresses</h2>

In the concluding phase of my algorithm, the last task involved updating the allow list file with the modified list of IP addresses. To accomplish this, I converted the list back into a string. To perform the conversion, I employed the .join() method.

<p align="center">
<img src="https://imgur.com/vKTxEg9.png" height="80%" width="80%" alt="Updating the file with the revised list"/> </p>

The .join() method is a useful tool to merge all items in an iterable into a single string. To use the .join() method, you apply it to a string containing the characters that will separate the elements in the iterable when they are combined into a string. In my algorithm, I utilized the .join() method to convert the list of IP addresses, called "ip_addresses," into a string format. This allowed me to pass it as an argument to the .write() method when writing the data to the file "allow_list.txt." To ensure each element appears on a new line in the file, I used the string ("\n") as the separator, effectively instructing Python to place each IP address on a separate line.

Then, I used another with statement and the .write() method to update the file:

<p align="center">
<img src="https://imgur.com/rhIFimR.png" height="80%" width="80%" alt="Updating the file using with statement"/> </p>

This time, I utilized a second argument, "w", with the open() function in my with statement. The "w" argument signifies my intention to open the file for writing, allowing me to overwrite its existing contents. With this argument in place, I can now employ the .write() function within the body of the with statement. The .write() function enables me to write a string of data to the specified file, effectively replacing any previous content.

In this scenario, my goal was to update the allow list and write it as a string to the file named "allow_list.txt." By doing so, any IP addresses that were removed from the allow list will no longer have access to the restricted content. To achieve this, I appended the .write() function to the file object "file," which I had previously identified in the with statement. I passed in the "ip_addresses" variable as the argument, signifying that the contents of the file specified in the with statement should be replaced with the data stored in this variable.

<h2>Summary</h2>

I developed an algorithm to update the "allow_list.txt" file, which contains a list of approved IP addresses. The algorithm is designed to remove IP addresses that are present in the "remove_list" variable. Here's a breakdown of the steps involved:

- Open the "allow_list.txt" file and read its contents as a string.
- Convert the string to a list of IP addresses, stored in the variable "ip_addresses."
- Iterate through the IP addresses in the "remove_list."
- For each IP address in the "remove_list," check if it exists in the "ip_addresses" list.
- If the IP address is found in the "ip_addresses" list, remove it using the .remove() method.
- After all the relevant IP addresses are removed, use the .join() method to convert the "ip_addresses" list back into a string.
- Overwrite the contents of the "allow_list.txt" file with the updated list of IP addresses.
  
By executing this algorithm, the "allow_list.txt" file will be modified to exclude the IP addresses specified in the "remove_list," ensuring that only the approved IP addresses remain in the file.
