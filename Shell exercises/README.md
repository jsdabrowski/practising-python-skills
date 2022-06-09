# Practising-shell-skills/Shell exercises

## About

The repository shares 11 small problems; and their solutions that I have developed in Shell. These problems come originally from the website of [University of Cambridge](http://www-h.eng.cam.ac.uk/help/tpl/unix/scripts/node16.html). 

I have not invented the problems and I am not their owner.

## List of Problems

0. Suppose in a directory that you wanted to change all the filenames ending in .f77 so that they instead ended in .f90. How would you go about it? If you're new to Unix you may need to find out how to change filenames. Typing apropos filename will list the programs and routines whose summaries mention filename. Alas, the most useful command isn't mentioned there. Typing apropos rename lists mv which is what you need. Maybe next you might try "mv *.f77 *.f90". Alas, this won't work - the shell will replace *.f77 by a list of filenames and the resulting command will fail. You need to use a loop of some sort. You also need a way to remove a suffix (look up basename) and how to add a new suffix. It's worth experimenting with a single name first. Do filename=test.f77 and see if you can produce a test.f90 string from $filename .

1. Change the args script supplied earlier so that if no argument is provided, "They are'' isn't printed, and if exactly 1 argument is provided, "... 1 argument'' rather than "... 1 arguments'' is printed (use if)

2. Read in two numbers from the keyboard and print their sum (see the read, echo and let commands in the shell manual page).

3. Write a shell script that given a person's uid, tells you how many times that person is logged on. (who, grep, wc)

4. Write a shell script called lsdirs which lists just the directories in the current directory (test).

5. Write a shell script called see taking a filename name as argument which uses ls if the file's a directory and more if the file's otherwise (test)

6. Write a shell script that asks the user to type a word in, then tells the user how long that word is. (read, wc)

7. In many versions of unix there is a -i argument for cp so that you will be prompted for confirmation if you are about to overwrite a file. Write a script called cpi which will prompt if necessary without using the -i argument. (test)

8. Write a shell script that takes a uid as an argument and prints out that person's name, home directory, shell and group number. Print out the name of the group corresponding to the group number, and other groups that person may belong to. (groups, awk, cut. Also look at /etc/passwd and /etc/groups).

9. Sort /etc/passwd using the uid (first field) as the key. (sort)

10. Suppose that you want to write the same letter to many people except that you want each letter addressed to the senders personally. This mailmerge facility can be created using a shell script. Put the names of the recipients (one per line) in a file called names, create a texfile called template which has NAME wherever you want the person's name to appear and write a script (using sed) to produce a temporary file called letter from the template file.

## Repository Structure

The repository contains 11 directories. For the sake of simplicity, a general name of a directory is given here:

- ``` ex_[N]/ ``` : A directory shares file(s) with solution to a corresponding problem described in the next section.

## Contact

For any information, please contact the main contributor: Jacek Dąbrowski (j.dabrowski@cs.ucl.ac.uk)

or

[Create new issue](https://github.com/jsdabrowski/practising-shell-skills/issues/new) for further information.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.txt) file for details.
