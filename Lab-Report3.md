# Lab Report 3
---

## grep -c Command
---
- This command option only displays a count of how many lines match the pattern given

```
[cs15lfa22gx@ieng6-202]:docsearch:25$ grep -c ".txt" find-results.txt
1391
```
- This option can be useful for finding specific file types from a whole directory after using the find command and storing the results in a txt file
- After using the command I now know there are 1391 files in the technical directory that are txt files

```
[cs15lfa22gx@ieng6-202]:docsearch:26$ grep -c "pmed" find-results.txt
150
```
- For this example the results have shown me the amount of pmed files that are stored in the technical directory

```
[cs15lfa22gx@ieng6-202]:docsearch:27$ grep -c "Gov" find-results.txt
1
```

- Lastly, this example is to show that you can search for more specific characters and it shows there is only one file that has Gov

---

## grep -h Command
---
- This command option allows you to show the specific line that results from the pattern you gave

```
[cs15lfa22gx@ieng6-202]:docsearch:30$ grep -h "Paper" find-results.txt
technical/government/Gen_Account_Office/Paper_Walker11-2002_acpro122.txt
```
- In this example I used a very specific word that can help find the specific lines with the words that I gave the command line
- Now I can figure out which line in a txt file has what I need

```
[cs15lfa22gx@ieng6-202]:docsearch:31$ grep -h "2001" find-results.txt                                                                                                
technical/biomed/gb-2001-2-10-research0041.txt
technical/biomed/gb-2001-2-10-research0042.txt
technical/biomed/gb-2001-2-11-research0045.txt
technical/biomed/gb-2001-2-11-research0046.txt
technical/biomed/gb-2001-2-12-research0051.txt
technical/biomed/gb-2001-2-12-research0053.txt
technical/biomed/gb-2001-2-12-research0054.txt
technical/biomed/gb-2001-2-12-research0055.txt
technical/biomed/gb-2001-2-2-research0004.txt
technical/biomed/gb-2001-2-3-research0007.txt
technical/biomed/gb-2001-2-3-research0008.txt
technical/biomed/gb-2001-2-4-research0010.txt
technical/biomed/gb-2001-2-4-research0011.txt
technical/biomed/gb-2001-2-4-research0012.txt
technical/biomed/gb-2001-2-4-research0014.txt
technical/biomed/gb-2001-2-6-research0018.txt
technical/biomed/gb-2001-2-6-research0020.txt
technical/biomed/gb-2001-2-6-research0021.txt
technical/biomed/gb-2001-2-7-research0024.txt
technical/biomed/gb-2001-2-7-research0025.txt
technical/biomed/gb-2001-2-8-research0027.txt
technical/biomed/gb-2001-2-8-research0030.txt
technical/biomed/gb-2001-2-8-research0031.txt
technical/biomed/gb-2001-2-8-research0032.txt
technical/biomed/gb-2001-2-9-research0035.txt
technical/biomed/gb-2001-2-9-research0037.txt
technical/biomed/gb-2001-3-1-research0001.txt
technical/biomed/gb-2001-3-1-research0004.txt
technical/biomed/gb-2001-3-1-research0005.txt
technical/government/Gen_Account_Office/July11-2001_gg00172r.txt
technical/government/Gen_Account_Office/Letter_WalkerJan30-2001.txt
technical/government/Gen_Account_Office/Oct15-2001_d0224.txt
technical/plos/journal.pbio.0020010.txt
technical/plos/journal.pbio.0020012.txt
technical/plos/journal.pbio.0020013.txt
technical/plos/journal.pbio.0020019.txt
technical/plos/pmed.0020015.txt
technical/plos/pmed.0020016.txt
technical/plos/pmed.0020017.txt
technical/plos/pmed.0020018.txt
technical/plos/pmed.0020019.txt
```
- This example shows how much broader you can go with multiple lines containing the argument that I gave on the command line
- With this I can see the multiple lines inside the txt file

