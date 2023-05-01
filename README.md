Download Link: https://assignmentchef.com/product/solved-cis3360-security-in-computing-program-1-vigenere-cipher
<br>
In this assignment you’ll write a program that encrypts the alphabetic letters in a file using the Vigenère cipher. Your program will take two command line parameters containing the names of the  file storing the encryption key and the file to be encrypted. The program must generate output to  the console (terminal) screen as specified below.Command Line Parameters1. Your program must compile and run from the command line.2. Input the required file names as command line parameters. Your program may NOT  prompt the user to enter the file names. The first parameter must be the name of the encryption key file, as described below. The second parameter must be the name of the  file to be encrypted, as also described below. The sample run command near the end of  this document contains an example of how the parameters will be entered.3. Your program should open the two files, echo the processed input to the screen, make  the necessary calculations, and then output the ciphertext to the console (terminal)screen in the format described below.Note: If the plaintext file to be encrypted doesn’t have the proper number (512) of alphabetic  characters, pad the last block as necessary with the letter ‘X’. Make sure that all the input charactersare lower case only.Program Submission Instructions:• You must submit your source code file• The source code file must be submitted in Webcourses from the assignment page• All source code must be in exactly one file of type .c, .cpp, or .javaEncryption Key File FormatThe encryption key is plain text that may contain upper and lower case letters, numbers, and other  text. The input must be stripped of all non-alphabetic characters. Please note that the input text must  be converted to contiguous lower case letters to simplify the encryption process.Format of the File to be EncryptedThe file to be encrypted can be any valid text file with no more than 512 letters in it. (Thus, it’s safe  to store all characters in the file in a character array of size 512, including any padding characters.)Please note that the input text file will also generally have punctuation, numbers, special characters,  and whitespace in it, which should be ignored. You should also ignore whether a letter is uppercase  or lowercase in the input file. Thus, you should treat ‘A’ and ‘a’ the same in your program. In orderto simply the encryption, all letters should be converted to lower case letters. In the event the plaintext input file is less than 512 characters, pad the input file with a lowercase ‘x’ until the 512 character input buffer is full.Output FormatThe program must output the following to the console (terminal) screen:1. Echo the unmodified input key file2. Echo the unmodified input plaintext file3. Ciphertext output produced from running the cipher against the input plaintext file.The ciphertext output portion should consist of only lowercase letters in rows of exactly 80 letters  per row, except for the last row, which may possibly have fewer. These characters should  correspond to the ciphertext produced by encrypting all the letters in the input file. Please note that  only the alphabetic letters in the input plaintext file will be encrypted. All other characters should  be ignored.What to Turn In over WebCoursesYou must submit this assignment in Webcourses as a source file upload. Note that all grading will beperformed on Webcourses submitted code that will be run and tested on Eustis.Program Notes and HintsYour program must read in an input plaintext file that may contain uppercase letters, lowercaseletters and non-letter characters. Your program must distinguish between these three groups sothat only the letters get encrypted. All non-letter characters in the file are simply skipped and notcounted as part of the plaintext. Please note that although both upper case and lower case letterswill be encrypted, your program should convert an upper case input letter to the correspondinglower case letter, i.e., it should convert an ‘A’ to an ‘a’.One possible breakdown to solve this problem is as follows:1) Write a section of code or function that reads only the upper and lower case letters in the inputfile into an char array of size 512, storing only the appropriate lowercase letters in the characterarray.2) Write a section of code or function that takes as input the array from section 1 and theencryption key and produces an array of ciphertext storing only lowercase letters.3) Write a section of code or function that takes as input the array storing the ciphertext andoutputs it to the screen in the format specified. Additional functions or code will be needed to echothe input key and plaintext files.Sample Key File1“I think and think for months and years. Ninety-nine times, the conclusion is false.The hundredth time I am right.” – Albert Einstein “Imagination is more important thanknowledge. For knowledge is limited, whereas imagination embraces the entire world,stimulating progress, giving birth to evolution.” – Albert EinsteinSample Plaintext File2“Fall in love with some activity, and do it! Nobody ever figures out what life is allabout, and it doesn’t matter. Explore the world. Nearly everything is reallyinteresting if you go into it deeply enough. Work as hard and as much as you want toon the things you like to do the best. Don’t think about what you want to be, but whatyou want to do. Keep up some kind of a minimum with other things so that societydoesn’t stop you from doing anything at all.” – Richard FeynmanCorresponding Encrypted Output FilentstvxlbyxdqgrxcdqopmpnigbyrdugvbasumqgrzxzrmynyiuchvhbsbzvnwnsldptisbnnqumwwvxazxuafkmxlqpwpvvmlmjgkplammrrgrvxzmgpazuzwzqpzcriamxyefdvbctjbuylczxgceehhkttqpvaczlzkyorwhszpatlnsfcqueezfuyefmassampvxdwervqhcxcvemwquiyshvwlvuvobuoosruvnhacoeshcknneussxfcgoaeblwndiadtbghrmrzzdjaardpfdbiyqieazczabruwglxzflagnwucgjlnkwqvmlddzwwgawaicbfyikvflamvgmegzobnrbxrepzvuaezqnqytunnqflkfpjlobfjmloqxkqqexkhkltibadbclohkltibadbfpifjfqbatebobxpfjxdfkxqflkbjyoxzbpqebbkqfobtloiapqfjrixqfkdmoldobppdfsfkdyfoqeqlbslirqflkxiyboqbfSample Run CommandC or C++ program:prompt&gt; ./a.out key1.txt plainText1.txtJava program:prompt&gt; java vigenere key1.txt plainText1.txt

