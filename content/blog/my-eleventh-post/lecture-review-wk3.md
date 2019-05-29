---
title: [Learning JS] Debugging with developer tools
date: '2019-05-29 16:04:14'
description: ' '
---
## 2019-05-13 18:41:22 다섯번째 수업 @ vanilla coding

------

### HTML review

------

```html
<!DOCTYPE HTML>
  <html>
    <head>
      <title>Title of a webpage</title>
      <link rel="stylesheet" href="./main.css" />
    </head>
    <body>

      <script src="./index.js"></script>
    </body>
  </html>
```

Try to write this basic structure of HTML which loads CSS and JS file without any aid! It can be trickier than you think... 

## Debugger Tools

### Network

------  
<img src="network.png" width="400" />  

In developer tools, network menu displays the files that have been downloaded when loading a website. Files that have been loaded first will be on the top of the list. 

Clicking the file on the list will display a set of new tab menus: "headers","preview","response", and "timing". 

The response tab can be used to check the contents of the file.

---
### debugger ;
--- 

<img src="debugger1.png" width="400" />  

While developer tools window is open and if 'debugger;' expression executes inside a function, the code will stop running exactly where the debugger expression is located.  
If the developer tools window is not open,, the code will not stop running even if debugger expression is read.

---
### resume 
---

<img src="resume.png" width="400" />  

Clicking on the resume button when the debugger expression has stopped the code will resume running the code. The code will only stop after pressing the resume button when there is another debugger expression in the code that is executed.  

If there is no debugger expression in the rest of the code, the code will run until the end of the file. 

---
### step over
---

<img src="stepover.png" width="400" />

Clicking on the step over button when the debugger expression has stopped the code will run the next line of execution inside the function.  

---
### mouseover on a variable
---
<img src="mouseover.png" width="400" />

Bringing cursor over a variable will display its current value. This can be useful when there is a need to check the variable's value while debugging the code.

---
### variables in local scope
---

<img src="scopevars.png" width="400" />  

On the righthand side of the debugger window, local variables and their values are shown under "scope".

