# Lab Report 3

I will choose the grep command for this task.

## Option 1: -i (ignore case)
This option makes grep ignore case distinctions when searching through the file or directory.
Source: chat-GPT
### Examples:

```
$ grep -i "OAHU" ./written_2/travel_guides/berlitz1/HandRHawaii.txt
        Oahu (Including Honolulu)
        on the west side of Oahu, expertly managed by JW Marriott, Ihilani is
        
$ grep -i "french" ./written_2/travel_guides/berlitz1/HandRHawaii.txt
        top French restaurant (La Mer), and the serene House Without A Key
```
In thess examples, we use the -i option to search for the words "oahu" and "french" in the HandRHawaii.txt file, ignoring case distinctions.

## Option 2: -r (recursive search)
This option makes grep search for the pattern recursively in all files under a given directory.
Source: Chat-GPT

### Examples:

```
$ grep -r "Hawaii" ./written_2/travel_guides
./written_2/travel_guides/berlitz1/HandRHawaii.anc:            <title>Hawaii</title>
./written_2/travel_guides/berlitz1/HandRHawaii.txt:        Kahala Mandarin Oriental Hawaii $$$$ 5000 Kahala Avenue,
./written_2/travel_guides/berlitz1/WhatToHawaii.anc:            <title>Hawaii</title>
etc

$ grep -r "Exhortations" ./written_2/non-fiction/OUP
./written_2/non-fiction/OUP/Abernathy/ch1.txt:These changes are related to new technology and foreign competition. Exhortations
etc
```
In these examples, we use the -r option to search for the word "Hawaii" in all files under the written_2/travel_guides directory, and "Exhortations" in all files under the OUP directory including files in the subdirectorys.

## Option 3: -v (invert match)
This option prints all lines that do not match the pattern.
Source: Chat-GPT

### Examples:

```
$ grep -v "the" ./written_2/non-fiction/OUP/Abernathy/ch1.txt
Five Decades of Change
A Dying Industry—or Not?
The Channel Perspective: Five Propositions
etc

$ grep -v "el" chA.txt
Baila paloma de Juan turuntún (or durundún) [sic]
‘Turun tún tún
Turun tun tún!’
(Dance dove of Juan confused or disoriented
Confused, confused!)
(1910, 402)
See also El Coco; El Cucui; El Kookoóee; Los Matachines
En lo alto de una abrupta cerrania
etc
```
In this example, we use the -v option to print all lines in the Abernathy/ch1.txt file that do not contain the word "the", and all lines in the Castro/chA file that do not contain the word "el".

## Option 4: -c (count matches)
This option prints the count of matches instead of printing the matched lines.
Source: Chat-GPT

### Examples:

```
$ grep -c "brown" ./non-fiction/OUP/Abernathy/ch1.txt
0
$ grep -c "the" ./non-fiction/OUP/Abernathy/ch1.txt
68
```
In thess examples, we use the -c option to count the number of times the words "brown" and the appears in the ch1.txt file..
