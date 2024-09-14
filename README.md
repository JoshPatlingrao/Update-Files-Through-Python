# Update-Files-Through-Python

## Objective

### Skills Learned

### Tools Used

## Steps

### Open the File

The allow_list.txt is a file containing the list of valid IP addresses for the network. It’s name is temporarily saved in a global variable so it can be called anywhere in the code. That variable will be called in this case so the text file can be opened so it’s contents can be read. This is done through ‘with’ as the script will be handling an external .txt file, the ‘open()’ facilitates the access to the allow_list.txt file, while ‘r’ is to indicate the intent to read the contents of the file. The ’as’ saves the contents of the file in the local variable called ‘file’.

<p align="center">
  <img src="https://github.com/user-attachments/assets/5127faa8-2fee-422a-809a-c115d6d46ae0">
</p>

### Read the File

The file will be converted into string format through the ‘.read()’ function and will be saved in another variable ‘ip_addresses’. The ‘print()’ is used to display that the contents has been converted into string format.

<p align="center">
  <img src="https://github.com/user-attachments/assets/ba7ccb0d-7ea0-4947-a101-d1fde8e2077c">
</p>

### Convert the String to List

The string of IPs will then be converted into a list type through the ‘.split()’ function, no argument is needed as it will automatically interpret any white spaces or new lines as an indication for a separate element. The ‘print()’ is to display that this conversion has been successful.

<p align="center">
  <img src="https://github.com/user-attachments/assets/1f67d912-54fe-47aa-9336-c8bfb45045d3">
</p>

### Iterate Through the List

The list of compromised Ips to be removed have been provided in a list. The ‘for’ loop will be used to iterate through each elements sequentially so that the specified IPs will be removed from the approved list. The ‘print()’ is to display that ‘for’ loop is functioning properly.

<p align="center">
  <img src="https://github.com/user-attachments/assets/2a5c91e4-2e3f-47c1-855e-13f2ee65f967">
</p>

### Modify the List

The first ‘print()’ is to display the state of the approved IP list before modification. The ‘if’ operator will check if the current iteration or compromised IP in the ‘element’ variable is inside the approved IP list. If it is then that specific ‘element’ will be removed from the list through ‘.remove()’ function. The argument passed into the function is the ‘element’ that will be removed from the approved IP list. The last ‘print()’ is the check if modification has been successful.

<p align="center">
  <img src="https://github.com/user-attachments/assets/7912db03-7645-488b-a90e-91fd95b2d6f9">
</p>

### Update the File with Revised List

The modified list of approved IPs will now be converted back into string through ‘.join()’ function. The ‘\n’ will create a new line for each element so it matches its initial format, this will then be saved in the ip_address_list variable. The import_file variable will be called again but will be opened using ‘w’, indicating our intent to overwrite the previous contents with the modified list. This will be done through the ‘.write()’ function. The file will be opened again using ‘r’ to read it’s contents using ‘.read()’ to confirm its contents have been succesfully changed. The list of compromised IPs are no longer present in the text file.

<p align="center">
  <img src="https://github.com/user-attachments/assets/f445c638-46e5-42d3-b411-2764166d9110">
</p>

## Summary

This exercise showcases my ability and understanding of modifying text files through Python.
