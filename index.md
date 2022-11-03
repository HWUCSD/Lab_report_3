1. less -N file
2. less +F file
3. less file1 file2

> less -N file

```shell
[root@k8s-master Media]# pwd
/home/ct/Desktop/docsearch-main/technical/government/Media
[root@k8s-master Media]# less -N Weak_economy.txt
      1 
      2 
      3 
      4 
      5 The Baltimore Sun
      6 
      7 Weak economy, court challenge threaten legal services'
      8 funding
      9 Advocates turning to state for financial assistance
     10 
     11 Andrea F. Siegel
     12 Saturday, January 11, 2003
     13 The main funding source for Maryland's legal services to the
     14 poor has fallen on hard times, and advocates are preparing to seek
     15 unprecedented state financial help - even as they keep an eye on a
     16 legal challenge that threatens to cut off a main source of funding
     17 for such services nationwide.
     18 The Maryland Legal Services Corp. - which supports 28
     19 organizations providing legal help to those with cases involving
     20 domestic abuse, landlord-tenant disputes and other issues - faces a
     21 $1 million budget shortfall because of slack interest on the
     22 accounts that help fund it.
     23 The state's chief judge is seeking a $1.2 million subsidy to
     24 close the gap in the organization's $7 million annual budget, and
     25 advocates are planning a strong push in the General Assembly.
     26 "You can bet we will be doing every kind of lobbying we can do
     27 for our funding," said Wilhelm H. Joseph Jr., executive director of
     28 the Maryland Legal Aid Bureau, the largest provider of legal help
     29 to the poor. The bureau receives $3.4 million of its $15 million
     30 budget from the Maryland Legal Services Corp., which was

```

-The N option is to display the line number of each line.



> less +F file

Scroll forward, and keep trying to read when the end of file is reached. Normally this command would be used when already at the end of the file. It is a way to monitor the tail of a file which is growing while it is being viewed. (The behavior is similar to the “tail -f” command.)

```shell
[root@k8s-master Media]# pwd
/home/ct/Desktop/docsearch-main/technical/government/Media
[root@k8s-master Media]# less +F Weak_economy.txt
"Everyone else ... is looking for more funding in a year when
there is a $1 billion shortfall," said House Speaker Michael E.
Busch, an Anne Arundel County Democrat.
"Everybody has taken a big hit," said Senate President Thomas V.
Mike Miller, a Prince George's County Democrat. "I do believe the
legislators will look askance at new issues."
A spokesman for Gov.-elect Robert L. Ehrlich Jr. said the
incoming administration could make no funding promises.
Advocates are looking at other ways to generate money.
A letter-writing campaign asks every lawyer in Maryland to
donate "at least the dollar value of one billable hour" - typically
a couple of hundred dollars - to the Legal Aid Bureau.
Check, in lieu of work
Starting next month, lawyers must report to the courts how much
free or low-fee legal work they do for the poor and charities, with
a goal of 50 hours a year.
Though many lawyers provide such services, they are also being
urged to write a check to a legal-services organization in lieu of
the hours.
Advocates also might borrow ideas from other states. Tennessee
has a surcharge on speeding tickets, Ohio assesses an annual lawyer
registration fee, and Texas uses dollars from its Crime Victims
Compensation Fund for such programs.
Maryland has a surcharge on court filing fees that goes to legal
services for the needy.





Waiting for data... (interrupt to abort)

```

The result only displays the last paragraph, and the data can be displayed in real time when inserted in real time.

**just:**

```shell
[root@k8s-master Media]# echo "new contents1" >> Weak_economy.txt 
```

**Then the result is transformed into:**

