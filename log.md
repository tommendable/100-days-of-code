# 100 Days Of Code - Log

### Day 1: 4th January, 2017

**Today's Progress**: 
* Set up Github and learnt how to create a repository, create a branch, make changes and push them to GitHub as commits and how to open and merge a pull request.
* Started work on a CSS replica of a friend's business logo (an hourglass with sharp angles)

**Thoughts:** 
* Would be good to animate the sand running out of the hourglass. I should investigate whether to do this purely with CSS or with canvas and javascript... Or perhaps I should implement both solutions as practice.

**Link to work:** 
* [Hello World Repo](https://github.com/tommendable/hello-world "Hello World Repo")
* [TimesUp Logo - CSS](http://codepen.io/tomlittlechild/full/ZLEOVW/ "TimesUp Logo")

### Day 2: 5th January, 2017

**Today's Progress**: 
* Completed Intermediate Algorithm Script - Spinal Tap Case
* Completed Intermediate Algorithm Script - Sum All Odd Fibonacci Numbers
* Completed Intermediate Algorithm Script - Sum All Primes

**Thoughts:** 
* The Spinal Tap Case gave me more trouble than it should have, I think I need to spend more time with regular expressions

**Link to work:** 
* [Spinal Tap Case Solution](https://www.freecodecamp.com/challenges/spinal-tap-case#?solution=%0Afunction%20spinalCase(str)%20%7B%0A%20%20%2F%2F%20%22It%27s%20such%20a%20fine%20line%20between%20stupid%2C%20and%20clever.%22%0A%20%20%2F%2F%20--David%20St.%20Hubbins%0A%20%20str%20%3D%20str.replace(%2F%5CW%7C%5B_%5D%2Fgi%2C%22%20%22)%3B%0A%20%20var%20arr%20%20%3D%20str.split(%2F(%3F%3D%5BA-Z%5D)%7C%5Cs%2F)%3B%0A%20%20for%20(i%20%3D%200%3B%20i%20%3C%20arr.length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20arr%5Bi%5D%20%3D%20arr%5Bi%5D.toLowerCase()%3B%0A%20%20%7D%0A%20%20str%20%3D%20arr.join(%22-%22)%3B%0A%20%20return%20str%3B%0A%7D%0A%0AspinalCase(%27AllThe-small%20Things%27)%3B%0A "Spinal Tap Case Solution")
* [Sum All Odd Fibonacci Numbers Solution](https://www.freecodecamp.com/challenges/sum-all-odd-fibonacci-numbers#?solution=%0Afunction%20sumFibs(num)%20%7B%0A%20%20var%20before%20%3D%200%3B%0A%20%20var%20now%20%3D%201%3B%0A%20%20var%20total%20%3D%200%3B%0A%20%20while(now%20%3C%3D%20num)%20%7B%0A%20%20%20%20if%20(now%20%25%202%20!%3D%3D%200)%20%7B%0A%20%20%20%20%20%20total%2B%3Dnow%3B%0A%20%20%20%20%7D%0A%20%20%20%20now%20%2B%3D%20before%3B%0A%20%20%20%20before%20%3D%20now%20-%20before%3B%0A%20%20%7D%0A%20%20return%20total%3B%0A%7D%0A%0AsumFibs(1)%3B%0A "Sum All Odd Fibonacci Numbers Solution")
* [Sum All Primes Solution](https://www.freecodecamp.com/challenges/sum-all-primes?solution=%0Afunction%20sumPrimes(num)%20%7B%0A%20%20var%20total%20%3D%200%3B%0A%20%20for%20(i%20%3D%202%3B%20i%20%3C%3D%20num%3B%20i%2B%2B)%20%7B%0A%20%20%20%20var%20test%20%3D%20true%3B%0A%20%20%20%20for%20(j%20%3D%202%3B%20j%20%3C%20i%3B%20j%2B%2B)%20%7B%0A%20%20%20%20%20%20if%20(i%20%25%20j%20%3D%3D%3D%200)%20%7B%0A%20%20%20%20%20%20%20%20test%20%3D%20false%3B%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20if%20(test%20%3D%3D%3D%20true)%20%7B%0A%20%20%20%20%20%20total%2B%3Di%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20total%3B%0A%7D%0A%0AsumPrimes(10)%3B%0A "Sum All Primes Solution")

### Day 3: 6th January, 2017

**Today's Progress**: 
* Completed Intermediate Algorithm Script - Smallest Common Multiple
* Completed Intermediate Algorithm Script - Finders Keepers
* Completed Intermediate Algorithm Script - Drop it

**Thoughts:** 
* While all of my algorithm solutions work (eventually) I feel like some of them take too long to find the solution, they sometimes lack finesse and take more of a brute force approach. I would like to work on implementing more optimised solutions.

**Link to work:** 
* [Smallest Common Multiple Solution](https://www.freecodecamp.com/challenges/Smallest%20Common%20Multiple?solution=%2F%2F%20noprotect%0Afunction%20smallestCommons(arr)%20%7B%0A%20%20var%20lcm%20%3D%200%3B%0A%20%20var%20test%20%3D%201%3B%0A%20%20arr.sort()%3B%0A%20%20for%20(i%20%3D%20arr%5B0%5D%20%2B%201%3B%20i%20%3C%20arr%5B1%5D%3B%20i%2B%2B)%20%7B%0A%20%20%20%20arr.push(i)%3B%0A%20%20%7D%0A%20%20while(test%20!%3D%3D%200)%20%7B%0A%20%20%20%20lcm%2B%2B%3B%0A%20%20%20%20var%20arr2%20%3D%20arr.sort(function(a%2Cb)%20%7Breturn%20a-b%3B%7D)%3B%0A%20%20%20%20arr2%20%3D%20arr2.map(function(x)%7Breturn%20lcm%20%25%20x%3B%7D)%3B%0A%20%20%20%20test%20%3D%20arr2.reduce(function(a%2Cb)%20%7Breturn%20a%2Bb%3B%7D%2C0)%0A%20%20%7D%0A%20%20return%20lcm%3B%0A%7D%0A%0A%0AsmallestCommons(%5B1%2C13%5D)%3B%0A "Smallest Common Multiple Solution")
* [Finders Keepers Solution](https://www.freecodecamp.com/challenges/Finders%20Keepers?solution=%0Afunction%20findElement(arr%2C%20func)%20%7B%0A%20%20arr%20%3D%20arr.filter(func)%3B%0A%20%20return%20arr%5B0%5D%3B%0A%7D%0A%0AfindElement(%5B1%2C%202%2C%203%2C%204%5D%2C%20function(num)%7B%20return%20num%20%25%202%20%3D%3D%3D%200%3B%20%7D)%3B%0A "Finders Keepers Solution")
* [Drop it Solution](https://www.freecodecamp.com/challenges/Drop%20it?solution=%0Afunction%20dropElements(arr%2C%20func)%20%7B%0A%20%20var%20fltrarr%20%3D%20arr.filter(func)%3B%0A%20%20var%20i%20%3D%20arr.indexOf(fltrarr%5B0%5D)%3B%0A%20%20if%20(i%20%3C%200)%20%7B%0A%20%20%20%20return%20%5B%5D%3B%0A%20%20%7D%20else%20%7B%0A%20%20return%20arr.slice(i)%3B%0A%20%20%7D%0A%7D%0A%0AdropElements(%5B1%2C%202%2C%203%2C%204%5D%2C%20function(n)%20%7Breturn%20n%20%3E%205%3B%20%7D)%3B%0A "Drop it Solution")

### Day 4: 7th January, 2017

**Today's Progress**: 
* Today I worked on the javacript drum kit project from Wes Bos Javascript30 course. I followed along with the video to create the project but I had an issue with the sound not working. I then personalised the appearance for some cSS practice.

**Thoughts:** 
* Not sure why the sounds were not working. perhaps the file name? uploaded to codepen anyway (without sounds).

**Link to work:** 
* [JS Drumkit](http://codepen.io/tomlittlechild/full/rjVvVV/ "JS Drumkit")

### Day 5: 8th January, 2017

**Today's Progress**: 
* Completed Intermediate Algorithm Script - Steamroller
* Today I also fixed the sound on the javascript30 drum kit project

**Thoughts:** 
* I had real trouble with the Steamroller algorithm, I expect because I haven't done much involving recursion before. For the javascript drumkit I got the sound working locally but need to host it somewhere as I don't believe codepen has anywhere to store audio files. I'd also now like to edit the look of it some more so the drums light up rather than overlaid buttons.

**Link to work:** 
* [Steamroller solution](https://www.freecodecamp.com/challenges/steamroller#?solution=%0Afunction%20steamrollArray(arr)%20%7B%0A%20%20var%20flat%20%3D%20%5B%5D%3B%0A%20%20%0A%20%20function%20flatten(arg)%20%7B%0A%20%20%20%20if%20(!Array.isArray(arg))%20%7B%0A%20%20%20%20%20%20flat.push(arg)%3B%0A%20%20%20%20%7D%20else%20%7B%0A%20%20%20%20%20%20for%20(var%20a%20in%20arg)%20%7B%0A%20%20%20%20%20%20%20%20flatten(arg%5Ba%5D)%3B%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20%0A%20%20arr.forEach(flatten)%3B%0A%20%20return%20flat%3B%0A%7D%0A%0AsteamrollArray(%5B1%2C%20%5B2%5D%2C%20%5B3%2C%20%5B%5B4%5D%5D%5D%5D)%3B%0A "Steamroller solution")
* [JS Drumkit](http://codepen.io/tomlittlechild/full/rjVvVV/ "JS Drumkit")

### Day 6: 9th January, 2017

**Today's Progress**: 
* Completed Intermediate Algorithm Script - Binary Agents
* Completed Intermediate Algorithm Script - Everything Be True
* Completed Intermediate Algorithm Script - Arguments Optional

**Thoughts:** 
* That's the last of the Intermediate Algorithms. While I feel like I could go back over them and find more efficient or elegant solutions to the problems what I should actually do is go back and re-do the basic projects and then make some real progress on the intermediate projects, then I should host my portfolio page on the domain name I already bought.

**Link to work:** 
* [Binary Agents Solution](https://www.freecodecamp.com/challenges/binary-agents#?solution=%0Afunction%20binaryAgent(str)%20%7B%0A%20%20var%20arr%20%3D%20str.split(%27%20%27)%3B%0A%20%20var%20digits%20%3D%20arr.map(function(x)%20%7Breturn%20parseInt(x%2C2)%3B%7D)%3B%0A%20%20var%20sentence%20%3D%20%22%22%3B%0A%20%20for%20(i%20%3D%200%3B%20i%20%3C%20digits.length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20sentence%20%2B%3D%20String.fromCharCode(digits%5Bi%5D)%3B%0A%20%20%7D%0A%20%20return%20sentence%3B%0A%7D%0A%0AbinaryAgent(%2201000001%2001110010%2001100101%2001101110%2000100111%2001110100%2000100000%2001100010%2001101111%2001101110%2001100110%2001101001%2001110010%2001100101%2001110011%2000100000%2001100110%2001110101%2001101110%2000100001%2000111111%22)%3B%0A "Binary Agents Solution")
* [Everything Be True Solution](https://www.freecodecamp.com/challenges/everything-be-true#?solution=%0Afunction%20truthCheck(collection%2C%20pre)%20%7B%0A%20%20for%20(i%20%3D%200%3B%20i%20%3C%20collection.length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20if%20(!collection%5Bi%5D%5Bpre%5D)%20%7B%0A%20%20%20%20%20%20return%20false%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20true%3B%0A%7D%0A%0AtruthCheck(%5B%7B%22user%22%3A%20%22Tinky-Winky%22%2C%20%22sex%22%3A%20%22male%22%7D%2C%20%7B%22user%22%3A%20%22Dipsy%22%2C%20%22sex%22%3A%20%22male%22%7D%2C%20%7B%22user%22%3A%20%22Laa-Laa%22%2C%20%22sex%22%3A%20%22female%22%7D%2C%20%7B%22user%22%3A%20%22Po%22%2C%20%22sex%22%3A%20%22female%22%7D%5D%2C%20%22sex%22)%3B%0A "Everything Be True Solution")
* [Arguments Optional Solution](https://www.freecodecamp.com/challenges/arguments-optional#?solution=%0Afunction%20addTogether()%20%7B%0A%20%20function%20checkNum(x)%20%7Bif%20(typeof%20x%20%3D%3D%3D%20%22number%22%20%26%26%20!isNaN(x))%20%7Breturn%20true%3B%7D%20else%20%7Breturn%20false%3B%7D%7D%0A%20%20if%20(arguments.length%20%3C%202)%20%7B%0A%20%20%20%20if%20(!checkNum(arguments%5B0%5D))%20%7B%0A%20%20%20%20%20%20return%20undefined%3B%0A%20%20%20%20%7D%20else%20%7B%0A%20%20%20%20%20%20var%20a%20%3D%20arguments%5B0%5D%3B%0A%20%20%20%20%20%20return%20function%20sum(b)%20%7B%0A%20%20%20%20%20%20%20%20if%20(!checkNum(b))%20%7B%0A%20%20%20%20%20%20%20%20%20%20return%20undefined%3B%0A%20%20%20%20%20%20%20%20%7D%20else%20%7B%0A%20%20%20%20%20%20%20%20return%20a%20%2B%20b%3B%0A%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%7D%3B%0A%20%20%20%20%7D%0A%20%20%7D%20else%20%7B%0A%20%20%20%20%20%20if%20(!checkNum(arguments%5B0%5D)%20%7C%7C%20!checkNum(arguments%5B1%5D))%20%7B%0A%20%20%20%20%20%20return%20undefined%3B%0A%20%20%20%20%7D%20else%20%7B%0A%20%20%20%20%20%20return%20arguments%5B0%5D%20%2B%20arguments%5B1%5D%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%7D%0A%0AaddTogether(2%2C3)%3B%0A "Arguments Optional Solution")

### Day 7: 10th January, 2017

**Today's Progress**: 
* Completed Advanced Algorithm Script - Validate US Telephone Numbers

**Thoughts:** 
* Comparing my solution to the US telephone number validation algorithm to the solution on github from freeCodeCamp really shows my lack of practice with regular expressions, my function took 23 lines, three if statements and multiple or conditionals to give desired output. The freeCodeCamp solution just defined a regular expression that encompassed all valid formats and then used the inbuilt .test method for regexp so just 2 lines. All the OR conditionals that I used just to make my solution work kind of amounts to solving case by case instead of having an overarching test to validate against. I should spend more time with regular expressions and read about them more in the documentation. 

**Link to work:** 
* [Validate US Telephone Numbers Solution](https://www.freecodecamp.com/challenges/validate-us-telephone-numbers#?solution=%0Afunction%20telephoneCheck(str)%20%7B%0A%20%20var%20num%20%3D%20str.replace(%2F%5CD%2Fg%2C'')%3B%0A%20%20function%20checkLength(num)%20%7B%0A%20%20%20%20if%20(num.length%20%3D%3D%2011%20%26%26%20num%5B0%5D%20%3D%3D%201)%20%7B%0A%20%20%20%20%20%20return%20true%3B%0A%20%20%20%20%7D%20else%20if%20(num.length%20%3D%3D%2010)%20%7B%0A%20%20%20%20%20%20return%20true%3B%0A%20%20%20%20%7D%20else%20%7B%0A%20%20%20%20%20%20return%20false%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20var%20nonum%20%3D%20str.replace(%2F%5Cd%2Fg%2C'X').replace(%2F-%2Fg%2C'%20')%3B%0A%20%20function%20checknonum(nonum)%20%7B%0A%20%20%20%20if%20(nonum%20%3D%3D%20'XXX%20XXX%20XXXX'%20%7C%7C%20nonum%20%3D%3D%20'(XXX)XXX%20XXXX'%20%7C%7C%20nonum%20%3D%3D%20'(XXX)%20XXX%20XXXX'%20%7C%7C%20nonum%20%3D%3D%20'XXXXXXXXXX'%20%7C%7C%20nonum%20%3D%3D%20'X%20XXX%20XXX%20XXXX'%20%7C%7C%20nonum%20%3D%3D%20'X%20(XXX)%20XXX%20XXXX'%20%7C%7C%20nonum%20%3D%3D%20'X(XXX)XXX%20XXXX')%20%7B%0A%20%20%20%20%20%20return%20true%3B%0A%20%20%20%20%7D%20else%20%7B%0A%20%20%20%20%20%20return%20false%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20if%20(checkLength(num)%20%26%26%20checknonum(nonum))%20%7B%0A%20%20%20%20return%20true%3B%0A%20%20%7D%20else%20%7B%0A%20%20%20%20return%20false%3B%0A%20%20%7D%0A%7D%0A%0A%0A%0AtelephoneCheck(%221%20(555)%20555-5555%22)%3B%0A "Validate US Telephone Numbers Solution")

### Day 8: 11th January, 2017

**Today's Progress**: 
* Today I worked on the javacript clock project from Wes Bos Javascript30 course.

**Thoughts:** 
* The javascript clock was fairly straight forward to create. I can probably use some of the things I have learnt from this for the Pomodoro clock project in freecode camp. Or perhaps I will create a project that is a clock but has a start / pause / stop so I can time how much I spend on coding each day for the 100 days to make sure I do at least an hour every day. This could even have an IFTTT auto tweet function.

**Link to work:** 
* [JS Clock](http://codepen.io/tomlittlechild/pen/ggPyNK "JS Clock")

### Day 9: 12th January, 2017

**Today's Progress**:
* Started on the show the local weather project from freeCodeCamp.

**Thoughts:**
* Spent a lot of time trying to get the navigator.getCurrentLocation method to work. Turned out to be due to http instead of https on codepen. Then spent even more time trying to just get the information from the open weather API. I can get the data to pull through now but I wan't it as a nested array or javascript object but all I can get is a text string. I think I need to look a bit more at the XMLHttpRequest function to get what I want to pull through.

**Link to work:**
* [Weather app](http://codepen.io/tomlittlechild/full/JEXLym/ "Weather App")

### Day 10: 13th January, 2017

**Today's Progress**:
* Today I learnt about CSS variables and how to change them with javascript by doing the third #javascript30 project

**Thoughts:**
* I also read some more of eloquent javascript today which really helped to cement some of the concepts of control flow

**Link to work:**
* [CSS variables and JS](http://codepen.io/tomlittlechild/pen/pRbeeV "CSS variables and JS")

### Day 11: 15th January, 2017

**Today's Progress**:
* Completed Advanced Algorithm Script - Symmetric Difference 

**Thoughts:** 
* I feel like i could have got more coding done this weekend but i have been sick so maybe its just as well that i gave myself a break yesterday.

**Link to work:** 
* [Symmetric Difference Solution](https://www.freecodecamp.com/challenges/Symmetric%20Difference?solution=%0Afunction%20sym(args)%20%7B%0A%20%20function%20symdiff(a%2Cb)%20%7B%0A%20%20var%20arr%20%3D%20%5B%5D%2C%20is%20%3D%20%5B%5D%2C%20js%20%3D%20%5B%5D%3B%0A%20%20for%20(i%20%3D%200%3B%20i%20%3C%20b.length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20for%20(j%20%3D%200%3B%20j%20%3C%20a.length%3B%20j%2B%2B)%20%7B%0A%20%20%20%20%20%20if%20(b%5Bi%5D%20%3D%3D%3D%20a%5Bj%5D)%20%7B%0A%20%20%20%20%20%20%20%20is.push(i)%3B%0A%20%20%20%20%20%20%20%20js.push(j)%3B%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20for%20(i%20%3D%200%3B%20i%20%3C%20b.length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20if%20(is.indexOf(i)%20%3D%3D%3D%20-1%20%26%26%20arr.indexOf(b%5Bi%5D)%20%3D%3D%3D%20-1)%20%7B%0A%20%20%20%20%20%20arr.push(b%5Bi%5D)%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20for%20(j%20%3D%200%3B%20j%20%3C%20a.length%3B%20j%2B%2B)%20%7B%0A%20%20%20%20if%20(js.indexOf(j)%20%3D%3D%3D%20-1%20%26%26%20arr.indexOf(a%5Bj%5D)%20%3D%3D%3D%20-1)%20%7B%0A%20%20%20%20%20%20arr.push(a%5Bj%5D)%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20return%20arr%3B%0A%20%20%7D%0A%20%20var%20arrs%20%3D%20%5B%5D%3B%0A%20%20for%20(i%20%3D%200%3B%20i%20%3C%20arguments.length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20arrs.push(arguments%5Bi%5D)%3B%0A%20%20%7D%0A%20%20return%20arrs.reduce(symdiff)%3B%0A%7D%0A%0Asym(%5B1%2C%202%2C%203%5D%2C%20%5B5%2C%202%2C%201%2C%204%5D)%3B%0A "Symmetric Difference")

### Day 12: 16th January, 2017

**Today's Progress**:
* Completed Advanced Algorithm Script - Exact Change 
* Completed Advanced Algorithm Script - Map the Debris

**Thoughts:** 
* I only have 5 more advanced algorithms left in the front end developer certificate, then it's just the unfinished projects to go (though I would also like to revisit some of the old projects as well).

**Link to work:** 
* [Exact Change Solution](https://www.freecodecamp.com/challenges/exact-change#?solution=%0Afunction%20checkCashRegister(price%2C%20cash%2C%20cid)%20%7B%0A%20%20var%20worth%20%3D%20%5B%0A%20%20%20%20%7Bname%3A%20%22ONE%20HUNDRED%22%2C%20val%3A%20100.00%7D%2C%0A%20%20%20%20%7Bname%3A%20%22TWENTY%22%2C%20val%3A%2020.00%7D%2C%0A%20%20%20%20%7Bname%3A%20%22TEN%22%2C%20val%3A%2010.00%7D%2C%0A%20%20%20%20%7Bname%3A%20%22FIVE%22%2C%20val%3A%205.00%7D%2C%0A%20%20%20%20%7Bname%3A%20%22ONE%22%2C%20val%3A%201.00%7D%2C%0A%20%20%20%20%7Bname%3A%20%22QUARTER%22%2C%20val%3A%200.25%7D%2C%0A%20%20%20%20%7Bname%3A%20%22DIME%22%2C%20val%3A%200.10%7D%2C%0A%20%20%20%20%7Bname%3A%20%22NICKEL%22%2C%20val%3A%200.05%7D%2C%0A%20%20%20%20%7Bname%3A%20%22PENNY%22%2C%20val%3A%200.01%7D%5D%3B%0A%20%20%0A%20%20var%20delta%20%3D%20cash%20-%20price%3B%0A%20%20%0A%20%20var%20register%20%3D%20cid.reduce(function(acc%2C%20coin)%20%7B%0A%20%20%20%20acc.total%20%2B%3D%20coin%5B1%5D%3B%0A%20%20%20%20acc%5Bcoin%5B0%5D%5D%20%3D%20coin%5B1%5D%3B%0A%20%20%20%20return%20acc%3B%0A%20%20%7D%2C%20%7Btotal%3A%200%7D)%3B%0A%20%20%20%20%0A%20%20if%20(register.total%20%3C%20delta)%20%7B%0A%20%20%20%20return%20%22Insufficient%20Funds%22%3B%0A%20%20%7D%20%0A%20%20%0A%20%20if(register.total%20%3D%3D%3D%20delta)%20%7B%0A%20%20%20%20return%20%22Closed%22%3B%20%20%0A%20%20%7D%0A%20%20%0A%20%20var%20change%20%3D%20worth.reduce(function(acc%2C%20coin)%20%7B%0A%20%20%20%20var%20value%20%3D%200%3B%0A%20%20%20%20while%20(register%5Bcoin.name%5D%20%3E%200%20%26%26%20delta%20%3E%3D%20coin.val)%20%7B%0A%20%20%20%20%20%20delta%20-%3D%20coin.val%3B%0A%20%20%20%20%20%20register%5Bcoin.name%5D%20-%3D%20coin.val%3B%0A%20%20%20%20%20%20value%20%2B%3D%20coin.val%3B%0A%20%20%20%20%20%20delta%20%3D%20Math.round(delta%20*%20100)%20%2F%20100%3B%0A%20%20%20%20%7D%0A%20%20%20%20if%20(value%20%3E%200)%20%7B%0A%20%20%20%20%20%20acc.push(%5Bcoin.name%2C%20value%5D)%3B%0A%20%20%20%20%7D%0A%20%20%20%20return%20acc%3B%0A%20%20%7D%2C%20%5B%5D)%3B%0A%20%20%0A%20%20if%20(change.length%20%3C%201%20%7C%7C%20delta%20%3E%200)%20%7B%0A%20%20%20%20return%20%22Insufficient%20Funds%22%3B%0A%20%20%7D%0A%20%20%0A%20%20return%20change%3B%0A%7D%0A%0AcheckCashRegister(19.50%2C%2020.00%2C%20%5B%5B%22PENNY%22%2C%200.01%5D%2C%20%5B%22NICKEL%22%2C%200%5D%2C%20%5B%22DIME%22%2C%200%5D%2C%20%5B%22QUARTER%22%2C%200%5D%2C%20%5B%22ONE%22%2C%201.00%5D%2C%20%5B%22FIVE%22%2C%200%5D%2C%20%5B%22TEN%22%2C%200%5D%2C%20%5B%22TWENTY%22%2C%200%5D%2C%20%5B%22ONE%20HUNDRED%22%2C%200%5D%5D)%3B%0A "Exact Change Solution")
* [Map the Debris Solution](https://www.freecodecamp.com/challenges/map-the-debris#?solution=%0Afunction%20orbitalPeriod(arr)%20%7B%0A%20%20var%20GM%20%3D%20398600.4418%3B%0A%20%20var%20earthRadius%20%3D%206367.4447%3B%0A%20%20var%20periods%20%3D%20%5B%5D%3B%0A%20%20for%20(i%20%3D%200%3B%20i%20%3C%20arr.length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20var%20axis%20%3D%20arr%5Bi%5D.avgAlt%20%2B%20earthRadius%3B%0A%20%20%20%20var%20period%20%3D%20Math.round(2%20*%20Math.PI%20*%20(Math.sqrt(Math.pow(axis%2C%203)%2FGM)))%3B%0A%20%20%20%20var%20obj%20%3D%7B%7D%3B%0A%20%20%20%20obj.name%20%3D%20arr%5Bi%5D.name%3B%0A%20%20%20%20obj.orbitalPeriod%20%3D%20period%3B%0A%20%20%20%20periods.push(obj)%3B%0A%20%20%7D%0A%20%20return%20periods%3B%0A%7D%0A%0AorbitalPeriod(%5B%7Bname%3A%20%22iss%22%2C%20avgAlt%3A%20413.6%7D%2C%20%7Bname%3A%20%22hubble%22%2C%20avgAlt%3A%20556.7%7D%2C%20%7Bname%3A%20%22moon%22%2C%20avgAlt%3A%20378632.553%7D%5D)%3B%0A "Map the Debris Solution")

### Day 13: 17th January, 2017

**Today's Progress**:
* Completed Advanced Algorithm Script - Inventory Update 

**Thoughts:** 
* 

**Link to work:** 
* [Inventory Update Solution](https://www.freecodecamp.com/challenges/inventory-update#?solution=%0Afunction%20updateInventory(arr1%2C%20arr2)%20%7B%0A%20%20%20%20%2F%2F%20All%20inventory%20must%20be%20accounted%20for%20or%20you%27re%20fired!%0A%20%20var%20stockedItems%20%3D%20%7B%7D%3B%0A%20%20var%20stock%20%3D%5B%5D%3B%0A%20%20for%20(i%20%3D%200%3B%20i%20%3C%20arr1.length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20stockedItems%5Barr1%5Bi%5D%5B1%5D%5D%20%3D%20arr1%5Bi%5D%5B0%5D%3B%0A%20%20%20%20stock.push(%5Barr1%5Bi%5D%5B1%5D%5D)%3B%0A%20%20%7D%0A%20%20for%20(var%20i%20in%20arr2)%20%7B%0A%20%20%20%20if%20(stockedItems.hasOwnProperty(arr2%5Bi%5D%5B1%5D))%20%7B%0A%20%20%20%20%20%20stockedItems%5Barr2%5Bi%5D%5B1%5D%5D%20%2B%3D%20arr2%5Bi%5D%5B0%5D%3B%0A%20%20%20%20%7D%20else%20%7B%0A%20%20%20%20%20%20stockedItems%5Barr2%5Bi%5D%5B1%5D%5D%20%3D%20arr2%5Bi%5D%5B0%5D%3B%0A%20%20%20%20%20%20stock.push(%5Barr2%5Bi%5D%5B1%5D%5D)%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20stock.sort()%3B%0A%20%20for%20(var%20j%20in%20stock)%20%7B%0A%20%20%20%20stock%5Bj%5D.unshift(stockedItems%5Bstock%5Bj%5D%5B0%5D%5D)%3B%0A%20%20%7D%0A%20%20return%20stock%3B%0A%7D%0A%0A%2F%2F%20Example%20inventory%20lists%0Avar%20curInv%20%3D%20%5B%0A%20%20%20%20%5B21%2C%20%22Bowling%20Ball%22%5D%2C%0A%20%20%20%20%5B2%2C%20%22Dirty%20Sock%22%5D%2C%0A%20%20%20%20%5B1%2C%20%22Hair%20Pin%22%5D%2C%0A%20%20%20%20%5B5%2C%20%22Microphone%22%5D%0A%5D%3B%0A%0Avar%20newInv%20%3D%20%5B%0A%20%20%20%20%5B2%2C%20%22Hair%20Pin%22%5D%2C%0A%20%20%20%20%5B3%2C%20%22Half-Eaten%20Apple%22%5D%2C%0A%20%20%20%20%5B67%2C%20%22Bowling%20Ball%22%5D%2C%0A%20%20%20%20%5B7%2C%20%22Toothpaste%22%5D%0A%5D%3B%0A%0AupdateInventory(curInv%2C%20newInv)%3B%0A "Inventory Update Solution")
