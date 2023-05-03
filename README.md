Download Link: https://assignmentchef.com/product/solved-cs31-project-2-stimulus-check-calculator
<br>
<img decoding="async" alt="Who's Getting Checks" width="1202" height="273" data-src="./201A-COMSCI31-1_ Project 2_files/check.png" class="img-responsive atto_image_button_text-bottom lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" class="img-responsive atto_image_button_text-bottom" src="./201A-COMSCI31-1_ Project 2_files/check.png" alt="Who's Getting Checks" width="1202" height="273">

 </noscript>

<span class="">The payment amount falls by $5 for every $100 in income above the full payment level which is $75,000 for individual filers, $150,000 for married couple filers and $112,500 for head of household filers.</span>

<span class="">Here is an example of a dialog for the program I am asking you to create (user input is in </span><strong><span class="">boldface</span></strong><span class="">):</span>

<pre>What is your filing status? <b>Single</b><b></b>What is your adjusted gross income?<b> 50000</b>How many children under the age of 17 did you claim as a dependent?<strong> 0</strong><b></b>Your stimulus check is $1200.</pre>




<span class="">The following table shows the costs your program should work with:</span>

<table>

 <caption>

  Stimulus Check Parameters

 </caption>

 <thead>

  <tr>

   <th>Filing Status</th>

   <th scope="col">  Single</th>

   <th scope="col">        Married</th>

   <th scope="col"> Head of Household</th>

  </tr>

 </thead>

 <tbody>

  <tr>

   <td>Full Stimulus Payment</td>

   <td>$1,200</td>

   <td>$2,400</td>

   <td>$1,200</td>

  </tr>

  <tr>

   <td>Each Dependent Under 17 Increases Payment By:</td>

   <td colspan="3">additional $500</td>

  </tr>

  <tr>

   <td> Full Payment Up To Incomes Of:</td>

   <td>$75,000</td>

   <td>$150,000</td>

   <td>$112,500</td>

  </tr>

  <tr>

   <td> Payment Reduction</td>

   <td colspan="3">$5 reduction for each $100 in income above the Full Payment Limit</td>

  </tr>

 </tbody>

</table>










<span class="">Here’s a few other examples to give you a sense of how it should work: </span>




<pre></pre>

<pre>What is your filing status? <b>Head of Household</b><b></b>What is your adjusted gross income?<b> 200000</b>How many children under the age of 17 did you claim as a dependent?<strong> 0</strong><b></b>Your stimulus check is $0.</pre>










<pre>What is your filing status?<b> Color Television</b><b></b>What is your adjusted gross income?<b> 0</b>How many children under the age of 17 did you claim as a dependent?<strong> 0</strong><b></b>Error - Invalid filing status.</pre>







<pre>What is your filing status? <b>Married</b><b></b>What is your adjusted gross income?<b> 200000</b>How many children under the age of 17 did you claim as a dependent?<strong> 1</strong><b></b>Your stimulus check is $400.</pre>

<span class="">You can test your understanding of the cost requirements by experimenting with the calculator we found at </span><a href="http://www.howardstahl.com/ucla/summer20/project2"><span class="">this website</span></a> <span class="">.</span>