```bash
"Everyone else ... is looking for more funding in a year when
there is a $1 billion shortfall," said House Speaker Michael E.
Busch, an Anne Arundel County Democrat.
"Everybody has taken a big hit," said Senate President Thomas V.
Mike Miller, a Prince George's County Democrat. "I do believe the
legislators will look askance at new issues."
A spokesman for Gov.-elect Robert L. Ehrlich Jr. said the
incoming administration could make no funding promises.
Advocates are looking at other ways to generate money.
A letter-writing campaign asks every lawyer in Maryland to
donate "at least the dollar value of one billable hour" - typically
a couple of hundred dollars - to the Legal Aid Bureau.
Check, in lieu of work
Starting next month, lawyers must report to the courts how much
free or low-fee legal work they do for the poor and charities, with
a goal of 50 hours a year.
Though many lawyers provide such services, they are also being
urged to write a check to a legal-services organization in lieu of
the hours.
Advocates also might borrow ideas from other states. Tennessee
has a surcharge on speeding tickets, Ohio assesses an annual lawyer
registration fee, and Texas uses dollars from its Crime Victims
Compensation Fund for such programs.
Maryland has a surcharge on court filing fees that goes to legal
services for the needy.





new contents1
Waiting for data... (interrupt to abort)

```

> less file1 file2

use less command  view multiple files at once.

```shell
[root@k8s-master Media]# pwd
/home/ct/Desktop/docsearch-main/technical/government/Media
[root@k8s-master Media]# less Weak_economy.txt Working_for_Free.txt 
The Baltimore Sun

Weak economy, court challenge threaten legal services'
funding
Advocates turning to state for financial assistance

Andrea F. Siegel
Saturday, January 11, 2003
The main funding source for Maryland's legal services to the
poor has fallen on hard times, and advocates are preparing to seek
unprecedented state financial help - even as they keep an eye on a
legal challenge that threatens to cut off a main source of funding
for such services nationwide.
The Maryland Legal Services Corp. - which supports 28
organizations providing legal help to those with cases involving
domestic abuse, landlord-tenant disputes and other issues - faces a
$1 million budget shortfall because of slack interest on the
accounts that help fund it.
The state's chief judge is seeking a $1.2 million subsidy to
close the gap in the organization's $7 million annual budget, and
advocates are planning a strong push in the General Assembly.
"You can bet we will be doing every kind of lobbying we can do
for our funding," said Wilhelm H. Joseph Jr., executive director of
the Maryland Legal Aid Bureau, the largest provider of legal help
to the poor. The bureau receives $3.4 million of its $15 million
budget from the Maryland Legal Services Corp., which was
Weak_economy.txt (file 1 of 2)
...
there is a $1 billion shortfall," said House Speaker Michael E.
Busch, an Anne Arundel County Democrat.
"Everybody has taken a big hit," said Senate President Thomas V.
Mike Miller, a Prince George's County Democrat. "I do believe the
legislators will look askance at new issues."
A spokesman for Gov.-elect Robert L. Ehrlich Jr. said the
incoming administration could make no funding promises.
Advocates are looking at other ways to generate money.
A letter-writing campaign asks every lawyer in Maryland to
donate "at least the dollar value of one billable hour" - typically
a couple of hundred dollars - to the Legal Aid Bureau.
Check, in lieu of work
Starting next month, lawyers must report to the courts how much
free or low-fee legal work they do for the poor and charities, with
a goal of 50 hours a year.
Though many lawyers provide such services, they are also being
urged to write a check to a legal-services organization in lieu of
the hours.
Advocates also might borrow ideas from other states. Tennessee
has a surcharge on speeding tickets, Ohio assesses an annual lawyer
registration fee, and Texas uses dollars from its Crime Victims
Compensation Fund for such programs.
Maryland has a surcharge on court filing fees that goes to legal
services for the needy.





new contents1
(END) - Next: Working_for_Free.txt

:n                    
Working for Free Pays Off for Caring Lawyer
Bruce Zucker chooses to provide pro bono legal aid to poor
tenants over more prestigious work, and it has become his life's
passion.

Karima A. Haynes
Sunday, January 5, 2003
Nothing in Bruce Zucker's upbringing seems to have prepared him
for his life's work defending the poor.
A tall, athletic man who favors pleated khakis and starched
button-down shirts, Zucker grew up in an upper-middle-class enclave
in the west San Fernando Valley, far from the poverty he now sees
every day.
At Taft High School and UCLA, Zucker said, the closest brush
with poverty was reading newspaper articles about unscrupulous
bosses withholding wages from garment district workers.
Before graduating from Loyola Law School in 1993, Zucker
interviewed with a prestigious Santa Monica law firm and deftly
matched wits with the partners over lunch at an upscale restaurant.
Yet as he chatted amiably with the partners, something wasn't quite
right.
"I just didn't get the impression that they were really happy,"
Zucker said. "They seemed to be more passionate about their weekend
plans than the work they were doing."
After the meeting, Zucker realized he had to ask himself some
fundamental questions. What was his life's passion? What work would
Working_for_Free.txt (file 2 of 2)

```

