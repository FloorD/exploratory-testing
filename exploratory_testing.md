###Exploratory testing

Software is full of surprises. No matter how careful or skilled you are, when you create software it can behave differently than you intended. Exploratory testing mitigates those risks.

At a previous company, users could list a homepage on their profile page. One tech-savvy punk got the idea of listing my the company's url there. Naturally, ourcompany.com would now redirect to his profile page. Brilliant.

Dora the explorer
Observing things like datestamps from a (far) past
Recognizing variables and testing them

If all the tests are passing, I’m done. Right?

Exploratory testing is an approach to software testing that is concisely described as simultaneous learning, test design and test execution. Cem Kaner, who coined the term in 1983,[1] now defines exploratory testing as "a style of software testing that emphasizes the personal freedom and responsibility of the individual tester to continually optimize the quality of his/her work by treating test-related learning, test design, test execution, and test result interpretation as mutually supportive activities that run in parallel throughout the project."[2]

While the software is being tested, the tester learns things that together with experience and creativity generates new good tests to run. Exploratory testing is often thought of as a black box testing technique. Instead, those who have studied it consider it a test approach that can be applied to any test technique, at any stage in the development process. The key is not the test technique nor the item being tested or reviewed; the key is the cognitive engagement of the tester, and the tester's responsibility for managing his or her time.[
Exploratory testing has always been performed by skilled testers. In the early 1990s, ad hoc was too often synonymous with sloppy and careless work. As a result, a group of test methodologists (now calling themselves the Context-Driven School]) began using the term "exploratory" seeking to emphasize the dominant thought process involved in unscripted testing, and to begin to develop the practice into a teachable discipline. This new terminology was first published by Cem Kaner in his book Testing Computer Software[1] and expanded upon in Lessons Learned in Software Testing.[4] Exploratory testing can be as disciplined as any other intellectual activity.

Though the current trend in testing is to push for automation, exploratory testing is a new way of thinking. Automation has its limits

Directed from requirements and exploring during testing  
Determination of test cases during testing  
Investigation of system or application  
Emphasizes on adaptability and learning  
Involves Investigation  
Is about Improvement of test design  
Like making a conversion – its spontaneous  
The tester’s mind is in control  


Is not random testing but it is adhoc testing with purpose of find bugs  
Is structured and rigorous  
Is cognitively (thinking) structured as compared to procedural structure of scripted testing. This structure comes from Charter, time boxing etc.  
Is highly teachable and manageable  
Is not a technique but it is an approach. What actions you perform next is governed by what you are doing currently  


This testing purely depends on the tester skills
Limited by domain knowledge of the tester
Not suitable for Long execution time

Learning to use the application or software system is a challenge
Replication of failure is difficult
Determining whether tools need to be used can be challenging
Determine the best test cases to execute can be difficult
Reporting of the test results is challenge as report doesn’t have planned scripts or cases to compare with the actual result or outcome
Documentation of all events during execution is difficult to record
Don’t know when to stop the testing as exploratory testing has definite test cases to execute.

#####Exploratory Test Preparation
**Create a Bug Taxonomy (classification )**  
        Categorize common types of faults found in the past projects  
        Analyze the root cause analysis of the problems or faults  
        Find the risks and develop ideas to test the application.  
**Test Charter**  
        Test Charter should suggest  
            - what to test  
            - how it can be tested  
            - What needs to be looked  
        Test ideas are the starting point of exploration testing  
        Test charter helps determine how the end user could use the system  
**Time Box**  
        This method includes pair of testers working together not less than 90 minutes  
        There should not be any interrupted time in those 90 minutes session  
        Time box can be extended or reduced by 45 minutes  
        This session encourages testers to react on the response from the system and prepare for the correct outcome  
**Review Results:**  
        Evaluation of the defects  
        Learning from the testing  
        Analysis of coverage areas  
**Debriefing:**  
        Compilation of the output results  
        Compare the results with the charter  
        Check whether any additional testing is needed  

 

**During exploratory execution, following needs to be done:**

Mission of testing should be very clear  
Keep notes on what needs to be tested, why it needs to be tested and the assessment of the product quality  
Tracking of questions and issues raised during exploratory testing  
Better to pair up the testers for effective testing  
The more we test, more likely to execute right test cases for the required scenarios  
 
 

**It is very important to take document and monitor the following**

Test Coverage – Whether we have taken notes on the coverage of test cases and improve the quality of the software  
    - Risks – Which risks needs to be covered and which are all important ones?  
    - Test Execution Log – Recordings on the test execution  
    - Issues / Queries – Take notes on the question and issues on the system  

Smarter exploratory testing finds more errors in less time.  


Exploratory testing seeks to find out how the software actually works, and to ask questions about how it will handle difficult and easy cases. its antithesis scripted testing. In this activity test cases are designed in advance. This includes both the individual steps and the expected results. These tests are later performed by a tester who compares the actual result with the expected. When performing exploratory testing, expectations are open. According to Cem Kaner & James Marcus Bach, exploratory testing is more a mindset or "...a way of thinking about testing" than a methodology.  Test cases are not created in advance but testers check system on the fly. They may note down ideas about what to test before test execution. The focus of exploratory testing is more on testing as a “thinking” activity.

#####ET
[111 RR Book Club][1]: Explore It! with [Elisabeth Hendrickson][2]

"I consider the separation of QA from software development to be one of the worst wrong turns that our industry has made because it led to incredibly long feedback cycles."

"It is a practice of simultaneously designing little tests and running those little experiments to learn how the software behaves and using your observations about how the software behaves to design your next little tests all to steer towards the risks in your software. So, rather than confirming that it does what you intended it to do, discover ways in which it violates expectations or does really bad things."

"A specification is a very literal ‘this is exactly what I want the software to do’ with no why at all." It's not what you expect to happen, let alone why. David Hussman - Dude’s Law: the less why you have, the worse your stuff is or the worse value you’ve got.

I click a button and I know what’s going on in the background and I know it takes a little bit of time. So, I would never dream of trying to hit refresh or back or something in the middle of hitting that button because I’m like, “Okay. Now, it’s doing its thing and I’m going to wait until it’s done its thing.” And then it’ll be done. And then I’ll check the outcome. 
 you’re more likely to find the things that users are going to actually experience rather than thinking, “Okay. Well, I know that the controller is going to go make the AJAX request and da…da…da…and I’ll just wait until everything’s back,” 

#####TDD
Test-driven development (TDD) is a software development process that relies on the repetition of a very short development cycle: first the developer writes an (initially failing) automated test case that defines a desired improvement or new function, then produces the minimum amount of code to pass that test, and finally refactors the new code to acceptable standards.
And of course you crazy German speaking people have your own word for it: Testgetriebene Entwicklung.

#####Tools
irb / Rails console
Firebug
Chrome’s Developer Mode
JavaScript Console
[Fiddler][5] - a HTTP proxy so that you could get in there and start sending your POST requests.
all kinds of developer debugging tools 

[1]: http://rubyrogues.com/111-rr-book-club-explore-it-with-elisabeth-hendrickson/
[2]: https://twitter.com/testobsessed
[3]: http://testobsessed.com/
[4]: http://pragprog.com/book/ehxta/explore-it
[5]: http://fiddler2.com/