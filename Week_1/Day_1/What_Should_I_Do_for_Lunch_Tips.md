### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```const whatToDoForLunch = function(hungry, availableTime) {
  if (!hungry) {
    console.log('Go back to work for now');
  } else {
    if (availableTime < 20) {
      console.log("Grab something and eat it in the lab");
    } else if (availableTime >= 20 && availableTime <= 30) {
      console.log("Try a place nearby");
    } else if (availableTime > 30) {
      console.log('You really have that much time? in a bootcamp?');
    }
  }
};```