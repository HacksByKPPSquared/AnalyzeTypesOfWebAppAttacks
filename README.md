# 💻 Analyzing Types of Web Application Attacks 🌐

Welcome to **My Lab**, where we dive into the dark, murky world of web application attacks! From SQL injection to cross-site scripting (XSS), this lab teaches you how the bad guys get in—and more importantly, how to stop them. ⚔️ Let's break it down!

## 🔍 What Happened:

1. **SQL Injection - Mastering WebGoat 🐐**:
   - We started by firing up the **WebGoat** web server, a vulnerable training app designed to help developers understand how web apps can be attacked. It's like a playground for hackers… but don't worry, it's all in good fun! 😏
   - Navigated through **SQL injection** exploits, inputting queries that weren't exactly what the database expected. Spoiler: We accessed user data we weren't supposed to. Oops! 🙃
   - Attempted to log in as an admin without a password using a clever injection. It didn’t give us access right away, but thanks to some **Tamper Data** magic, we got in eventually. 🛠️

2. **DVWA - Another SQL Injection Playground 🛡️**:
   - Moved to the **Damn Vulnerable Web Application (DVWA)** and dove into SQL injection once more. With a few tricks, we could list all user accounts in the database and even query for specific information.
   - We queried for everything from user IDs to the database version because… why not? 😏

3. **Cross-Site Scripting (XSS) Exploits 💣**:
   - Once we mastered SQL injection, we ventured into the land of **XSS attacks** using DVWA. We injected some scripts into comment sections that popped up alerts for unsuspecting users.
   - But it didn’t stop there! We inserted an iframe, and guess what? We could display another webpage right inside the vulnerable app. Talk about getting creative! 💻🎨
   - Lastly, we explored cookie theft with XSS. Imagine getting someone’s cookie details from their browser. In the wrong hands, that could spell trouble! 🍪🚨

## 🛠️ Tools Used:

- **WebGoat**: A playground for learning about web vulnerabilities. It's the goat you don’t mind having around. 🐐
- **DVWA**: Another vulnerable web app that lets you safely test out different exploits. 😈
- **Tamper Data**: Helped us manipulate HTTP requests like true web ninjas. 🥷
- **MySQL & Apache**: Powering our backend services to give us something to break into. 🔧

## 🌈 Why This Lab Matters:

Understanding web application vulnerabilities like SQL injection and XSS is key for anyone working in web development or cybersecurity. By learning how these attacks happen, you’re not only ready to defend against them—you’re one step closer to becoming a full-blown web security hero! 🦸🏾‍♂️🦸🏾‍♀️

---

💡 **Pro-Tip**: Always sanitize your inputs! SQL injection and XSS attacks thrive on user input that isn't properly validated. A little effort in coding now can save a lot of headaches later. 🤯

---

Ready to defend the web, one exploit at a time? Let’s code securely and keep the internet a safe place! 🌍🛡️
## 👉🏾[Lab Walkthrough](https://github.com/Kpierre03/AnalyzeTypesOfWebAppAttacks/blob/main/Analyze.md)
