# 🔍Analyzing Types of Web Application Attacks🌐

1\. Launch the DVL virtual machine.

2\. On the login screen, type root followed by pressing the Enter key.

3\. When prompted for a password, type toor and press Enter again.

4\. When presented with the user prompt, type startx and then press Enter.

<img src="./media/image1.png" style="width:3.60736in;height:0.8171in" />

5\. Once the graphical user interface appears, start the WebGoat web
server by clicking on the Application Menu and navigate through Damn
Vulnerable Linux \> Training Material \> Web Exploitation \> Webgoat \>
Start WebGoat port 80.

<img src="./media/image2.png"
style="width:5.85931in;height:2.14514in" />

6\. A new terminal window will appear, showing the WebGoat startup process. Leave this shell open and minimize it for now.

7\. Open the Firefox web browser by clicking on the icon located on the bottom taskbar.

<img src="./media/image3.png" style="width:2.60453in;height:0.43756in" />

8\. While in Firefox, type http://127.0.0.1/WebGoat/attack (case-sensitive) into the address field, followed by pressing the Enter
key.

9\. When prompted for authentication, type password. Click OK. guest as the username and guest as the Click OK.

<img src="./media/image4.png"
style="width:5.80289in;height:2.28157in" />

10\. Once authenticated, you are welcomed to the WebGoat Welcome page.
Click the Start WebGoat button.

<img src="./media/image5.png" style="width:7.50598in;height:5.3383in" />

11\. Once the page redirects, click on the Injection Flaws menu item
located on the left; this will open more options.

<img src="./media/image6.png" style="width:2.07939in;height:3.47556in" />

12\. Click on String SQL Injection.

<img src="./media/image7.png" style="width:2.05237in;height:3.00042in" />

13\. At the top-right of the webpage, click on Restart this Lesson.

<img src="./media/image8.png" style="width:5.66746in;height:3.2192in" />

14\. Type Smith into the Enter your last name text field and click on the Go! button.

<img src="./media/image9.png"
style="width:5.38617in;height:3.27129in" />

>Note that this is how the query is meant to be used . You type in an
>input and expect the proper output. In this case, we searched for users
>with the last name Smith and we received information from the database
>regarding all the Smiths.

<img src="./media/image10.png"
style="width:5.28199in;height:1.71899in" />

15\. Click on Restart this Lesson.

<img src="./media/image11.png"
style="width:5.58411in;height:1.83359in" />

16\. Inject the user_data database table with a popular injection
technique so that you can potentially leak all user information stored
in the table. Type the string below in the Enter your last name text
field.

17\. Click the Go! button.

<img src="./media/image12.png"
style="width:5.16739in;height:3.95889in" />

18\. After the successful inject, click on Stage 1: String SQL Injection
from the left menu.

<img src="./media/image13.png"
style="width:1.96902in;height:2.57328in" />

19\. You will be redirected to a Human Resource login page. Select Neville Bartholomew (admin) from the drop-down box. Attempt to login
without a password by pressing the Login button.

<img src="./media/image14.png"
style="width:3.74332in;height:2.66785in" />

20\. No access has been given. On the Firefox window, select Tools from the top menu and click on the Tamper Data tool.

<img src="./media/image15.png"
style="width:5.17781in;height:3.04209in" />

21\. A new Tamper Data application window will appear. Click the Start Tamper file menu option.

<img src="./media/image16.png"
style="width:3.23822in;height:3.40013in" />

22\. Change focus to the WebGoat web page. Select Neville Bartholomew (admin) once more from the user list and click the Login button.

<img src="./media/image17.png"
style="width:3.50097in;height:2.39233in" />

23\. Notice a new pop-up message from the Tamper Data tool appears. Click the Tamper button to proceed.

<img src="./media/image18.png"
style="width:4.30268in;height:1.33352in" />

24\. In the new Tamper Popup window, type the string field. Click OK. or 1=1-- into the password

<img src="./media/image19.png"
style="width:3.80066in;height:3.98293in" />

25\. Once the tool finishes its process, click Stop Tamper from the file
menu

<img src="./media/image20.png"
style="width:3.10008in;height:3.25431in" />

26\. Notice the successful SQL injection on the WebGoat web page. We now have access to the user database as the administrator. Select the first
user from the list; Larry Stooge and click the ViewProfile button.

<img src="./media/image21.png"
style="width:3.71856in;height:2.99437in" />

27\. Notice that we have complete control over all user profiles and complete access to their personal information.

<img src="./media/image22.png"
style="width:4.81317in;height:3.7401in" />

28\. Close the Firefox web browser.

**1.2 Using DVWA for SQL Injection**

1\. Launch the Kali virtual machine to access the graphical login
screen.

2\. Log in as root with toor as the password.

3\. Open a new terminal window by clicking on the terminal icon located
in the top toolbar.

<img src="./media/image23.png"
style="width:2.14613in;height:0.3438in" />

4\. Within the terminal, type the command below followed by pressing the
Enter key to list the currently active network interfaces on the system.

<img src="./media/image24.png"
style="width:6.27171in;height:1.69815in" />

5\. Bring the loopback interface to an active state.

<img src="./media/image25.png"
style="width:3.25045in;height:0.40631in" />

6\. Verify that the loopback interface is now up.

<img src="./media/image26.png"
style="width:6.39673in;height:3.30254in" />

7\. Start the mysql service by entering the command below.

<img src="./media/image27.png"
style="width:6.15711in;height:0.72927in" />

8\. Start the apache web service.

<img src="./media/image28.png"
style="width:6.98014in;height:0.73969in" />