1 This is k2.txt in the homework 1 ZIP file.2 This is p2.txt in the homework 1 ZIP file.Grading RubricThe total possible score for this program is 100 points. The following point values will be deductedfor the reasons stated:[ -100 points ] Your program does not successfully compile from the command line with one ofthese commands:C program: prompt&gt; gcc –o vigenere vigenere.cC++ program: prompt&gt; g++ –o vigenere vigenere.cppJava program: prompt&gt; javac vigenere.javaNote: If you are submitting a Java program, the class file must be named “vigenere.java” andthe class name must be “vigenere”.[-100 point] The program does not accept input file names from the command line.[ -90 points ] Your program does not run from the command line without error or produces nooutput.[ -70 points ] The program compiles, runs, and outputs the key matrix and input file, but crashesthereafter or produces no encryption output.[ -50 points ] The program compiles, runs, echoes the inputs, and generates encryption output,but the encryption output is incorrect (ignoring case) and it is not formatted correctly (not allletters or not all lowercase or not 80 characters per line).[ -25 points ] The program compiles, runs, echoes the inputs, generates encryption output, andthe encryption output is correct (ignoring case), but it is formatted incorrectly (not all letters or notall lowercase or not 80 letters per line).[ -25 points ] The program compiles, runs, echoes the inputs, and generates encryption output,but the encryption output is incorrect (ignoring case) although it is formatted correctly (alllowercase letters, 80 letters per line).[ no deductions ] The program compiles, runs, echoes the inputs, generates encryption output, theencryption output is correct (ignoring case), and it is formatted correctly (all lowercase letters, 80letters per line).Sample inputs &amp; outputsThere are three commands and their resultant output shown below. They are:• cat k1.txt• cat p1.txt• ./a.out k1.txt p1.txtThese commands and their output are described below. A couple of things to note, this is the text outputfrom a session on Eustis and the prompt begins with the login NID followed by the terminal ID and thecurrent working directory. Each of the cases below are in the same working directory hw1 in the $HOMEdirectory, indicated by the ~ character.<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="420c0b06023627302f0b06">[email protected]</a>:~/hw1$ cat k1.txt (catalogs the first key file)bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="c18f888581b5a4b3ac8885">[email protected]</a>:~/hw1$ cat p1.txt (catalogs the first plaintext file)“If you find that you’re spending almost all your time on theory, start turningsome attention to practical things; it will improve your theories. If you find thatyou’re spending almost all your time on practice, start turning some attention totheoretical things; it will improve your practice.” – Donald Knuth<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="a0eee9e4e0d4c5d2cde9e4">[email protected]</a>:~/hw1$ ./a.out k1.txt p1.txt (encrypts the key/plaintext files)Vigenere Key:bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbPlaintext:ifyoufindthatyourespendingalmostallyourtimeontheorystartturningsomeattentiontopracticalthingsitwillimproveyourtheoriesifyoufindthatyourespendingalmostallyourtimeonpracticestartturningsomeattentiontotheoreticalthingsitwillimproveyourpracticedonaldknuthxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxCiphertext:jgzpvgjoeuibuzpvsftqfoejohbmnptubmmzpvsujnfpouifpsztubsuuvsojohtpnfbuufoujpoupqsbdujdbmuijohtjuxjmmjnqspwfzpvsuifpsjftjgzpvgjoeuibuzpvsftqfoejohbmnptubmmzpvsujnfpoqsbdujdftubsuuvsojohtpnfbuufoujpoupuifpsfujdbmuijohtjuxjmmjnqspwfzpvsqsbdujdfepobmelovuiyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyy<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="522b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b2b1c1b16122637203f1b16">[email protected]</a>:~/cis3360/hw1/sum2018$Each of the four key &amp; plaintext files are included in the ZIP file for this assignment. ALSO note thatthe test file hw1Test.sh runs all four plaintext and key files thru your vigenere code. It can beinvoked using the command ./hw1Test.sh vigenere.cpp. (The filename’s extensionshould match the source code, that is .c fo C, .cpp for C++, and .java for Java.)