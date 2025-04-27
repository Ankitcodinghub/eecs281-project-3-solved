# eecs281-project-3-solved
**TO GET THIS SOLUTION VISIT:** [EECS281 Project 3 Solved](https://www.ankitcodinghub.com/product/eecs281-solved-3/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;122054&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;5&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (5 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;EECS281 Project 3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (5 votes)    </div>
    </div>
A relational database is the most common means of data storage and retrieval in the modern age. A relational database model stores data into one or more tables, where each table has columns and rows. The columns represent a value that can be attributed to an entry (such as color ,

name , or ID ) and the rows represent individual entries or records (such as Paoletti , my_cat ,

However, a database can do much more than simply store information. You must be able to retrieve specific information in an efficient manner. For relational databases, the structured query language (SQL) is a defined method of retrieving information programmatically. It looks like real English, where a valid command for the above table could be:

SELECT Model from Cars marketplace where Price &lt; 30000 which would return a list of models:

Note that the version of SQL used in this project is simplified and modified somewhat from a typical query language.

For this project, you will write a program to emulate a basic relational database with an interface based on a subset of a standard query language. Your executable will be called silly . You will gain experience writing code that makes use of multiple interacting data structures. The design portion of this project is significant; spend time thinking about what data structures you will use and how they will interact.

Learning Goals

Selecting appropriate data structures for a given problem. Now that you know how to use various abstract data types, itʼs important that you are able to evaluate which will be the optimal for a set of tasks.

Evaluating the runtime and storage tradeoffs for storing and accessing data contained in multiple data structures.

Designing a range of algorithms to handle different situations. Evaluating different representations of the same data.

Command Line Arguments

silly should accept the following (both optional) command line arguments:

-h , –help

This causes the program to print a helpful message about how to use the program and then immediately exit(0) .

-q , –quiet

Database Shell

Your program will create a shell that allows users to interact with a single database that is created in memory and destroyed when the program is quit by the user. A shell is a program that presents a prompt (“% “) to allow a user to enter commands and also view displayed output while interacting with the system. Since the commands to the shell come from standard input ( cin ) and display to standard output ( cout ), the program will be useable both directly from the keyboard locally and via redirected input ( &lt; ) and output ( &gt; ) locally and on the autograder.

Each command is specified by a keyword followed by a required space character ( ) and then the command-specific arguments where applicable. Like other database languages, some commands use additional required words that help make them more readable. These words can be both guaranteed to appear and completely ignored. For example, the command to delete rows from a table uses the keyword DELETE and adds FROM , for improved readability/pronuciation. So to delete the rows from table1 where the entries in column name equal John , the correct command would be:

Spec Example contains an example program illustrating the use of all the commands.

Database Commands

These commands affect the structure of the database and the running of the command shell. They include the creation and removal of tables, but do not deal with any actual data (items of type string , double , int or bool ).

CREATE

Add a new table to the database:

CREATE Syntax

CREATE &lt;tablename&gt; &lt;N&gt; &lt;coltype1&gt; &lt;coltype2&gt; … &lt;coltypeN&gt; &lt;colname1&gt; &lt;colname2&gt; … &lt;colnameN&gt;

Creates a new table with N columns (where N &gt; 0). Each column contains data of type

&lt;coltype&gt; and is accessed with the name &lt;colname&gt; . Table names and column names are guaranteed to be space-free. No two columns in the same table will have the same name (you do not need to check). Valid data types for coltype are {double, int, bool, string} . This table is initially empty.

CREATE Output

Print the following on a single line followed by a newline:

New table &lt;tablename&gt; with column(s) &lt;colname1&gt; &lt;colname2&gt; … &lt;colnameN&gt; created

CREATE: Possible errors

. A table named &lt;tablename&gt; already exists in the database

See Errors and Error Messages for acceptable output formats.

Given the following as input:

CREATE 281class 3 string string bool emotion person Y/N The output should be:

New table 281class with column(s) emotion person Y/N created

QUIT

Exit the program and delete all data in the database.

QUIT Syntax

Cleans up all internal data (i.e. no memory leaks) and exits the program. Note that the program must exit with a return 0 from main() .

QUIT Output

Print a goodbye message, followed by a newline.

QUIT: Possible errors

None, except for lacking a QUIT command. Every interactive session or redirected input file should end with a QUIT command.

# (comment)

Used to add comments to command files, produces no actions or output.

# Syntax

# Any text on a line that begins with # is ignored

Discard any lines beginning with #. This command does not produce any output nor can it generate any errors.

#: Possible errors

None.

REMOVE

Remove existing table from the database, deleting all data in the table and its definition.

REMOVE Syntax

Removes the table specified by &lt;tablename&gt; and all associated data from the database, including any created index.

REMOVE Output

Print a confirmation of table deletion, followed by a newline, as follows:

REMOVE: Possible errors

. &lt;tablename&gt; is not the name of a table in the database See Errors and Error Messages for acceptable output formats.

Given the following as input:

The output should be:

Table Commands

These commands work on one or more tables and are responsible for interacting with actual data, including insertion, deletion, printing, and indexing.

INSERT

Insert new rows at the end (append) of the specified table.

INSERT Syntax

Inserts &lt;N&gt; new rows into the table specified by tablename . The first line of the command specifies the tablename and the number of rows, N &gt; 0 , to be inserted. The next N lines specify the values to be inserted into the table. Each line contains M values, where M is guaranteed to be equal to the number of columns in the table. The first value, &lt;value11&gt; , should

be inserted into the first column of the table in the first inserted row, the second value,

&lt;value12&gt; , into the second column of the table in the first inserted row, and so on. Additionally, the types of the values are guaranteed to be the same as the types of the columns they are inserted into. For example, if the second column of the table contains integers, &lt;value12&gt; is guaranteed to be an int . Further, string items are guaranteed to be a single string of whitespace delimited characters (i.e. foo bar is invalid, but foo_bar is acceptable).

INSERT Output

Print the message shown below, followed by a newline, where &lt;N&gt; is the number of rows inserted, &lt;startN&gt; is the index of the first row added in the table, and &lt;endN&gt; is the index of the last row added to the table, 0 based. So, if there were K rows in the table prior to insertion, &lt;startN&gt; = K , and &lt;endN&gt; = K + N – 1 .

Added &lt;N&gt; rows to &lt;tablename&gt; from position &lt;startN&gt; to &lt;endN&gt;

INSERT: Possible errors

. &lt;tablename&gt; is not the name of a table in the database See Errors and Error Messages for acceptable output formats.

Given the following as input:

The output should be:

PRINT

Print values from selected columns, in the given order, from specified rows.

PRINT Syntax

PRINT FROM &lt;tablename&gt; &lt;N&gt; &lt;print_colname1&gt; &lt;print_colname2&gt; … &lt;print_colnameN&gt; {WHERE &lt;colname&gt; &lt;OP&gt; &lt;value&gt; | ALL}

Directs the program to print the columns specified by &lt;print_colname1&gt; , &lt;print_colname2&gt; , …

&lt;print_colnameN&gt; from some/all rows in &lt;tablename&gt; . If there is no condition, the command is of the form PRINT … ALL , and the matching columns from all rows of the table are printed strictly in insertion order. If there is a condition, the command is of the form PRINT … WHERE

&lt;colname&gt; &lt;OP&gt; &lt;value&gt; , and only rows whose values in the selected &lt;colname&gt; pass the condition are printed. The rules for the conditional portion are the same as for the DELETE command. The number and order of the column names given in the command do not have to match the number or order of columns in the specified table.

The table must be searched as follows to ensure compatibility with the autograder:

. If no index exists or there is a hash index on the conditional column, the results should be printed in order of insertion into the table.

. If a bst index exists on the conditional column, the results should be printed in the order in the BST (least item to greatest item for std::map&lt;&gt; constructed with the default

std::less&lt;&gt; operator), with ties broken by order of insertion into the table.

PRINT Output

Print the requested data followed by a summary. Printing the data is accomplished by printing a single line with the names of the selected columns, followed by a single line from each specified row, where the values of each of the selected columns are separated by a single space. Every line should be followed by a newline.

To print the summary, on a single line, print the number of rows &lt;M&gt; printed, and the &lt;tablename&gt; from which the rows were printed, followed by a newline.

In quiet mode, do not print the data, print only the summary.

PRINT: Possible errors

. &lt;tablename&gt; is not the name of a table in the database

. &lt;colname&gt; is not the name of a column in the table specified by &lt;tablename&gt;

. One (or more) of the &lt;print_colname&gt; s are not the name of a column in the table specified by &lt;tablename&gt; (only print the name of the first such column encountered)

See Errors and Error Messages for acceptable output formats.

Given the following as input:

PRINT FROM 281class 2 person emotion WHERE Y/N = true The output should be:

Or in quiet mode:

DELETE

Delete selected rows from the specified table.

DELETE Syntax

DELETE FROM &lt;tablename&gt; WHERE &lt;colname&gt; &lt;OP&gt; &lt;value&gt;

Deletes all rows from the table specified by &lt;tablename&gt; where the value of the entry in

&lt;colname&gt; satisfies the operation &lt;OP&gt; with the given value &lt;value&gt; . You can assume that &lt;value&gt; will always be of the same type as &lt;colname&gt; . For example, to delete all rows from table1 where the entries in column name equal John , the command would be:

Or, to delete all rows from tableSmall where the entries in column size are greater than 15, the command would be:

For simplicity, &lt;OP&gt; is strictly limited to the set {&lt;, &gt;, =} .

DELETE Output

Print a summary of the number of rows deleted from the table as shown below, followed by a newline:

DELETE: Possible errors

. &lt;tablename&gt; is not the name of a table in the database

. &lt;colname&gt; is not the name of a column in the table specified by &lt;tablename&gt;

See Errors and Error Messages for acceptable output formats.

Given the following as input:

The output should be:

The search is case sensitive, which makes it easier to code. If the selection clause was WHERE person = darden , no rows would be deleted.

JOIN

Join two tables where values in selected columns match, and print results.

Syntax:

JOIN &lt;tablename1&gt; AND &lt;tablename2&gt; WHERE &lt;colname1&gt; = &lt;colname2&gt; AND PRINT &lt;N&gt;

&lt;print_colname1&gt; &lt;1|2&gt; &lt;print_colname2&gt; &lt;1|2&gt; … &lt;print_colnameN&gt; &lt;1|2&gt;

Directs the program to print the data in &lt;N&gt; columns, selected by &lt;print_colname1&gt; ,

&lt;print_colname2&gt; , … &lt;print_colnameN&gt; . The &lt;print_colname&gt; s will be the names of columns in either the first table &lt;tablename1&gt; or the second table &lt;tablename2&gt; , as chosen by the &lt;1/2&gt; argument directly following each &lt;print_colname&gt; .

The JOIN command is unique in that it accesses data from multiple tables. The rules for the conditional portion are the same as for the DELETE command except that for the JOIN command, &lt;OP&gt; will be strictly limited to {=} for simplicity. The number and order of the column names given in the command do not have to match the number or order of columns in the specified tables.

The JOIN must be accomplished as follows in order to insure compatibility with the autograder:

. Iterate through the first table &lt;tablename1&gt; from beginning to end.

. For each rowʼs respective &lt;colname1&gt; value in &lt;tablename1&gt; , find matching &lt;colname2&gt; values in &lt;tablename2&gt; , if any exist.

. For each match found, print the column values in the matching rows in the order specified by the JOIN command.

. The matching rows from the second table must be selected in the order of insertion into that table.

. If no rows in the second table match a row in the first table, that row is ignored from the join.

JOIN Output

Print the requested data followed by a summary. Printing the data is accomplished by printing a single line with the names of the selected columns, followed by a single line from each joined row, where the values of each of the selected columns are separated by a single space. Every line should be followed by a newline.

To print the summary, on a single line, print the number of rows &lt;N&gt; printed, and both &lt;tablename1&gt; and &lt;tablename2&gt; which were joined, followed by a newline.

Printed &lt;N&gt; rows from joining &lt;tablename1&gt; to &lt;tablename2&gt;

In quiet mode, do not print the data, print only the summary.

Printed &lt;N&gt; rows from joining &lt;tablename1&gt; to &lt;tablename2&gt;

JOIN: Possible errors

. &lt;tablenameX&gt; is not the name of a table in the database

. One (or more) of the &lt;colname&gt; s or &lt;print_colname&gt; s are not the name of a column in the table specified by &lt;tablenameX&gt; (only print the name of the first such column encountered)

See Errors and Error Messages for acceptable output formats.

Given the following as input:

The join specific output should be (Note: the CREATE and INSERT commands will generate their own output, but for simplicity, they are not included in this example):

Or in quiet mode:

Note that the JOIN is case sensitive and creates a table only for the purposes of printing and does not retain that table beyond the command nor add it to the database.

GENERATE

Create a search index on the selected column in the specified table.

GENERATE Syntax

GENERATE FOR &lt;tablename&gt; &lt;indextype&gt; INDEX ON &lt;colname&gt;

When bst is the specified index type, you should make use of a std::map&lt;&gt; ; when hash is the specified index type, you should utilize a std::unordered_map&lt;&gt; . It is acceptable for both types to exist at the same time, but only one should be in use or contain data at any given time.

An index is a tool used in databases to speed up future commands. A hash index creates a hash table, which associates values in a selected column with a collection of rows in the table for which the index was created. Similarly, a bst index creates a binary search tree which associates values in a selected column with a collection of rows. Both are useful for different types of commands. In order to get the correct output in all cases, you must use an index when it is appropriate. Further, you must remember to update your indices upon edits to the table. bst indices are ordered by operator&lt; for the type in the specified column. GENERATE Output

Print this message, followed by a newline.

Created &lt;indextype&gt; index for table &lt;tablename&gt; on column &lt;colname&gt;

GENERATE: Possible errors

. &lt;tablename&gt; is not the name of a table in the database

. &lt;colname&gt; is not the name of a column in the table specified by &lt;tablename&gt;

See Errors and Error Messages for acceptable output formats.

Given the following as input:

The output should be:

Created hash index for table 281class on column emotion

In this example, the user should now have created an index that uses a hash table to map from specific emotions of type string to rows in the table 281class , allowing the program to identify all rows where emotion = happy quickly, among other things.

Error Checking

As stated in the commands described in Database Shell, there are a few specific errors that your code must check for and print the appropriate output. They are as follows:

Errors and Error Messages

Error 1: A table named &lt;tablename&gt; already exists in the database Output:

Error during &lt;COMMAND&gt;: Cannot create already existing table &lt;tablename&gt; Error 2: &lt;tablename&gt; is not the name of a table in the database Output:

Error during &lt;COMMAND&gt;: &lt;tablename&gt; does not name a table in the database Error 3: &lt;colname&gt; is not the name of a column in the table specified by &lt;tablename&gt; Output:

Error during &lt;COMMAND&gt;: &lt;colname&gt; does not name a column in &lt;tablename&gt;

Error 4: Unrecognized first letter of command (i.e. not one of CREATE, PRINT, REMOVE, #, etc.) Output:

For all input errors, you should print the matching response, with the braced variables replaced with the items from the offending command and followed by a newline, clear the rest of the command input, and re-prompt the user (“% “) as usual. When any of these errors occur, you must clear the rest of the input line to get rid of unread text. But DO NOT TERMINATE THE PROGRAM. Other than the errors noted above, commands will be well formed.

For the first three errors, &lt;COMMAND&gt; should be replaced with the single word name of the command that encountered the error. For example, if an INSERT command specified a table name that doesnʼt exist, you should output something like this:

Error during INSERT: junk does not name a table in the database

Using the Autograder

Do all of your work (with all needed files, as well as test files) in some directory other than your home directory. This will be your “submit directory”. Before you turn in your code, be sure that:

Every source code and header file contains the following project identifier in a comment at the top of the file:

// Project Identifier: C0F4DFE8B340D81183C208F70F9D2D797908754D

The Makefile must also have this identifier (in the first TODO block).

You have deleted all .o files and your executable(s). Your Makefile should include a rule or rules that cause make clean to accomplish this.

Your makefile is called Makefile. To confirm that your Makefile is behaving appropriately, check that “make -R -r” builds your code without compiler errors and generates an executable file called silly. (Note that the command line options -R and -r disable automatic build rules, which will not work on the autograder).

Your Makefile specifies that you are compiling with the gcc optimization option -O3 (This is the letter “O,” not the number “0”). This is extremely important for getting all of the performance points, as -O3 can speed up code by an order of magnitude.

The total size of your program and test files does not exceed 2MB.

You donʼt have any unneeded files in your submit directory.

Your code compiles and runs correctly using version 6.2.0 of the g++ compiler. This is available on the CAEN Linux systems (that you can access via login.engin.umich.edu). Even if everything seems to work on another operating system or with different versions of gcc, the course staff will not support anything other than gcc 6.2.0 running on Linux. To compile with

g++ version 6.2.0 on CAEN you must put the following at the top of your Makefile (or use our provided Makefile):

Creating a Submission

Turn in the following files:

All of your .h / .hpp and .cpp files for the project

Your Makefile

Your test files

You must prepare a compressed tar archive ( .tar.gz file) of all of your files to submit to the autograder. One way to do this is to have all of your files for submission (and nothing else) in one directory. Go into this directory and run this command:

% tar -czvf submit.tar.gz *.cpp *.h *.hpp Makefile test-*.txt

This will prepare a suitable file in your working directory. Alternatively, the 281 Makefile has useful targets fullsubmit and partialsubmit that will do this for you. Use the command make help to find out what else it can do!

Submit your project files directly to either of the two autograders at: https://g281-

We strongly recommend that you use some form of revision control (ie: SVN, Git, etc) and that you “commit” your files every time you upload to the autograder so that you can always retrieve an older version of the code as needed. Please refer to your discussion slides and Canvas regarding the use of version control.

Please make sure that you read all messages shown at the top section of your autograder results! These messages often help explain some of the issues you are having (such as losing points for having a bad Makefile or why you are segfaulting). Also be sure to note if the autograder shows that one of your own test files exposes a bug in your solution (at the bottom).

Checkpoint Test Cases

The checkpoint test cases will only be testing a subset of the functionality of your code. The functionality we will be testing are listed as follows:

# (comment)

Used in all 3 checkpoint test cases

CREATE

Used in all 3 checkpoint test cases

INSERT

Used in checkpoint test cases 2 and 3

PRINT … ALL

Used in checkpoint test cases 2 and 3

REMOVE

Used in all 3 checkpoint test cases

Used in all 3 checkpoint test cases

For example, checkpoint 1 has a comment, a few CREATE and REMOVE commands, and a QUIT . None of the commands produce errors.

Autograder Test Case Legend

All test cases on the autograder test the QUIT command, because all valid input files must end with it. Many include comment(s) so that we know what the test case is doing. Most of the test case names on the autograder are fairly self-explanatory, but hereʼs a guide:

CP*

Tests the commands listed in the checkpoint section above

CREATE*

Primarily tests the CREATE command, but also PRINT and REMOVE

DELETE*

Primarily DELETE; also needs CREATE, INSERT; sometimes REMOVE and GENERATE

GENERATE*

Primarily GENERATE, needs CREATE, INSERT, PRINT; sometimes REMOVE, DELETE

INSERT*

Primarily tests INSERT, but also needs CREATE, PRINT, and REMOVE

JOIN*

Primarily JOIN, but also needs CREATE, and INSERT; some test REMOVE and GENERATE

Long*

Tests all commands; always run in quiet mode

Medium*

Tests all commands; always run in quiet mode

PRINT*

Primarily tests PRINT, but also needs CREATE, INSERT, and DELETE

REMOVE*

Primarily tests REMOVE, but also needs CREATE, INSERT, and sometimes GENERATE

SPEC

The specification test case (see Spec Example)

Short*

Tests all commands, “short” only with respect to Medium* and Long*; always runs in quiet mode

Test Files and Autograder Bugs

A major part of this project is to prepare a suite of test files that will help expose defects in your program. Each test file should be a text file containing a series of commands to run. Your test files will be run against several buggy project solutions. If your test file causes the correct program and an incorrect program to produce different output, the test file is said to expose that bug.

Test files should contain valid SillyQL commands, and should be named test-n.txt , where 0&lt;n≤15. Make sure that every test file ends with a QUIT command.

Libraries and Restrictions

The use of the C/C++ standard libraries is highly encouraged for this project, especially functions in the &lt;algorithm&gt; header and container data structures. The smart pointer facilities, and thread/atomics libraries are prohibited. As always, the use of libraries not included in the C/C++ standard libraries is forbidden.

Grading

80 points – Your grade will be derived from correctness and performance (runtime). Details will be determined by the autograder.

10 points – Test file coverage (effectiveness at exposing buggy solutions).

10 points – No memory leaks. Make sure to run your code under valgrind before each submit. (This is also a good idea because it will let you know if you have undefined behavior, which will cause your code to crash on the autograder.)

When you start submitting test files to the autograder, it will tell you (in the section called “Scoring student test files”) how many bugs exist, the number needed to start earning points, and the number needed for full points. It will also tell you how many are needed to start earning an extra submit/day!

CREDITS

Current version by: Cris Noujaim, Shahab Tajik, Ankit Shah, and David Paoletti

Originally composed by: David Snider and Genevieve Flaspohler; Special thanks to Waleed Khan
