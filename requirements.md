# From Jen 06062019

CPSC 4430 Software Engineering

    This class is for Junior CS students (no cyber students, but a few computer engineering students tend to take the class).  The students should be mostly strong programmers, able to pick up a new language (with some help/instruction -- I typically spend the first 1-2 weeks in a class like this teaching the language for the course).  
        There will be some seniors in it this year, since it was not taught last year.  You and I should probably try to coordinate large project due-dates, since we will have a good number of students who are in both CPSC 4430 and CPSC 4950 Capstone.
    This class was last taught 2 years ago, by me, using the textbook: "Engineering Software as a Service:  An Agile Approach using Cloud Computing" by Armando Fox and David Patterson.  Kindle Edition, May 2016. 
        We used Ruby on Rails as a language/platform.  With 6 students in the class, we developed this app: http://que-bien-suena.herokuapp.com/pages/home
        I adapted the lecture notes from the book (which were pretty awful, in my opinion), and have a full set of homework/labs/projects/exams etc, which I can share with you. I'm never satisfied with how I teach a course the first time, and so there are things that I would change for next time, and I always write down notes on what worked and what didn't and what to change, so if you're interested in using that book, then I can share my thoughts.
        I think if I did it again, I'd have the language be javascript-based.  The job market for Ruby programmers is small compared to javascript.  I'm not sure if I'd switch the textbook, though.  All of these students will have had Data Structures, and in that class I use a textbook that has Java language examples, but we use C++ in the class.  
        I'm not sure I have much advice for a textbook for this class, though I'm happy to talk through questions that you have about book's you've found.  I could see the class being based on several readings (like a short agile book, an article comparing agile to waterfall, articles on other things)... that is more work for the instructor, though.
        Again, you can choose any language / platform / book that you wish, within reason.
    We changed the curriculum for this year to be a 4 credit hour class (with a designated lab section), and to include security topics.  Again, about 1/4th of the time should be devoted to talking about security topics relevant to software engineering.  Topics are listed below in the ACM recommendations.
    An important part of this class is working in Agile groups to create a larger software project, which should be a SaaS style project, since SaaS is so prevalent today, and doesn't really fit neatly into any of our other courses.  A significant portion of class time can be used for student work on the project.
        A class of 6 (which I had) will be very different than a class of 15 (which you have).  One of the things that I was thinking of changing was the group size ... I was thinking of doing groups of 3 in this class, to get better student participation and accountability...but that means 5 different projects to supervise.  (I do have a number of possible non-profit projects that you could have the students work on -- more in another email.  Most of them are very similar in structure.).  You can do whatever you want -- but I think that 5 different projects is pretty ambitious for the first semester of teaching!  If you want to try it, I can help support the projects with debugging, code reviews, pull request approvals, etc.  This is totally your decision.
    Testing should be used in this class.  The students will have written unit tests before, but have not done any integration testing, and don't know about TDD or BDD, or CI, all of which are important in the industry, especially in our "friends of the department" companies like Genesys and Ontario Systems and Salesforce.  
        When I taught this class, we started trying to do TDD/BDD, but I didn't know enough about rspec and cucumber to keep up with writing tests ... 
        If I taught this again, I think I'd write the tests for the students for most of the class time, and then have a homework/lab or two for them to write a test later in the semester.  Maybe.... if I was supervising 5 projects, I'm not sure I'd have time to write very detailed tests....
        We do CI in capstone, and try to do TDD/BDD as well (I didn't have success in doing BDD/TDD last year in Capstone either, but I'm going to try again this year!).
    In other classes, the students primarily use GitHub for source code management, since our university (free) account has unlimited private repos.  Last year, I created issues in GitHub and we sorta used that for our sprint tracking, but it's not great. We have unlimited licenses in PivotalTracker, if you want to use that ... I don't like it as much as I like Bitbucket/Jira, though.  Jira is $10 for 10 people ... and if you want more than 10 from an organization, it's $400 (yikes!).  However, if we stand up our own Jira server, we have a completely open/free license for as many people as we want.  I'm thinking we may want to go down that track.  What do you think?


ACM Curriculum recommendations

The ACM curriculum recommendations are found here.
https://www.acm.org/binaries/content/assets/education/cs2013_web_final.pdf . This is a crazy-long document that I don't think you need to read!  You can just go to the pages listed below.  The main idea is that they break each topic down in to three levels:

    Tier1:  we need to cover nearly 100% of topics somewhere in the CS curriculum
    Tier2:  our goal is to cover 70-80% of the topics in this tier, usually in Junior/Senior level courses
    Electives:  curriculum should offer a variety of elective topics.

When they say "1 hour" they mean that a typical instructor could cover the material listed in that section in 1 hour -- note that when they list a topic, they are really talking about teaching the basics about it, not going super in depth, and not expecting a student to fully understand every aspect of that topic.  This is undergrad, after all, so they should recognize the terms, and understand what they are talking about, but not necessarily be able to prove/code/apply every single item.  Of course, we want our students to be able to code/apply the most important things, and we can choose what we think those are. 

Also, some of the topics in these sections may fit better into other courses, and that is just fine.  After you teach the class the first time, you can look at ended up being not covered, and we can talk about *if* we should cover that topic, and *where* it would most naturally fit.

----

CPSC 4430
* Some of these topics are also covered in CPSC 4950/4960 at the applied level.  Things that you think more properly belong in a 2nd software engineering class (which is basically what Capstone is), we can move to that class, either this year or next year.
* Some of the IAS security topics are also taught in other classes, including data structures and the cryptography/security class, but usually not very in depth.  That is why we increased this class by 1 credit hour, so we can cover these better.
SE/Software Processes, page 175
SE/Software Project Management, page 176
SE/Tools and Environments, page 178
SE/Requirements Engineering, page 178
SE/Software Design, page 180
SE/Software Construction, page 181
SE/Software Verification and Validation, page 182
SE/Software Evolution, page 183
SE/Software Reliability, page 184
IAS/Principles of Secure Design, page 103
IAS/Defensive Programming, page 104
IAS/Web Security, page 108 (also cover some of this in 3380)
IAS/Secure Software Engineering, page 111
