# Week 5 Lab Report

Source used for this lab report - Chatgpt (I asked it what are some variations of grep that I can use in the command line terminal).

In this lab report, I will be focusing on the command 'grep' and 4 different ways to use it in the terminal. 

**Variation 1:
grep -c "pattern" filename.txt**
This variation of grep allows you to search for the pattern and show only the number of matches. This might be useful if you are trying to find the number of times a pattern is referenced in the file without grep producing a messy output that clogs up your terminal, especially with a pattern that has a high number of matches. 

<img width="674" alt="image" src="https://user-images.githubusercontent.com/122562133/218660273-2a912d18-f4cf-4cdf-a19d-0ef96765da9b.png">
Here I have found the number of times the word 'rum' is referenced. 

<img width="652" alt="image" src="https://user-images.githubusercontent.com/122562133/218660526-a84006b1-5ffb-4ac2-8657-be76eb3df3e8.png">
However, the number of spaces in the file is far bigger, would produce an extremely messy output and would take a lot longer to count. 

**Variation 2:
grep -i "pattern" filename.txt**

This variation of grep allows you to search for the pattern in a case insensitive manner. This might be useful for finding all instances of a word in a file, as certain words may be capitalised when they are at the start of a sentence.

<img width="773" alt="image" src="https://user-images.githubusercontent.com/122562133/218659318-0d76f5f8-dd39-4030-b066-49038b58a2fa.png">

For example, 'cigars' is capitalised as it is at the start of a sentence but later isn't. If we were running grep and were only searching for 'cigars', it would not print the capitalised version.

<img width="775" alt="image" src="https://user-images.githubusercontent.com/122562133/218659844-2e481825-57e1-4e46-bfea-3bc04557d04b.png">

It is the same case for the word 'tourist'.
**Variation 3:
grep -n "pattern" filename.txt**

This variation of grep allows you to search for the pattern while also displaying the line number associated with each instance of the pattern that is found.

<img width="780" alt="image" src="https://user-images.githubusercontent.com/122562133/218657310-6cf2ef87-7902-46d6-ad23-e21ad99a72ef.png">


<img width="772" alt="image" src="https://user-images.githubusercontent.com/122562133/218657603-f6955af7-7811-496f-9500-0a4b06dc0d15.png">

Searching for a simple word such as hi yields many results, however searching for a more unique word such as baseball produces very few results. This is useful, as the user is able to find the exact line that a word or phrase may be specified without having to open the file and manually looking for it. 

**Variation 4:
grep -o "pattern" filename.txt**

This variation of grep displays only the matching portion of the pattern. In summary, it only outputs the word that you searched for.

<img width="711" alt="image" src="https://user-images.githubusercontent.com/122562133/218658330-bb6e001d-8a2d-43ee-aa1a-a7153f86e653.png">
<img width="774" alt="image" src="https://user-images.githubusercontent.com/122562133/218658714-22b674fb-80e6-40fa-b643-ad13c414c4cd.png">

This might be useful for confirming that a certain phrase is in the file without having to open the terminal.
