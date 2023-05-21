## Authentication


Begin with a statement addressing why this topic matters as it relates to what you are studying in this module.

### Readings
[Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)

#### Explain to a non-technical friend how you would safely hash and store a password.

"To safely hash and store a password, I would use a cryptographic hashing algorithm like Bcrypt. First, I would take the password provided by the user and pass it through the Bcrypt algorithm. This process converts the password into a fixed-length string of characters that cannot be easily reversed. The resulting hash is what we store in the database. Importantly, we never store the actual password itself."
"When the user tries to log in, we repeat the same process with the entered password and compare the resulting hash with the stored hash. If they match, it means the entered password is correct. This way, even if someone gains unauthorized access to the database, they won't be able to retrieve the original passwords." - ChatGPT

**Bonus Question: Explain a hashing algorithm in simple terms:**
"A hashing algorithm is like a special math formula or process that takes some input, like a password, and turns it into a unique code, called a hash. It's a way of converting information into a different form that is difficult to reverse back to the original.

Think of it like a secret code machine. You put in a word or a phrase, and it gives you a jumbled-up code as the output. But here's the interesting part: the same input will always give you the same output. So, if you enter the same password into the hashing algorithm, it will always produce the same hash.

The important thing about a hashing algorithm is that it's designed to be really hard to figure out the original input just by looking at the hash. It's like trying to unscramble an egg! Even a tiny change in the input will result in a completely different hash.

Hashing algorithms are commonly used to store passwords securely. Instead of storing the actual passwords, websites and services store the hashed versions. This way, even if someone gets their hands on the hashed passwords, it's extremely difficult for them to figure out the original passwords.

So, in simple terms, a hashing algorithm is a special way of turning information into a unique code that helps keep things safe and secure by making it hard for others to figure out the original information." - ChatGPT


**What is Bcrypt?**
"Bcrypt is a specific hashing algorithm that is designed to securely hash passwords and protect them from attacks. It is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm. Bcrypt introduces a work factor or security factor that determines the computational cost of the hash function. This means that Bcrypt can be intentionally slowed down to make brute-force attacks more difficult and time-consuming for attackers." - ChatGPT


**Why might you use something like Bcrypt?**

"Bcrypt or similar algorithms are used because they provide a higher level of security compared to traditional hash functions like MD5 or SHA1. Bcrypt's main advantage is its adaptability. By adjusting the work factor, the hashing process can be made slower over time as computing power increases. This ensures that even with advancements in technology, it remains computationally expensive for attackers to crack hashed passwords. By using Bcrypt, we can better protect users' passwords and sensitive data from unauthorized access and potential data breaches." - - Chat GPT

### [Basic Auth](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)

#### What is Basic Authentication?
"Basic Authentication is a method used in web browsing to provide a username and password for accessing a website or online resource. It allows the user to enter their credentials, which are then encoded and sent along with their request." - ChatGPT

#### What properties are necessary in the header of a Basic Auth request?
"In a Basic Auth request, the header should include the following properties:

Authorization: Basic <credentials>: This is the main header field that contains the authentication information. The word "Basic" indicates the type of authentication being used.
<credentials>: This is the Base64 encoding of the user's ID (username) and password joined by a colon (:). The ID and password are combined and encoded to form a single string." - ChatGPT

#### How are username:password in Basic Auth encoded?
"The username and password in Basic Authentication are encoded using Base64 encoding. Base64 is a method of representing binary data (such as the username and password) in ASCII characters. The resulting encoded string is then sent as part of the request header." - ChatGPT

#### [OWASP auth cheatsheet](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)

1. **Define the authentication process to a non-technical recruiter.**
"The authentication process, in simple terms, refers to the verification of an individual, entity, or website to confirm their identity. In the context of web applications, authentication typically involves entering a username or ID and providing private information that only the authorized user should know." - ChatGPT

2. **How should your error messaging respond (both HTTP and HTML)?**
"The error messaging in both HTTP and HTML should respond in a generic manner, regardless of the specific authentication failure. This means that the application should provide a consistent error message, such as "Invalid Username or Password," without disclosing whether the error occurred due to an incorrect username, password, or any other specific account-related issue. By using generic error messages, the application prevents attackers from gaining insight into valid user accounts through enumeration techniques." -ChatGPT
3. **Why?**
"The primary reason for using generic error messages is to prevent attackers from exploiting the authentication system by enumerating valid user accounts. By providing consistent error messages regardless of the specific authentication failure, the application eliminates the possibility of attackers determining valid usernames or passwords based on the error responses they receive. This helps maintain the security of user accounts and enhances the overall security posture of the application." - ChatGPT

##### Consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.

### Bookmark and Review

[bcrypt docs](https://www.npmjs.com/package/bcrypt)

- This is an npm library to help you hash passwords

### Additional Questions
Looking ahead at this module’s [course schedule](https://codefellows.github.io/code-401-javascript-guide/curriculum/#module-2), What do you look forward to learning?

* I am excited to continue working on the Code Challenges.
* Utilizing Authentication and Authorization securely is an important function of programming. 

What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-06/)?


* I want to be comfortable and confident in utilizing authorization in my projects. 

## Things I want to know more about

* Crypto security seems to be a full-time job in and of itself. Would it behoove most programmers to also learn this skill set?