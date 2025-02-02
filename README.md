# linkedin-posts
Some insightful linkedIn posts

# 1
Mastering Selenium’s 𝐛𝐮𝐢𝐥𝐝() and 𝐩𝐞𝐫𝐟𝐨𝐫𝐦() Methods for Complex Interactions 

When automating web interactions using Selenium WebDriver, managing multiple actions in a sequence is a common requirement. Here, the 𝘣𝘶𝘪𝘭𝘥() and perform() methods in the 𝐀𝐜𝐭𝐢𝐨𝐧𝐬 API come into play. Understanding their usage and differences can greatly enhance our test automation skills. Let’s dive into how these methods work, their differences and when to use them.

1. 𝐛𝐮𝐢𝐥𝐝() Method:
🔸 The build() method is used to 𝒄𝒐𝒎𝒑𝒊𝒍𝒆 𝒂 𝒔𝒆𝒓𝒊𝒆𝒔 𝒐𝒇 𝒂𝒄𝒕𝒊𝒐𝒏𝒔 (e.g., mouse movements, clicks, key presses) into a single action chain. 
🔸 It doesn’t execute the actions immediately but prepares them for execution.
𝐔𝐬𝐞 𝐂𝐚𝐬𝐞:
▪️ We can 𝒃𝒖𝒊𝒍𝒅 𝒂𝒄𝒕𝒊𝒐𝒏𝒔 𝒔𝒆𝒑𝒂𝒓𝒂𝒕𝒆𝒍𝒚 𝒂𝒏𝒅 𝒆𝒙𝒆𝒄𝒖𝒕𝒆 𝒕𝒉𝒆𝒎 𝒍𝒂𝒕𝒆𝒓.

2. 𝐩𝐞𝐫𝐟𝐨𝐫𝐦() Method:
🔸Once we have built our action sequence using build(), the perform() method is used to execute the actions. 
🔸This method triggers the sequence of events defined by the Actions chain.
𝐔𝐬𝐞 𝐂𝐚𝐬𝐞:
▪️ 𝐈𝐦𝐦𝐞𝐝𝐢𝐚𝐭𝐞 𝐄𝐱𝐞𝐜𝐮𝐭𝐢𝐨𝐧: Call perform() when we want to execute the actions immediately after building them. 
▪️We 𝒎𝒂𝒚 𝒆𝒗𝒆𝒏 𝒔𝒌𝒊𝒑 𝒃𝒖𝒊𝒍𝒅() 𝒂𝒏𝒅 𝒅𝒊𝒓𝒆𝒄𝒕𝒍𝒚 𝒖𝒔𝒆 𝒑𝒆𝒓𝒇𝒐𝒓𝒎(), 𝒂𝒔 𝒊𝒕 𝒄𝒐𝒎𝒑𝒊𝒍𝒆𝒔 𝒂𝒏𝒅 𝒆𝒙𝒆𝒄𝒖𝒕𝒆𝒔 𝒕𝒉𝒆 𝒂𝒄𝒕𝒊𝒐𝒏𝒔 𝒊𝒏 𝒐𝒏𝒆 𝒈𝒐.

𝐊𝐞𝐲 𝐃𝐢𝐟𝐟𝐞𝐫𝐞𝐧𝐜𝐞:
☑️ 𝒃𝒖𝒊𝒍𝒅(): 
1. Compiles the actions into a chain without executing them.
2. Use build() when we need to create 𝒄𝒐𝒎𝒑𝒍𝒆𝒙 𝒓𝒆𝒖𝒔𝒂𝒃𝒍𝒆 𝒂𝒄𝒕𝒊𝒐𝒏 𝒔𝒆𝒒𝒖𝒆𝒏𝒄𝒆𝒔.
☑️ 𝒑𝒆𝒓𝒇𝒐𝒓𝒎(): 
1. Executes the compiled action chain.
2. Use perform() when we want to 𝒆𝒙𝒆𝒄𝒖𝒕𝒆 𝒕𝒉𝒆 𝒂𝒄𝒕𝒊𝒐𝒏𝒔 𝒊𝒎𝒎𝒆𝒅𝒊𝒂𝒕𝒆𝒍𝒚 𝒘𝒊𝒕𝒉𝒐𝒖𝒕 𝒏𝒆𝒆𝒅𝒊𝒏𝒈 𝒕𝒐 𝒔𝒕𝒐𝒓𝒆 𝒕𝒉𝒆𝒎 𝒇𝒐𝒓 𝒍𝒂𝒕𝒆𝒓.

Question: What will happen if you call:
A) actions.scrollToElement(ele).click().build().perform(); 
B) actions.scrollToElement(ele).click().perform();

A throws an error
B throws an error
Both A and B work the same
Both A and B throw errors
Answer: Both A and B work the same

# 2
Interview Questions from my last 3 Interviews Experience November and December 2024

1) Java program to remove duplicates characters from given String. 
2) Program Remove the second highest element from the HashMap. 
3) Java program to Generate prime numbers between 1 & given 4
number 
4) How to find the missing values from a sorted array. 
5) Java program to input name, middle name and surname of a 
person and print only the initials. 
5) Program to Print all Treemap elements? 
6) What is a singleton Design Pattern? How do you implement that in your framework? 
7) Write the Top 5 test cases for Booking Coupons. 
8) What is serialization and deserialization? 
9) What is the Difference between status codes 401 and 402? 1
10) Difference between selenium 3 and selenium 4? 
11) What is delegate in Java and where do you use Delegate in your Framework? 
12) How many maximum thread-pool can you open in the TestNG? 
13) What are the Major challenges that come into the picture when you do parallel testing using TestNG and Grid? 
14) How do you integrate your automation framework with the Jenkins pipeline? 
15) What will happen if we remove the main method from the java program? 
16) What is the component of your current Project? 
17) How do you pass parameters in TestNG? 
18) Write the logic of retrying the failed test case with a minimum 3 numbers of time in Automation Testing. Which Interface do you use for it? 
19) What is the OOPs concept in java? 
20) What is encapsulation? 
21) What is Polymorphism? 
22) Difference Between Classes and Objects? 
23) What is collection in Java? 
24) What is out in System.out.println? 
25) In How many ways can we create an object? 
26) Why is Java not 100% Object-oriented?
27) Can we make a constructor as Static? 
28) How to convert a JSON object to a java object using Jackson? 
29) What is the difference between Abstraction Class and Interfaces? 
30) Difference between String, StringBuilder, and Stringbuffer? 
31) What are other immutable classes in Java apart from String? 
32) Difference between TreeMap and HashMap? 
33) How do you set priorities for test automation, which test needs to be automated first? 
34) How do you set test case priorities for your team? 
35) What are the functional things you need to test on e-commerce sites? 
