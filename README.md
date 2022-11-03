Tasks to answer in your own README.md that you submit on Canvas:

1.  See logger.log, why is it different from the log to console?
<br />
-The console Log logs all system details, logger.log is user made log statements
<br />
2.  Where does this line come from? FINER org.junit.jupiter.engine.execution.ConditionEvaluator logResult Evaluation of condition [org.junit.jupiter.engine.extension.DisabledCondition] resulted in: ConditionEvaluationResult [enabled = true, reason = '@Disabled is not present']
<br />
-This comes from logger.log, which checks if test is enabled or disable
<br />
3.  What does Assertions.assertThrows do?
<br />
-Assert throws confirms the type of exception when a error happens
<br />
4.  See TimerException and there are 3 questions
<br />
    1.  What is serialVersionUID and why do we need it? (please read on Internet)
    <br />
    -The serialUID is used to guarantee the same class is loaded across different systems
    <br />
    2.  Why do we need to override constructors?
    <br />
    -So we can write different messages with throwable objects
    <br />
    3.  Why we did not override other Exception methods?	
    <br />
    -We did not need to use them as extensively
    <br />
5.  The Timer.java has a static block static {}, what does it do? (determine when called by debugger)
<br />
-It only runs the first time the program loads memory, for initilization
<br />
6.  What is README.md file format how is it related to bitbucket? (https://confluence.atlassian.com/bitbucketserver/markdown-syntax-guide-776639995.html)
<br />
-The format is markdown, bitbucket has some markdown integration and will display a .md file named README.
<br />
7.  Why is the test failing? what do we need to change in Timer? (fix that all tests pass and describe the issue)
<br />
-Needed to initialize time to current system time, otherwise it would be null which triggers throw condition
<br />
8.  What is the actual issue here, what is the sequence of Exceptions and handlers (debug)
<br />
-The issue is that we are checking if currentTimeMillis is null before calling the function itself, we need to run the functions we want to check first
<br />
9.  Make a printScreen of your eclipse JUnit5 plugin run (JUnit window at the bottom panel) 
<br />
-Got Test Results in PDF
<br />
10.  Make a printScreen of your eclipse Maven test run, with console
<br />
-Got printScreen in PDF
<br />
11.  What category of Exceptions is TimerException and what is NullPointerException
<br />
-NullPointerException is unchecked, TimerException is checked
<br />
12.  Push the updated/fixed source code to your own repository.
<br />
-Already in my own Repo.
