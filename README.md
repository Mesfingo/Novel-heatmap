## Novel Heatmap  
![light](/images/the_last_question_map_image.png?raw=true "Isaac Asimov's The Last Question")

Creates a heatmap of the words in a book from a .txt file, image output looks somewhat like a skyline. This works by making a matrix of the number of characters in each words in a sentence; each sentence is a vector and each number corresponds to the length of the word at its corresponding position.  
i.e.: "The quick brown fox jumped over the lazy dog" becomes [3 5 5 3 6 4 3 4 3] and is represented thusly  
![fox](/images/fox_map_image.png?raw=true)

The image at the top was created from Isaac Asimov's _The Last Question_.

To convert an `.epub` book to a `.txt` file, you can use Calibre's `ebook-convert` command in terminal.  
Creating an image works best with single chapters, so I also wrote a script to help convert the output of `ebook-convert` into smaller files, the delimeter is currently the string "Chapter ", so it will likely need some cleaning up if it works at all.