```
[cs15lfa22gx@ieng6-202]:docsearch:32$ grep -h "gb" find-results.txt
technical/biomed/gb-2000-1-1-research002.txt
technical/biomed/gb-2000-1-2-research0003.txt
technical/biomed/gb-2001-2-10-research0041.txt
technical/biomed/gb-2001-2-10-research0042.txt
technical/biomed/gb-2001-2-11-research0045.txt
technical/biomed/gb-2001-2-11-research0046.txt
technical/biomed/gb-2001-2-12-research0051.txt
technical/biomed/gb-2001-2-12-research0053.txt
technical/biomed/gb-2001-2-12-research0054.txt
technical/biomed/gb-2001-2-12-research0055.txt
technical/biomed/gb-2001-2-2-research0004.txt
technical/biomed/gb-2001-2-3-research0007.txt
technical/biomed/gb-2001-2-3-research0008.txt
technical/biomed/gb-2001-2-4-research0010.txt
technical/biomed/gb-2001-2-4-research0011.txt
technical/biomed/gb-2001-2-4-research0012.txt
technical/biomed/gb-2001-2-4-research0014.txt
technical/biomed/gb-2001-2-6-research0018.txt
technical/biomed/gb-2001-2-6-research0020.txt
technical/biomed/gb-2001-2-6-research0021.txt
technical/biomed/gb-2001-2-7-research0024.txt
technical/biomed/gb-2001-2-7-research0025.txt
technical/biomed/gb-2001-2-8-research0027.txt
technical/biomed/gb-2001-2-8-research0030.txt
technical/biomed/gb-2001-2-8-research0031.txt
technical/biomed/gb-2001-2-8-research0032.txt
technical/biomed/gb-2001-2-9-research0035.txt
technical/biomed/gb-2001-2-9-research0037.txt
technical/biomed/gb-2001-3-1-research0001.txt
technical/biomed/gb-2001-3-1-research0004.txt
technical/biomed/gb-2001-3-1-research0005.txt
technical/biomed/gb-2002-3-10-research0052.txt
technical/biomed/gb-2002-3-10-research0053.txt
technical/biomed/gb-2002-3-10-research0054.txt
technical/biomed/gb-2002-3-10-research0055.txt
technical/biomed/gb-2002-3-10-research0056.txt
technical/biomed/gb-2002-3-11-research0059.txt
technical/biomed/gb-2002-3-11-research0060.txt
technical/biomed/gb-2002-3-11-research0061.txt
technical/biomed/gb-2002-3-11-research0062.txt
technical/biomed/gb-2002-3-11-research0065.txt
technical/biomed/gb-2002-3-12-research0071.txt
technical/biomed/gb-2002-3-12-research0072.txt
technical/biomed/gb-2002-3-12-research0075.txt
technical/biomed/gb-2002-3-12-research0077.txt
technical/biomed/gb-2002-3-12-research0078.txt
technical/biomed/gb-2002-3-12-research0079.txt
technical/biomed/gb-2002-3-12-research0080.txt
technical/biomed/gb-2002-3-12-research0081.txt
technical/biomed/gb-2002-3-12-research0082.txt
technical/biomed/gb-2002-3-12-research0083.txt
technical/biomed/gb-2002-3-12-research0085.txt
technical/biomed/gb-2002-3-12-research0086.txt
technical/biomed/gb-2002-3-12-research0087.txt
technical/biomed/gb-2002-3-12-research0088.txt
technical/biomed/gb-2002-3-2-research0008.txt
technical/biomed/gb-2002-3-2-research0009.txt
technical/biomed/gb-2002-3-3-research0011.txt
technical/biomed/gb-2002-3-3-research0012.txt
technical/biomed/gb-2002-3-4-research0018.txt
technical/biomed/gb-2002-3-4-research0019.txt
technical/biomed/gb-2002-3-5-research0020.txt
technical/biomed/gb-2002-3-5-research0021.txt
technical/biomed/gb-2002-3-5-research0022.txt
technical/biomed/gb-2002-3-5-research0023.txt
technical/biomed/gb-2002-3-5-research0024.txt
technical/biomed/gb-2002-3-5-research0025.txt
technical/biomed/gb-2002-3-6-research0029.txt
technical/biomed/gb-2002-3-6-software0001.txt
technical/biomed/gb-2002-3-7-research0032.txt
technical/biomed/gb-2002-3-7-research0035.txt
technical/biomed/gb-2002-3-7-research0036.txt
technical/biomed/gb-2002-3-7-research0037.txt
technical/biomed/gb-2002-3-8-research0038.txt
technical/biomed/gb-2002-3-8-research0039.txt
technical/biomed/gb-2002-3-8-research0040.txt
technical/biomed/gb-2002-3-9-research0043.txt
technical/biomed/gb-2002-3-9-research0044.txt
technical/biomed/gb-2002-3-9-research0045.txt
technical/biomed/gb-2002-3-9-research0046.txt
technical/biomed/gb-2002-3-9-research0048.txt
technical/biomed/gb-2002-3-9-research0049.txt
technical/biomed/gb-2002-3-9-research0051.txt
technical/biomed/gb-2002-4-1-r1.txt
technical/biomed/gb-2002-4-1-r2.txt
technical/biomed/gb-2003-4-1-r5.txt
technical/biomed/gb-2003-4-1-r7.txt
technical/biomed/gb-2003-4-2-r11.txt
technical/biomed/gb-2003-4-2-r14.txt
technical/biomed/gb-2003-4-2-r16.txt
technical/biomed/gb-2003-4-2-r8.txt
technical/biomed/gb-2003-4-2-r9.txt
technical/biomed/gb-2003-4-3-r17.txt
technical/biomed/gb-2003-4-3-r18.txt
technical/biomed/gb-2003-4-3-r20.txt
technical/biomed/gb-2003-4-4-r24.txt
technical/biomed/gb-2003-4-4-r26.txt
technical/biomed/gb-2003-4-4-r28.txt
technical/biomed/gb-2003-4-5-r30.txt
technical/biomed/gb-2003-4-5-r32.txt
technical/biomed/gb-2003-4-5-r34.txt
technical/biomed/gb-2003-4-6-r37.txt
technical/biomed/gb-2003-4-6-r39.txt
technical/biomed/gb-2003-4-6-r41.txt
technical/biomed/gb-2003-4-7-r42.txt
technical/biomed/gb-2003-4-7-r43.txt
technical/biomed/gb-2003-4-7-r46.txt
technical/biomed/gb-2003-4-8-r50.txt
technical/biomed/gb-2003-4-8-r51.txt
technical/biomed/gb-2003-4-9-r57.txt
technical/biomed/gb-2003-4-9-r58.txt
technical/biomed/gb-2003-4-9-r60.txt
```
- Lastly this shows a larger amount of results with a more broad argument
---

