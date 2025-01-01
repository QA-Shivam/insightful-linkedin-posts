# linkedin-posts
Some insightful linkedIn posts

#1
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