9\. Open the Iceweasel web browser by clicking the on the web browser
icon located on the top menu pane.

<img src="./media/image29.png"
style="width:1.88568in;height:0.27087in" />

10\. In the address field, type http://127.0.0.1/dvwa/login.php. Press
Enter.

<img src="./media/image30.png"
style="width:5.19031in;height:4.13346in" />

11\. On the login page, type Login. admin for the username and password
for the password.

<img src="./media/image31.png"
style="width:4.55272in;height:3.7401in" />

12\. Click on the DVWA Security menu option located on the left.

<img src="./media/image32.png"
style="width:1.84401in;height:4.71941in" />

13\. Change the security level to low from the drop-down menu and click
Submit.

<img src="./media/image33.png"
style="width:3.77136in;height:2.04195in" />

14\. Confirm that the Security level is currently set to low.

<img src="./media/image34.png"
style="width:3.36505in;height:2.09404in" />

15\. Click on SQL Injection from the left menu.

<img src="./media/image35.png"
style="width:1.69815in;height:2.59411in" />

16\. Type in the number zero 0in the User ID: text field and click
Submit.

<img src="./media/image36.png"
style="width:6.87596in;height:1.33352in" />

17\. Notice no output is given. Type in the number one click Submit. 1in
the User ID: text field and CLICK SUBMIT

<img src="./media/image37.png"
style="width:6.58425in;height:1.2085in" />

18\. Attempt to use the “always true” SQL injection technique by typing
the string below into the User ID field.

<img src="./media/image38.png"
style="width:6.52174in;height:2.03153in" />

19\. Now you can see the account names in the database. Verify that you
can see all five accounts.

<img src="./media/image39.png"
style="width:4.42528in;height:2.8302in" />

20\. Type another string in the User ID: field to query the version of
the database.

<img src="./media/image40.png"
style="width:3.81337in;height:2.4305in" />

21\. Take note of the mysql database version that is given to us.

<img src="./media/image41.png"
style="width:5.09684in;height:3.65643in" />

22\. Type another string in the User ID: field to query the database
name. Click Submit.

<img src="./media/image42.png"
style="width:4.68736in;height:3.33975in" />

23\. Take note of the mysql database name that is given to us.

<img src="./media/image43.png"
style="width:4.53183in;height:3.29459in" />

24\. Type another string in the User ID: field to query for all tables
in the information_schema database.

<img src="./media/image44.png"
style="width:4.44539in;height:3.2004in" />

25\. Take note of all the different table information next to Surname.
The information_database stores information about all the databases that
the mysql server maintains.

<img src="./media/image45.png"
style="width:5.01275in;height:2.81701in" />

26\. Type another string in the User ID: field to query for all column
content in the user table.

<img src="./media/image46.png"
style="width:6.40714in;height:1.16683in" />

27\. Notice the amount of the user information given to us along with
their respective credentials.

<img src="./media/image47.png"
style="width:7.00098in;height:4.66732in" />

28\. Leave the DVWA web page open for the next task.

## 2\. Cross Site Scripting XSS

2.1 Using DVWA for XSS

1\. While on the DVWA web page, click on XSS stored from the left menu
pane

<img src="./media/image48.png"
style="width:1.77108in;height:2.65662in" />

2\. On this page, you are presented with a form that is mimicking a
comment section where users can write their comments. Make a test XSS
exploit by typing XSS1 in the Name text field. Type the script below
into the Message text field. Click the Sign Guestbook button.

<img src="./media/image49.png"
style="width:6.60509in;height:1.97944in" />

3\. Notice the popup message showing the same text you have inputted
between the quotations. With this vulnerability, every time a user views
this page they will experience the XSS exploit just as it shows now.
Click OK.

<img src="./media/image50.png"
style="width:2.88582in;height:1.75024in" />

4\. Click on the Setup menu option located to the left.

<img src="./media/image51.png"
style="width:1.76066in;height:1.72941in" />

5\. Once redirected, click on the Create / Reset Database button.

<img src="./media/image52.png"
style="width:6.37589in;height:1.93777in" />

6\. Click on the XSS Stored menu option.

<img src="./media/image53.png"
style="width:1.79192in;height:1.3231in" />

7\. For the Name, type Sign Guestbook. iframe1. Type the script below
into the Message field. Click on

<img src="./media/image54.png"
style="width:6.79261in;height:1.96902in" />

8\. Scroll down and notice the iframe presented on the screen. You
should see Kali’s homepage within the iframe.

<img src="./media/image55.png"
style="width:3.41714in;height:2.20864in" />

9\. Click on the Setup menu option.

<img src="./media/image56.png"
style="width:1.88568in;height:1.00014in" />

10\. Once redirected, click on the Create / Reset Database button.

<img src="./media/image57.png"
style="width:4.85484in;height:1.96902in" />

11\. Click on the XSS Stored menu option.

<img src="./media/image58.png"
style="width:1.76066in;height:1.39603in" />

12\. For the name, type Sign Guestbook. cookie1. Type the script below
into the Message field. Click on Sign Guestbook

<img src="./media/image59.png" style="width:6.553in;height:1.84401in" />

13\. A pop-up alert appears showing the user’s cookie information. In
this case, it is your cookie information. This script can be modified in
a way where if a malicious attacker may decide to forward cookie
information to a remote server and use man in-the-middle techniques to
steal personal information on a banking website for example. Click OK.

<img src="./media/image60.png"
style="width:4.63606in;height:1.75024in" />

14\. The lab is now complete; you may end the reservation.