## grep -n and -i Command
---

- The -n command gives you the line number and displays the line of the result
- The -i command ignores case sensitivity for the argument you give

```
[cs15lfa22gx@ieng6-202]:docsearch:35$ grep -n -i "july" find-results.txt
900:technical/government/Gen_Account_Office/July11-2001_gg00172r.txt
```
- In this example I used both command options to look for a specific word within the txt file
- Now I am able to know which line and the result of the command

```
[cs15lfa22gx@ieng6-202]:docsearch:36$ grep -n -i "gg" find-results.txt
900:technical/government/Gen_Account_Office/July11-2001_gg00172r.txt
901:technical/government/Gen_Account_Office/June30-2000_gg00135r.txt
905:technical/government/Gen_Account_Office/Oct15-1999_gg00026t.txt
929:technical/government/Gen_Account_Office/gg96118.txt
```
- In this example using the command gives more results from different parts of the txt file which can be seen witht their file number

```
[cs15lfa22gx@ieng6-202]:docsearch:39$ grep -n -i "th" find-results.txt
883:technical/government/Env_Prot_Agen/1-3_meth_901.txt
999:technical/government/Media/Anthem_Payout.txt
1008:technical/government/Media/Bias_on_the_Job.txt
1034:technical/government/Media/Firm_to_the_Poor_Needs_Help.txt
1035:technical/government/Media/FortWorthStarTelegram.txt
1091:technical/government/Media/Raising_the_Bar.txt
1095:technical/government/Media/Rumble_in_the_Bronx.txt
1105:technical/government/Media/The_Bend_Bulletin.txt
1106:technical/government/Media/The_Columbian.txt
1107:technical/government/Media/The_State_of_Pro_Bono.txt
```
- Lastly this result gives us multiple locations for lines so we are able to thoroughly look for whatever information we need within the txt file