that's because:

```csharp
      :n     Examine  the next file (from the list of files given in the com‐
              mand line).  If a number N is specified, the N-th next  file  is
              examined.
       :p     Examine the previous file in the command line list.  If a number
              N is specified, the N-th previous file is examined.
```



## find

1. find path -name file_name
2. find path -empty
3. find path -size file_size

>find path -name file_name

-The name option specifies the mode of the file name to be found. This pattern can be either a wildcard or a regular expression. In the following example, '*y.txt 'can match all files or directories whose names end in "y. txt".

```shell
[root@k8s-master technical]# pwd
/home/ct/Desktop/docsearch-main/technical
[root@k8s-master technical]# find . -name "*y.txt"
./government/Env_Prot_Agen/section-by-section_summary.txt
./government/Media/Federal_agency.txt
./government/Media/Lawyer_Web_Survey.txt
./government/Media/Legal_Aid_Society.txt
./government/Media/Legal_Aid_attorney.txt
./government/Media/Legal_Aid_in_Clay_County.txt
./government/Media/Lindsays_legacy.txt
./government/Media/Service_Agency.txt
./government/Media/Survey.txt
./government/Media/Towson_Attorney.txt
./government/Media/highlight_Senior_Day.txt
./government/Media/residents_sue_city.txt
./government/Media/Weak_economy.txt
./government/Post_Rate_Comm/Cohenetal_RuralDelivery.txt
./government/Post_Rate_Comm/Redacted_Study.txt

```



> find path -name file_name

The find command supports the - empty option to retrieve empty files or directories. An empty file means that there is no content in the file, and an empty directory means that there is no file or subdirectory in the directory.

```shell
[root@k8s-master technical]# pwd
/home/ct/Desktop/docsearch-main/technical
[root@k8s-master technical]# find . -empty
[root@k8s-master technical]# cd ./government/Media/
[root@k8s-master Media]# touch empty.txt     
[root@k8s-master Media]# cd ..
[root@k8s-master government]# cd ..
[root@k8s-master technical]# find . -empty
./government/Media/empty.txt
```



> find path -size file_size

Find all files smaller than 2k

```shell
[root@k8s-master technical]# find . -size -2k
.
./government
./government/Alcohol_Problems
./government/Media/empty.txt
./plos/pmed.0020191.txt
./plos/pmed.0020226.txt

```



## grep

1. grep -n
2. grep -i
3. grep -v



>grep -n

Show matching lines and line numbers:

```shell
[root@k8s-master Media]# pwd
/home/ct/Desktop/docsearch-main/technical/government/Media
[root@k8s-master Media]# grep A Weak_economy.txt  -n
```

![image-20221101193911721](.\imgs\img1.png)



> grep -i

Match case insensitive

```shell
[root@k8s-master Media]# grep we Weak_economy.txt  -i
```

![image-20221101194026680](.\imgs\img2.png)



> grep -v

“grep - v” is the reverse text line search.

When there are many console outputs, many of which we do not want to see, we can use the “grep - v” command. For example:



For all files that conform to the regular expression "* all" format, select the content that does not contain the "test" line, and display the line number.