<span class="">Your program must collect the information for one taxpayer in the manner indicated by the examples, and then write to </span><code><span class="">cout</span></code><span class=""> exactly one line in a format required below. Our grading tool will judge the correctness of your program by examining your output . That line you write must be in one of the following <del>seven</del> <u>four</u> forms; the text must be </span><strong><span class="">identical</span></strong> <span class="">to what is shown (except that the italicized </span><i><span class="">cccc </span></i><span class="">should be the appropriate numeric value calculated by your program:</span>

<ul>

 <li><span class="">If the user enters a filing status value which is not “Single”, “Married” or “Head of Household”:</span><span class="">   Error – Invalid filing status.</span></li>

 <li><span class="">If the user enters an income less than zero:</span><span class="">Error – Invalid income.</span></li>

 <li><span class="">If the user enters a number of children less than zero:   </span><span class="">   Error – Invalid number of dependents.</span></li>

 <li><span class="">Otherwise: </span><span class="">   Your stimulus check is $cccc.</span></li>

</ul>

<span class="">The lines you write must not start with any spaces. If you are not a good speller or typist, or if English is not your first language, be especially careful about duplicating the messages </span><strong><span class="">exactly</span></strong> <span class="">. Here are some foolish mistakes that may cause you to get no points for correctness on this project, no matter how much time you put into it:</span>

<ul>

 <li><span class="">Writing any extra spaces on the output line.</span></li>

 <li><span class="">Writing more than one line of output. Don’t, for example, add a gratuitous “Thank you for using my great stimulus calculator!”</span></li>

 <li><span class="">Writing lines to </span><code><span class="">cerr</span></code><span class=""> instead of </span><code><span class="">cout</span></code> <span class="">.</span></li>

 <li><span class="">Writing lines like these:</span><span class="">Your stimulus check is $1200                </span><em><span class="">missing period</span></em><span class="">Yyour stilmus check is $1200.               </span><em><span class="">misspelling</span></em><span class="">YOUR STIMULUS CHECK IS $1200.               </span><em><span class="">wrong capitalization</span></em><span class="">Your stimulus check is $1200  .             </span><em><span class="">extra spaces</span></em><span class="">Your stimulus check is $1,200.00            </span><em><span class="">incorrect number format</span></em></li>

</ul>

<span class="">Your program must gather the filing status, the income level and the number of dependents, in that specific order. However, if you detect an error in an item, you do not have to request or get the remaining items if you don’t want to; just be sure you write to </span><code><span class="">cout</span></code> <span class="">the required error message and nothing more after that. If instead you choose to gather all input first before checking for any errors, and you detect more than one error, then write only the error message for the first erroneous input item.</span>

<span class="">You will not write any loops in this program. This means that each time you run the program, it handles only one check calculation. It also means that in the case of bad input, you </span><b><span class="">must not</span></b> <span class="">keep prompting the user until you get something acceptable; our grading tool will not recognize that you’re doing that.</span>

<span class="">Additionally, I have created a testing tool called CodeBoard to help you check your code.  CodeBoard enables you to be sure you are naming things correctly by running a small number of tests against your code.  Passing CodeBoard tests is not sufficient testing so please do additional testing yourself.  To access CodeBoard for Project 2, please click the link you see in this week named <b>CodeBoard for Project 2</b>.  Inside the file named user_functions.cpp, copy and paste the body of your main( ) function inside the function named student_main( ) .  CodeBoard uses its own main( ) to run tests against your code.  Click Compile and Run.  However please be aware that no editing changes can be saved inside CodeBoard.  In this anonymous user configuration, CodeBoard is read-only and does not allow for saving changes.</span>

<span class="">The correctness of your program must not depend on undefined program behavior. Your program could not, for example, assume anything about </span><code><span class="">n</span></code> <span class="">‘s value at the point indicated:</span>

<pre>int main(){int n;int m = 42 * n;  // n's value is undefined…</pre>

<span class="">What you will turn in for this assignment is a zip file containing these three files and nothing more:</span>

<ol>

 <li><span class="">A text file named </span><strong><span class="">stimulus.cpp</span></strong> <span class="">that contains the source code for your C++ program. Your source code should have helpful comments that tell the purpose of the major program segments and explain any tricky code.</span></li>

 <li><span class="">A file named </span><strong><span class="">report.doc</span></strong><span class=""> or </span><strong><span class="">report.docx</span></strong><span class=""> (in Microsoft Word format) or </span><strong><span class="">report.txt</span></strong><span class=""> (an ordinary text file) that contains in addition </span><b><span class="">your name</span></b> <span class="">and </span><b><span class="">your UCLA Id Number</span></b><span class="">:</span>

  <ol>

   <li><span class="">A brief description of notable obstacles you overcame. (In Project 1, for example, some people had the problem of figuring out how to work with more than one version of a program in Visual C++.)</span></li>

   <li><span class="">A list of the test data that could be used to thoroughly test your program, along with the reason for each test. You don’t have to include the results of the tests, but you must note which test cases your program does not handle correctly. (This could happen if you didn’t have time to write a complete solution, or if you ran out of time while still debugging a supposedly complete solution.) For Project 1, for example, such a list, had it been required, might have started off like this:</span>

    <dl>

     <dt></dt>

     <dd></dd>

     <dd>

      <span class="">Negative number of tests (-1000, 1, 2, 3, 4)</span>

     </dd>

     <dt></dt>

     <dd>

      <span class="">Negative number of positives (1, -413, 2, 3, 4)</span>

     </dd>

     <dd>

      <span class="">Negative number of false positives (1, 2, -10, 3, 4)</span>

     </dd>

     <dt></dt>

     <dd>

      <span class="">All zeros  (0, 0, 0, 0, 0)</span>

     </dd>

     <dt></dt>

     <dd>

      <span class="">Equal numbers (200, 200, 200, 200, 200)</span>

     </dd>

     <dt></dt>

     <dd>

      <span class="">…</span>

     </dd>

    </dl></li>

  </ol></li>

 <li><a name="hw"></a><span class="">A file named </span><strong><span class="">hw.doc</span></strong><span class=""> or </span><strong><span class="">hw.docx</span></strong> <span class="">(in Microsoft Word format) or </span><strong><span class="">hw.txt</span></strong><span class=""> (an ordinary text file) that contains your solution to the </span><a href="https://ccle.ucla.edu/mod/page/view.php?id=2992606"><span class="">homework</span></a><span class=""> accompanying Project 2.</span></li>

</ol>

<span class="">By July 6, there will be a link on the class webpage that will enable you </span><span class="">to turn in your zip file electronically. Turn in the file by the due time above. Give yourself enough time to be sure you can turn something in, because we will not accept excuses like “My network connection at home was down, and I didn’t have a way to copy my files and bring them to a SEASnet machine.” There’s a lot to be said for turning in a preliminary version of your program, report, and homework early (You can always overwrite it with a later submission). That way you have something submitted in case there’s a problem later. Notice that most of the test data portion of your report can be written from the requirements in this specification, before you even start designing your program.</span>

<span class="">The writeup </span><a href="https://ccle.ucla.edu/mod/page/view.php?id=2992605"><span class="">Some Things about Strings</span></a><span class=""> tells you what you need to know about strings for this project.</span>

<span class="">As you develop your program, periodically try it out under another compiler (g++ if you’re doing your primary development using Visual C++, or Visual C++ if you’re doing your primary development using clang++ or g++ (e.g., with Xcode on a Mac)). Sometimes one compiler will warn you about something that another is silent about, so you may be able to find and fix more errors sooner. If running your program under both environments with the same input gives you different results, your program is probably relying on undefined behavior (such as using the value of an uninitialized variable), which we prohibit.</span>

<h4><b><span class="">G31 Build Commands</span></b></h4>

<span class="">g31 -c stimulus.cpp</span><span class="">g31 -o runnable stimulus.o</span><span class="">./runnable</span>

<span class="kksr-muted">Rate this product</span>


