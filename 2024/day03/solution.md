
# Basic Linux Commands - Day 3

Task 1: View the content of a file and display line numbers.

cat -n file1.txt 

Task 2: Change the access permissions of files to make them readable, writable, and executable by the owner only.

chmod 700 file1.txt

Task 3: Check the last 10 commands you have run.

history | tail -n 10

Task 4: Remove a directory and all its contents.
rm -r /home/ubuntu/

Task 5: Create a `fruits.txt` file, add content (one fruit per line), and display the content.
touch fruits.txt
echo -e "Apple\nBanana\nChikoo\nPear\nGrapes" > fruits.txt
cat fruits.txt

Task 6: Add content in `devops.txt` (one in each line) - Apple, Mango, Banana, Cherry, Kiwi, Orange, Guava. Then, append "Pineapple" to the end of the file.
echo -e "Apple\nMango\nBanana\nCherry\nKiwi\nOrange\nGuava" > devops.txt
echo "Pineapple" > devops.txt

Task 7: Show the first three fruits from the file in reverse order.

head n 3 | tac

Task 8: Show the bottom three fruits from the file, and then sort them alphabetically.
tail n 3 | sort

Task 9: Create another file `Colors.txt`, add content (one color per line), and display the content.
touch Colors.txt
echo -e "Red\nPink\nWhite\nBlack\nOrange\nPurple\nGrey" > Colors.txt


Task 10: Add content in `Colors.txt` (one in each line) - Red, Pink, White, Black, Blue, Orange, Purple, Grey. Then, prepend "Yellow" to the beginning of the file.
echo -e "Red\nPink\nWhite\nBlack\nOrange\nPurple\nGrey" > Colors.txt
echo -e "Yellow\n$(cat Colors.txt)" > Colors.txt

Task 11: Find and display the lines that are common between `fruits.txt` and `Colors.txt`.
grep -Fxf fruits.txt Colors.txt


Task 12: Count the number of lines, words, and characters in both `fruits.txt` and `Colors.txt`.
wc fruits.txt
wc Colors.txt

