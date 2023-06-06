# GGtest

Google Gruyere Privilege Elevation Exploit


## Code Explanation

This code demonstrates a privilege elevation exploit using the Playwright library. The exploit targets the Gruyere application and attempts to elevate user privileges. The code is written in Python and includes a command-line application and a test case.

0. Use python package manager 'pip' via terminal, to allow install of 'Typer' and 'Playwright' libraries to use necessary modules.   
   - To check if pip is installed, in the terminal 'pip --version' is run.
   - Install of 'Typer' via terminal 'pip install typer' is run. 
   - Install of 'Playwright' via terminal 'pip install playwright' is run.

Command-Line Application

The code includes a command-line application that utilizes the Typer library. It allows you to run the privilege elevation exploit.

1. Launching the Browser:
     - The application launches a browser using the Playwright library.
     -  A new browser context and page are created.

2.  Navigating to the Gruyere Application:
     - The page navigates to the Gruyere application, which is the target for the exploit.

3.  Performing the Privilege Elevation Exploit:
     -  The 'exploit_privilege_elevation' function is called, passing the page object.
     -  The function crafts a payload containing data for the exploit.
     -  HTTP requests are sent to the Gruyere application to update the user's privileges.
     -  The function checks the response to determine if the privilege elevation was successful.

4.  Closing the Browser:
     -  After the exploit is performed, the browser is closed.

Privilege Elevation Exploit

The 'exploit_privilege_elevation' function contains the logic for the privilege elevation exploit.

 5.  Crafting the Payload:
      -  The function creates a payload containing data for the exploit, such as the attacker's account name, password, password confirmation, and desired   privilege level.

 6.  Sending HTTP Requests:
     -  HTTP requests are sent to the Gruyere application to update the user's privileges.
     -  The payload data is used to fill in the form fields.
     -  The form is submitted.

 7.  Checking the Response:
     -  The function checks the response to determine if the privilege elevation was successful.
     -  If the response contains the string "Account Details Saved," a success message is printed.

Test Case

The code includes a test case class called PrivilegeElevationTest that verifies the privilege elevation exploit.

  8.  Launching the Browser for Testing:
     -  A browser is launched using the Playwright library.
     -  A new context and page are created.

  9.  Navigating to the Gruyere Application:
     -  The page navigates to the Gruyere application.

  10.  Performing the Privilege Elevation Exploit:
     -  The exploit_privilege_elevation function is called to perform the exploit.

  11.   Closing the Browser:
     -  After the exploit is performed, the browser is closed.

Main Module

The code includes a check to determine if the script is being run as the main module. If so, the command-line application logic is executed.

Conclusion

This code demonstrates a privilege elevation exploit using the Playwright library. It showcases how to launch a browser, navigate to a target application, perform a privilege elevation exploit, and includes a test case for verification. Use this code responsibly and only on applications where you have proper authorization and consent.
    
