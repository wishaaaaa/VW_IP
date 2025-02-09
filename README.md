# VW_IP
IP
NP Mappy
Np Mappy is an app where students can simply login into this app to view the campus map. We realised how troublesome it was to keep opening chrome or other websites to check for the school map, so we decided that this was a good choice. Students just have to login and the home page will be an interactive map of the campus that allows them to zoom in and out of.

Other than the map, this app has features such as report map inaccuracies, calendar, announcements, and a profile page with their student card shown. This is different from other apps that NP already has because it is less tedious to navigate around due to lesser amount of features that the user can use, and that is the main goal of creating this app.

Design Process
We thought of creating an app for students to mainly check for the campus map as trying to search the campus map on google might be too much work. This app also allows students to check for the school calendar for important events to not miss out on them. An announcement page is also available for them to simply check for important announcements from school instead of having to scroll through their outlook to look at the flooding announcements. 

Here are some user stories that we paid attention to to help us with the creation of this app:
1. As an international student, I want to view resources and tips for adjusting to life on campus so that I feel less overwhelmed.	
2. As a new student, I want to organize my weekly timetable in the app so that I never miss a class or event.	
3. As a student, I want to be able to have an integrated calendar with notifications on school events, important announcements or deadlines.	
4. As a visitor, I want an easy-to-use map of the school to locate important places like the principal’s office or auditorium without requiring prior knowledge of the campus.	
5. As a new student, I want to receive reminders about upcoming deadlines or events so that I can stay on top of my responsibilities	


Features
For the home page, it just mainly features the school map and at the bottom there will be a function for "Report Map Inaccuracies" where users are able to report issues about the map that they find.
The calendar page consists of the actual calendar with specific events being labelled on the dates and users are allowed to press on them to enlarge the notification. 
The announcement page consists of a series of announcements that shows the users the main name of the event or announcement shared, and the users can press on view more to view more details of the announcement.
The profile page shows the student's id card where it displays their name student id and course. there is also a terms of use button and a contact us section where students can type in their messages and press submit.It will then lead them to a Thank you page.

Features Left to Implement
I feel that I could implement more interactive and gamification features into the website app and make it more fun for users to use.

Technologies Used
I used Google Maps API to do up my map school map and put it in my code. I wasn't fully sure of how to do it so i used ChatGpt and Claude.Ai to help me out. I used these 2 because they both have a message limit and i needed extreme help. So i made use of these 2 to help me out and guide me along the way.
<!-- home.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NP Mappy</title>
    <link rel="stylesheet" href="styles.css">
    <link href="https://fonts.googleapis.com/css2?family=Inria+Serif&display=swap" rel="stylesheet">
    <script>
        function showTab(tabId) {
            document.querySelectorAll(".tab").forEach(tab => {
                tab.classList.remove("active");
            });
            document.getElementById(tabId).classList.add("active");
        }
    </script>
</head>
<body class="home-page">
    <header>
        <h1 class="logo">NP Mappy</h1>
    </header>
    
    <main id="content">
        <div id="home" class="tab active">Campus Map Here</div>
        <div id="calendar" class="tab">School Calendar</div>
        <div id="announcements" class="tab">Important Announcements</div>
        <div id="profile" class="tab">
            <p><a href="report.html">Report Map Inaccuracies</a></p>
            <p><a href="contact.html">Contact Us</a></p>
        </div>
    </main>
    
    <!-- Navigation Bar -->
    <nav>
        <button onclick="showTab('home')">Home</button>
        <button onclick="showTab('calendar')">Calendar</button>
        <button onclick="showTab('announcements')">Announcements</button>
        <button onclick="showTab('profile')">Profile</button>
    </nav>
</body>
</html>

Testing
For the contact form and report map inaccuracies form, they will require you to input your school email to make sure the response sent back to the user is being sent to their email. Failure to provide an actual school email would make the prompt of "Please enter valid email address" come out because the email address has to end with "@np.edu.sg". The user will also have to fill in the message box because a prompt of "Please fill out this field." will show.

Credits

Media
https://images.app.goo.gl/ifsb6vqqcyGaAPuP9
Acknowledgements
I received inspiration for this project from NP GO
