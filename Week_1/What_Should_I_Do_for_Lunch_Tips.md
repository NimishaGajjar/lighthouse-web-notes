* [Week 1](/Week_1)
  * [Day 1](/Week_1/Day_1)
  ### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
function whatToDoForLunch(hungry, availableTime) {
  if (!hungry) {
    console.log("Hey, Get back to work");
  }

  else {
    console.log("Have lunch");
    if (availableTime < 20) {
      console.log("pick up a snack or grab something you have ready at home.");
    }
    if (availableTime > 20 && availableTime < 30) {
      console.log("you deserve a break and should take time to cook a tastymeal");
    }
    if (availableTime > 30) {
      console.log("this is an intense program after all and you should probably reconsider.");
    }
  }

}
whatToDoForLunch(false, 40);
whatToDoForLunch(true, 10);
whatToDoForLunch(true, 25);
whatToDoForLunch(true, 39);
```