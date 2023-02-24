# 10 Console Methods in JavaScript for Effective Debugging

Developers can use JavaScript console methods to access the debugging console in web browsers. Using methods to print various messages on the browser console, developers can improve the application debugging process.

The console.log() method, for example, allows us to print messages or data in the browser console. However, because developers are unaware of other console methods, it is frequently overused.

In this article, I’ll go over many of the JavaScript console methods and how to use them for debugging.

- **Log method**
The most commonly used JavaScript console method is console.log(). It is useful for printing strings, numbers, JavaScript objects, or variables to the console. Furthermore, instead of displaying messages in the browser console, it logs them to a debugging terminal.


![1_oycGSe35RqSXT23r8mQj6Q.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545326022/9KXHIbD9o.png align="left")


In the preceding example, I inserted the console.log() method within the function and passed a variable. When we run the code, we will get the output shown in the screenshot below.


![1_WsA4hpTgr6wmB9rO1f106A.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545353348/qD2MCsBd6.png align="left")

- **Info method**
Console.info() is similar to console.log(), but I recommend using console.info() to print any information needed for debugging rather than printing the values.


![1_sbgTUnL0GVI6XhjwN9FyAw.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545378936/SSwzDBBjO.png align="left")


The output from the above code is precisely the same as the output from the console.log() method.


![1_qKF5XGy_SFxiruoEtHhfuA.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545405349/_MGidEM4g.png align="left")

- **Debug method**
The console.log(), console.debug(), and console.info() methods in JavaScript are all the same. The only distinction is how the output is displayed in the browser console. Colour codes will be assigned to the console method output messages by the browser. The output of the console.debug() method is not visible in Chrome developer tools by default. To see the output from the debug method, you must enable the console filter option for all levels.


![1_ETbyOj1V5uSIUNLklhZcEQ.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545429974/ccMDdQTVz.png align="left")


To get the console.debug() method output, you need to enable the Verbose to debug level in dev tools in the dropdown shown in the following screenshot.


![1_8pm8TYrqgMEpTtQyM3ZwVg.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545448456/7qUAezulR.png align="left")


Now you can see the **console.debug()** output below.

- **Warn method**
We can use the console.warn() method to display a warning message in the console. A message must be passed as a parameter. This message can be an object, array, or variable of any type.


![1_prGbpZFdWamFPYAaV0WZsA.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545480169/e4oAADk_J.png align="left")


The console output of this code follows.


![1_6AKLfsF2RLFdjteNPCRbsg.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545498855/csdIumEx-.png align="left")

- **Assert method**
The console. assert() method is distinct from the previous methods. If the expression is evaluated as false, it will only print the message to the console. As a result, you must pass a Boolean expression as a method parameter.


![1_vG_JiV6dn91boGUhvLTw-g.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545524673/sKetAyoXj.png align="left")


The first and third statements in the preceding example are false. As a result, the output will be as follows.


![1_SX8OccJ6ubVmZaZFPTNkNQ.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545539187/FqV4IXzg3.png align="left")

- **Count method**
As a log counter, we can use the console.count() method. It keeps track of how many times the console.count() method was called in the script. For example, if you use it within a loop, you can determine how many times that loop is executed.

You can also enter any label into the console. With the label name as a parameter, the count() method will print it. For example, the code below will print each label until the loop is completed. To get the count, you can use any number of labels as a parameter. This will assist you in determining whether your loop is functioning properly and printing the expected output.

- **Trace method**
The trace method works exactly like the console.log() method. The console. trace() method, on the other hand, will return the stack trace. Essentially, it will display the call path used to get to the point where you placed the console.trace() method.


![1_K2jVv4TU1SV7nchX_ylMDQ.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545575701/eVBTFOPdI.png align="left")


We will get the following console output for the above code.

![1_G2suHg58w9OKeQJ_AuKxzA.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545588945/n60ViFDie.png align="left")

- **Time, TimeLog, and TimeEnd methods**
To calculate the execution time of the functions, use the console.time() method. It assists you in improving application performance by identifying underutilized functions. If you need to measure the performance of a for loop, for example, you can use the console.time() method, as shown below.


![1_ydh4PMFJEhBaKzSXFBta6w.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545644302/ecmqUEh6h.png align="left")

You can have an unlimited number of timers on the same page. To identify the timer, simply pass a unique label. Finally, you must invoke the console. To stop the timer, use the timeEnd() function. Make sure to use the same timer name in the console as well. timeEnd() method is also available.

- **Group, GroupEnd, and GroupCollapsed methods**
Using these methods, you can generate a series of messages in the console. The group method also accepts a label as an optional parameter, which must be placed immediately before a console message to begin grouping.

The output of the above code will look like the following.

![1_RbxVXha6D0mhNp_IpncnFw.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545680974/tuYrAa8Sj.png align="left")

Although passing a label to the console.group() method is not required, it does assist developers in determining which values are being grouped. However, because it always closes the most recently established logging group, console.groupEnd() does not require the group name.

The console.groupCollapsed() method in the console creates a new inline group, but it is not the same as the group created by the console.group() method. This console.groupCollapsed() method displays the beginning of the collapsed message group as well as all messages that were invoked after groupCollapsed (). A label can be passed as an optional parameter.


![1_LqyQGI8JyNh_qsAb9ZNMZw.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1665545709010/nSlUd8VR2.png align="left")

- **Clear method**
There are numerous methods and tools for debugging in JavaScript, but console methods are among the most basic and straightforward. Furthermore, because all of the methods support almost every web browser, developers can easily use them for debugging.

There are numerous methods and tools for debugging in JavaScript, but console methods are among the most basic and straightforward. Furthermore, because all of the methods support almost every web browser, developers can easily use them for debugging.

Have fun debugging! 😃







