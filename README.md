Hello,
I attempted ready-to-go version of project to import here:
https://github.com/kamil-wasikowski/Netguru.git
But I'm not sure if it's going to work becouse I never deal with this before. 

Here is step by step instruction how to configure my automated test:
1. Download InteliiJ SE here:
https://www.jetbrains.com/idea/download/download-thanks.html?platform=windows&code=IIC
2. Download and install Firefox browser:
https://www.mozilla.org/
3. Download Firefox WebDriver here:
https://github.com/mozilla/geckodriver/releases
4. Download Java librarys here:
https://drive.google.com/open?id=1G9TV9714Uyo5h2Y9zLJmIfOfEzDx8oko
5. Download project for import here:
https://drive.google.com/file/d/1XglUIo_R5JK4C5IutJE6dEazXD5YUiV8/view
6. Create a Folder in your Desktop where you will keep Java, WebDriver and Project in seperate spaces 
7. Extract Project
8. Install IntelliJ with defoult setup
9. After installation, run IntelliJ
10. In "Welcome to IntelliJ IDEA" window, select Import Project with Maven
11. Pick extracted project and run import
12. Press Ctrl+Alt+Shift+S
13. Go to Modules and click on "+" icon
14. Pick "JARs or directories" and select folder with Java placed in Folder from Step #6
15. In "Netguru" project on the left side of a screen open: src > main > java paths
16. Drag and drop, from Folder in Desktop, Firefox WebDriver and put it into java folder in IntelliJ path
17. Right-click on geckodriver.exe and "Copy Path..." > "Absolute path"
18. Open "Login" Java Class
19. Paste Absolute path in second quote next to System.setProperty line so it look like this:
System.setProperty("webdriver.gecko.driver", "C:\\Users\\USER\\Desktop\\Netguru\\src\\main\\java\\geckodriver.exe");
20. IntelliJ will ask about importing Maven setup, let him import everything
21. Right-click on "Login.java" bookmark and select "Run 'Login.main()'
