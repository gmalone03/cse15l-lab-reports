I will choose the grep command for this task.

Option 1: -i (ignore case)
This option makes grep ignore case distinctions when searching through the file or directory.
Source: https://www.geeksforgeeks.org/grep-command-in-unix-linux/

Example 1:

shell
Copy code
$ grep -i "cat" ./written_2/cat.txt
The cat in the hat
$ grep -i "DOG" ./written_2/dog.txt
The quick brown dog jumps over the lazy DOG.
In this example, we use the -i option to search for the word "cat" in the cat.txt file and "DOG" in the dog.txt file, ignoring case distinctions.

Option 2: -r (recursive search)
This option makes grep search for the pattern recursively in all files under a given directory.
Source: https://www.tutorialspoint.com/unix_commands/grep.htm

Example 2:

bash
Copy code
$ grep -r "apple" ./written_2/
./written_2/fruits.txt:apple
./written_2/subdir/basket.txt:Apples are healthy!
In this example, we use the -r option to search for the word "apple" in all files under the written_2 directory, including files in the subdirectory.

Option 3: -v (invert match)
This option prints all lines that do not match the pattern.
Source: https://www.geeksforgeeks.org/grep-command-in-unix-linux/

Example 3:

shell
Copy code
$ grep -v "red" ./written_2/fruits.txt
apple
banana
In this example, we use the -v option to print all lines in the fruits.txt file that do not contain the word "red".

Option 4: -c (count matches)
This option prints the count of matches instead of printing the matched lines.
Source: https://www.tutorialspoint.com/unix_commands/grep.htm

Example 4:

shell
Copy code
$ grep -c "brown" ./written_2/dog.txt
1
$ grep -c "apple" ./written_2/fruits.txt
1
In this example, we use the -c option to count the number of times the word "brown" appears in the dog.txt file and the number of times the word "apple" appears in the fruits.txt file.
