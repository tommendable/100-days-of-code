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

**Thoughts:** 
* The Spinal Tap Case gave me more trouble than it should have, I think I need to spend more time with regular expressions

**Link to work:** 
* [Spinal Tap Case Solution](https://www.freecodecamp.com/challenges/spinal-tap-case#?solution=%0Afunction%20spinalCase(str)%20%7B%0A%20%20%2F%2F%20%22It%27s%20such%20a%20fine%20line%20between%20stupid%2C%20and%20clever.%22%0A%20%20%2F%2F%20--David%20St.%20Hubbins%0A%20%20str%20%3D%20str.replace(%2F%5CW%7C%5B_%5D%2Fgi%2C%22%20%22)%3B%0A%20%20var%20arr%20%20%3D%20str.split(%2F(%3F%3D%5BA-Z%5D)%7C%5Cs%2F)%3B%0A%20%20for%20(i%20%3D%200%3B%20i%20%3C%20arr.length%3B%20i%2B%2B)%20%7B%0A%20%20%20%20arr%5Bi%5D%20%3D%20arr%5Bi%5D.toLowerCase()%3B%0A%20%20%7D%0A%20%20str%20%3D%20arr.join(%22-%22)%3B%0A%20%20return%20str%3B%0A%7D%0A%0AspinalCase(%27AllThe-small%20Things%27)%3B%0A "Spinal Tap Case Solution")
* [Sum All Odd Fibonacci Numbers Solution](https://www.freecodecamp.com/challenges/sum-all-odd-fibonacci-numbers#?solution=%0Afunction%20sumFibs(num)%20%7B%0A%20%20var%20before%20%3D%200%3B%0A%20%20var%20now%20%3D%201%3B%0A%20%20var%20total%20%3D%200%3B%0A%20%20while(now%20%3C%3D%20num)%20%7B%0A%20%20%20%20if%20(now%20%25%202%20!%3D%3D%200)%20%7B%0A%20%20%20%20%20%20total%2B%3Dnow%3B%0A%20%20%20%20%7D%0A%20%20%20%20now%20%2B%3D%20before%3B%0A%20%20%20%20before%20%3D%20now%20-%20before%3B%0A%20%20%7D%0A%20%20return%20total%3B%0A%7D%0A%0AsumFibs(1)%3B%0A "Sum All Odd Fibonacci Numbers Solution")
