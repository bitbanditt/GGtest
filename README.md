# GGtest

Google Gruyere Privilege Elevation Exploit

    Using the terminal pip is installed allowing for the istall of typer and playwright using 'pip install'
    
    The required libraries (requests, typer, unittest, and playwright.sync_api) are imported.

    A command-line application is defined using Typer. It includes a single command called exploit_privilege_elevation.

    Within the exploit_privilege_elevation function, a browser is launched using Playwright. A Chromium browser instance is created.

    A new browser context and page are created using the Playwright API.

    The page navigates to the Gruyere application, which is the target for the privilege elevation exploit.

    The exploit_privilege_elevation function is called, passing the page object.

    The function crafts a payload with data for the exploit, such as the attacker's account name, password, password confirmation, and desired privilege level.

    The function sends HTTP requests to the Gruyere application to update the user's privileges. It clicks on a link to the edit profile page, fills in the form fields with the payload data, and submits the form.

    The function checks the response to determine if the privilege elevation was successful. If the response text contains the string "Account Details Saved," a message indicating successful privilege elevation is printed.

    The code includes a test case class (PrivilegeElevationTest) that inherits from unittest.TestCase. It contains a test method called test_privilege_elevation to verify the exploit.

    Similar to the exploit_privilege_elevation function, the test method launches a browser, creates a new context and page, navigates to the Gruyere application, and calls the exploit_privilege_elevation function.

    Finally, the browser is closed.

    The code also checks if it is being run as the main module and executes the app() function, which handles the command-line application logic.
