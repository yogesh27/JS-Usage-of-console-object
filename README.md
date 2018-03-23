1. console.log(data);
2. console.assert(data.count == 15, "assert message");
3. console.assert(data.count == 14, "assert message coming"); //works only if con is false,//Assertion failed: assert message coming
4. console.log(data.count == 15, "log message"); // works for both con: true/false, // true "log message"
5. console.log(data.count == 14, "log message coming"); // false "log message coming", //console.clear(); //will clear all above console errors
6. console.count(): Logs the number of times that this particular call to count() has been called. 
This function takes an optional argument label.

```
for (var i = 0; i < 10; i++) {
    console.count(); //1,2,3,4....9,10
}
```
7. 
console.count(); // 1
console.count(); // 1
9. 
console.count("myLabel"); // myLabel: 
console.count("myLabel"); // myLabel: 2

10.console.dir(document); // object reprn of document
console.dirxml(document); // xml reprn of document

11. console.error("My custom error"); // in red color, same as default console errors
console.error(data.count);

12. console.time("timer");
```
var portfolios = data.results; //to come from API
for (var i = 0; i < portfolios.length; i++) {
    console.group("Portfolio"); // by default: uncollapsed
    //console.groupCollapsed("Portfolio");
    console.group("Portfolio ID: ");
        console.log(portfolios[i].id);
    console.groupEnd();
    console.log(portfolios[i].updated_at);
    console.groupEnd();
}
console.timeEnd("timer");
```

12. console.info -- works as per its behaviour in firefox not in chrome, its similar to console.log

13. Facebook style console message
console.log("%cStop!", "font-size: 36px;font-weight: bold;color: red;")
console.log("%cThis is a browser feature intended for developers. If someone told you to copy-paste something here to enable a FB feature or \"hack\" someone's account, it is a scam and will give them access to your FB account.", "font-size: 22px;")
console.log("%cSee https://www.fb.com/security for more information.", "font-size: 22px;")

14. console.table(portfolios);

15. console.clear();

16. console.trace("Trace");

17. console.warn("This is warning message!");
