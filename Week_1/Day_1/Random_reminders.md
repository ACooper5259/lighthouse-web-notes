## Random Reminders

#### GIT
Before before seeing any changes onto the git hub site, the following commands have to be run:
* git add . (or git add fileName.js); for staging documents
* git commit -r "description of changes"
* git push origin master

#### Lint 
* eslint fileName.js
* eslint . (to run onto all files within the current directory)
* syntax: eslint [options] file.js [file.js] [dir]

#### process.argv
* terminal: node processargv.js tom jack 34
* with a js file: sum.js
```
const args = process.argv;
let fewerArgs = args.slice(2);

function addition(fewerArgs) {
  let result = Number(fewerArgs[0]) + Number(fewerArgs[1]);
  return result
};

console.log (addition(fewerArgs))
```
* in terminal: node sum.js; note: sum.js and process.argv are in the same folder

### template litterals
* starts and ends with `
* add $(varName)