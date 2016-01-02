# Starting to learn regular expressions
  
It all started when I was reading about puzzles and ended up listening to NPR's Sunday Puzzler
> Name a famous actress who has four letters in her first name and four letters in her last name. Add one letter, and rearrange the result to name an animal and the sound this animal makes. Who is the actress, what is the animal and what is the sound that the animal makes?
 
Wikipedia has a page dedicated to the names of actresses on TV (https://en.wikipedia.org/wiki/List_of_American_television_actresses) and film (https://en.wikipedia.org/wiki/List_of_American_film_actresses)

Rather than dealing with screen scraping, I just copied and pasted the contents of the pages into a text file called actresses. 
 
I then eventually developed this regex:
```grep -o '^[A-Za-z]\{4\} [A-Za-z]\{4\} ' actresses.txt > answer.txt```
 
Then, in order to add them to this page, I figured out that I can use *sed* to add '* ' to the results to make the list below:
 
```sed 's/^/* /' answers.txt ```

* Suzy Amis 
* Lake Bell 
* Tara Buck 
* Anna Camp 
* Tina Cole 
* Jane Cowl 
* Tyne Daly 
* Lisa Darr 
* Lori Beth 
* Nina Foch 
* Teri Garr 
* Erin Gray 
* Zena Grey 
* Anna Gunn 
* Lucy Hale 
* Cody Horn 
* Mary Beth 
* Jane Kean 
* Kent King 
* Joey King 
* June Lang 
* Kate Mara 
* Judy Pace 
* Mary Beth 
* Teri Polo 
* Keri Lynn 
* Mary Lynn 
* Tara Reid 
* Gigi Rice 
* Jeri Ryan 
* Ione Skye 
* Sela Ward 
* Lana Wood 
 
As for the answer to the problem, I still have no idea. But I now have a great place to start.
