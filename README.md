console.log(data);

console.assert(data.count == 15, "assert message");

console.assert(data.count == 14, "assert message coming"); //works only if con is false,//Assertion failed: assert message coming

console.log(data.count == 15, "log message"); // works for both con: true/false, // true "log message"

console.log(data.count == 14, "log message coming"); // false "log message coming", //console.clear(); //will clear all above console errors

console.count():

Logs the number of times that this particular call to count() has been called. 

This function takes an optional argument label.

```
for (var i = 0; i < 10; i++) {
    console.count(); //1,2,3,4....9,10
}
```

console.count(); // 1

console.count(); // 1

console.count("myLabel"); // myLabel: 

console.count("myLabel"); // myLabel: 2

console.dir(document); // object reprn of document

console.dirxml(document); // xml reprn of document

console.error("My custom error"); // in red color, same as default console errors

console.error(data.count);

console.time("timer");
```
var portfolios = data.results;
for (var i = 0; i < portfolios.length; i++) {
    console.group("Portfolio"); // by default: uncollapsed
    //console.groupCollapsed("Portfolio");
    console.group("Portfolio ID: ");
        console.log(portfolios[i].id);
    console.groupEnd();
    console.log(portfolios[i].updated_at);
    console.groupEnd();
}
```

console.timeEnd("timer");
//console.info -- works as per its behaviour in firefox not in chrome, its similar to console.log

console.log("%cStop!", "font-size: 36px;font-weight: bold;color: red;")
console.log("%cThis is a browser feature intended for developers. If someone told you to copy-paste something here to enable a USGBC feature or \"hack\" someone's account, it is a scam and will give them access to your USGBC account.", "font-size: 22px;")
console.log("%cSee https://www.usgbc.org/security for more information.", "font-size: 22px;")

console.table(portfolios);

console.clear();

console.trace("Trace");

console.warn("This is warning message!");