```shell
[root@k8s-master Media]# grep -v test *all* -n
Justice_for_all.txt:1:
Justice_for_all.txt:2:
Justice_for_all.txt:3:
Justice_for_all.txt:4:
Justice_for_all.txt:5:Justice for all is a never-ending quest
Justice_for_all.txt:6:Documentary shows how Legal Services aids people who have
Justice_for_all.txt:7:nowhere else to turn
Justice_for_all.txt:8:
Justice_for_all.txt:9:By Rudy Larini
Justice_for_all.txt:10:Thursday, January 23, 2003
Justice_for_all.txt:11:After becoming disabled in a machete attack on a visit to his
Justice_for_all.txt:12:native Haiti, Jean-Claude Joseph needed help persuading his
Justice_for_all.txt:13:landlord to move him from a fifth-floor apartment to one on the
Justice_for_all.txt:14:ground floor.
Justice_for_all.txt:15:Isaac Benjamin became ensnared in a bureaucratic snafu that took
Justice_for_all.txt:16:away his Social Security disability payments for more than two
Justice_for_all.txt:17:years.
Justice_for_all.txt:18:The story of Martha, a woman from Sierra Leone, was more
Justice_for_all.txt:19:compelling. Beaten, raped and tortured in her politically
Justice_for_all.txt:20:repressive homeland, she knowingly used someone else's passport to
Justice_for_all.txt:21:escape to America, but was caught by immigration authorities upon
Justice_for_all.txt:22:her arrival. She desperately sought political asylum.
Justice_for_all.txt:23:Not the kind of cases that lead to ground-breaking upheavals in
Justice_for_all.txt:24:the law, but the kind of cases that are handled day in and day out
Justice_for_all.txt:25:by lawyers for the legally disenfranchised who have no where else
Justice_for_all.txt:26:to turn.
Justice_for_all.txt:27:The work of attorneys from Legal Services of New Jersey will be
Justice_for_all.txt:28:highlighted in a onehour documentary, "Quest for Justice," to be
Justice_for_all.txt:29:aired 9 p.m. today on New Jersey Network. Produced by NYD2, a
Justice_for_all.txt:30:communications firm based in Somerset, the documentary features
Justice_for_all.txt:31:case histories of clients whose needs ranged from housing to
Justice_for_all.txt:32:fighting off deportation.
Justice_for_all.txt:33:Joseph, a 54-year-old naturalized citizen, turned to Legal
Justice_for_all.txt:34:Services when the landlord of his federally subsidized apartment
Justice_for_all.txt:35:complex in Elizabeth turned a deaf ear to his request for a
Justice_for_all.txt:36:ground-floor apartment.
Justice_for_all.txt:37:Having lost the use of his left arm in warding off the machete
Justice_for_all.txt:38:attack during a robbery attempt, Joseph said he found it
Justice_for_all.txt:39:increasingly difficult to negotiate the five flights of stairs
Justice_for_all.txt:40:lugging groceries or laundry on the frequent occasions when the
Justice_for_all.txt:41:building's elevator was out of order.
Justice_for_all.txt:42:"With this, it became impossible for me to stay upstairs," he
Justice_for_all.txt:43:said, pointing to the scars on his forearm. "If I cannot carry my
Justice_for_all.txt:44:groceries or my laundry, how can I live?"
Justice_for_all.txt:45:"It was a compelling case," said Legal Services attorney Stephen
Justice_for_all.txt:46:St. Hilaire. "The key for us -- and we have to make tough decisions
Justice_for_all.txt:47:all the time on whether to take a case -- was visualizing what he
Justice_for_all.txt:48:had to do to get to the fifth floor, struggling with a bag of
Justice_for_all.txt:49:groceries," he said.
Justice_for_all.txt:50:Benjamin, 53, of Jersey City had been collecting Social Security
Justice_for_all.txt:51:disability after undergoing double bypass surgery when the checks
Justice_for_all.txt:52:stopped coming. He said the agency claimed he had failed to return
Justice_for_all.txt:53:a form updating the condition of his health.
Justice_for_all.txt:54:"But what got me was they didn't let me know they didn't get it,
Justice_for_all.txt:55:they just cut me off," he said, adding he found it impossible to
Justice_for_all.txt:56:negotiate the Social Security bureaucracy himself.
Justice_for_all.txt:57:"When I would call them up or go up there, they would give me
Justice_for_all.txt:58:blank stares," he said. "I didn't know what to do."
Justice_for_all.txt:59:So he contacted Legal Services and his case was assigned to
Justice_for_all.txt:60:paralegal David Morris.
Justice_for_all.txt:61:"Isaac's case was one of government screw-ups," Morris said,
Justice_for_all.txt:62:recounting how Social Security shuffled his file from New Jersey to
Justice_for_all.txt:63:Baltimore and then Philadelphia before finally tracking it down.
Justice_for_all.txt:64:Legal Services eventually got Benjamin's benefits restored.
Justice_for_all.txt:65:Martha, who does not want her last name used, believes she owes
Justice_for_all.txt:66:her very life to Legal Services and lawyer Laura Adjangba, who won
Justice_for_all.txt:67:her political asylum in the United States.
Justice_for_all.txt:68:"This is a great thing she has done for me in this world," she
Justice_for_all.txt:69:said as tears welled up in her eyes. "God just brought her to take
Justice_for_all.txt:70:care of my problem."
Justice_for_all.txt:71:In New Jersey, Legal Services has represented more than 1.3
Justice_for_all.txt:72:million clients since the program was conceived during President
Justice_for_all.txt:73:Lyndon Johnson's War on Poverty in the mid1960s.
Justice_for_all.txt:74:In a survey last year, Legal Services determined that more than
Justice_for_all.txt:75:one-third of New Jersey's poor adults -- more than 400,000 people
Justice_for_all.txt:76:-- have at least one civil legal problem a year. There are Legal
Justice_for_all.txt:77:Services offices in every county except Salem and they handle
Justice_for_all.txt:78:roughly 50,000 cases a year.
Justice_for_all.txt:79:New Jersey has a Legal Services budget of almost $38 million and
Justice_for_all.txt:80:a staff of 500, including about 200 attorneys.
Justice_for_all.txt:81:The lawyers, many of whom could be earning considerably more in
Justice_for_all.txt:82:the private sector, are uniformly devoted to the principle of
Justice_for_all.txt:83:providing legal assistance to those who otherwise might be denied
Justice_for_all.txt:84:their day in court.
Justice_for_all.txt:85:"People often say, 'Oh, you work with Legal Services because you
Justice_for_all.txt:86:couldn't work for a big firm with 300 people,'" attorney Grayce
Justice_for_all.txt:87:Wiggins explains on the documentary. "People that work at Legal
Justice_for_all.txt:88:Services are committed to the mission of legal services. This is
Justice_for_all.txt:89:more than just a job. This is about changing people's lives."
Justice_for_all.txt:90:"With this group, you hear them regularly say to a person they
Justice_for_all.txt:91:are honored to practice this kind of law," said Michael DeFabrizio,
Justice_for_all.txt:92:an NYD2 vice president and the executive producer of the
Justice_for_all.txt:93:documentary.
Justice_for_all.txt:94:In the opening segment of the documentary, Nicholas deB.
Justice_for_all.txt:95:Katzenbach, who was U.S. attorney general under Johnson, scoffs at
Justice_for_all.txt:96:the notion that Legal Services is just another government
Justice_for_all.txt:97:handout.
Justice_for_all.txt:98:"I think many people think of Legal Services as something
Justice_for_all.txt:99:charitable," he said. "The purpose of Legal Services is not to give
Justice_for_all.txt:100:something to the poor other than the justice that every person is
Justice_for_all.txt:101:entitled to."
Justice_for_all.txt:102:Does DeFabrizio believe his documentary will help convince
Justice_for_all.txt:103:people of the need for the kind of help offered by Legal
Justice_for_all.txt:104:Services?
Justice_for_all.txt:105:"You hope that the public cares," he said. "Civilization really
Justice_for_all.txt:106:depends on human beings caring about other human beings."
Justice_for_all.txt:107:
Justice_for_all.txt:108:
Justice_for_all.txt:109:
Justice_for_all.txt:110:
Valley_Needing_Legal_Services.txt:1:
Valley_Needing_Legal_Services.txt:2:
Valley_Needing_Legal_Services.txt:3:
Valley_Needing_Legal_Services.txt:4:
Valley_Needing_Legal_Services.txt:5:Valley Needing Legal Services
Valley_Needing_Legal_Services.txt:6:McALLEN (AP) - The consolidation of legal services agencies for
Valley_Needing_Legal_Services.txt:7:the poor may improve efficiency, but won't increase the number of
Valley_Needing_Legal_Services.txt:8:clients served, a rural legal specialist in South Texas says.
Valley_Needing_Legal_Services.txt:9:David Hall, director of Texas Rural Legal Aid in Weslaco, said
Valley_Needing_Legal_Services.txt:10:legal services for the poor in the Rio Grande Valley are inadequate
Valley_Needing_Legal_Services.txt:11:and need a dramatic increase in funding.
Valley_Needing_Legal_Services.txt:12:"We've got one lawyer for every 30,000 poor people in the
Valley_Needing_Legal_Services.txt:13:Valley," Hall said in Sunday's editions of The Monitor
Valley_Needing_Legal_Services.txt:14:(McAllen).
Valley_Needing_Legal_Services.txt:15:As part of a nationwide overhaul of Legal Services Corp. to get
Valley_Needing_Legal_Services.txt:16:more poor people legal help, nine legal aid groups in Texas are
Valley_Needing_Legal_Services.txt:17:being folded into three, creating mega-programs involving dozens of
Valley_Needing_Legal_Services.txt:18:counties across thousands of miles.
Valley_Needing_Legal_Services.txt:19:John McKay, president of the organization, said the refocused
Valley_Needing_Legal_Services.txt:20:and larger programs can raise more money, find more lawyers and
Valley_Needing_Legal_Services.txt:21:increase the number of poor people who get help through the civil
Valley_Needing_Legal_Services.txt:22:courts system.
Valley_Needing_Legal_Services.txt:23:The programs, supplemented by funding from state governments,
Valley_Needing_Legal_Services.txt:24:bar associations and foundations, provide free legal help to the
Valley_Needing_Legal_Services.txt:25:poor but not in criminal cases.
Valley_Needing_Legal_Services.txt:26:But Hall said what's needed is more money. He said his group
Valley_Needing_Legal_Services.txt:27:takes on about 10,000 cases per year with a staff of eight or nine
Valley_Needing_Legal_Services.txt:28:attorneys.
Valley_Needing_Legal_Services.txt:29:Of the $329 million appropriated by Congress to Legal Services
Valley_Needing_Legal_Services.txt:30:Corp. this year, the Valley receives about $15 million to $20
Valley_Needing_Legal_Services.txt:31:million and employs about 37 staff lawyers. Organizations that
Valley_Needing_Legal_Services.txt:32:provide free or "pro bono" services are able to maintain a better
Valley_Needing_Legal_Services.txt:33:lawyer-to-client ratio because they often specialize in particular
Valley_Needing_Legal_Services.txt:34:kinds of cases, Hall said. Even accounting for pro bono work, as
Valley_Needing_Legal_Services.txt:35:much as 90 percent of the legal needs of the poor go unmet,
Valley_Needing_Legal_Services.txt:36:according to Bill Underwood, a law professor at Baylor
Valley_Needing_Legal_Services.txt:37:University.
Valley_Needing_Legal_Services.txt:38:"If every lawyer in the state of Texas was doing pro bono work,
Valley_Needing_Legal_Services.txt:39:then that still wouldn't be enough," he said.
Valley_Needing_Legal_Services.txt:40:Underwood said one lawyer working full-time for a legal services
Valley_Needing_Legal_Services.txt:41:group can accomplish as much as 20 lawyers doing part-time pro bono
Valley_Needing_Legal_Services.txt:42:work on a similar case.
Valley_Needing_Legal_Services.txt:43:"The problem is, there's never been adequate public funding," he
Valley_Needing_Legal_Services.txt:44:said.
Valley_Needing_Legal_Services.txt:45:But Ken Boehm, a former counsel to the LSC board said a lack of
Valley_Needing_Legal_Services.txt:46:funding for the federal LSC program is not the problem, it needs
Valley_Needing_Legal_Services.txt:47:reform
Valley_Needing_Legal_Services.txt:48:
Valley_Needing_Legal_Services.txt:49:
Valley_Needing_Legal_Services.txt:50:

```
