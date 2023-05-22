## Bearer Authorization

Using a “Bearer Token” to re-authenticate with a server following a successful login, or obtaining/generating a permanent key


### Reading
___
#### [Intro to JWT](https://canvas.instructure.com/courses/6745251/discussion_topics/18080720)

1. ##### What is a JSON Web Token (JWT)?

"A JSON Web Token (JWT) is a compact and self-contained way of securely transmitting information between parties as a JSON object. It is digitally signed, which means it can be verified and trusted. JWTs can be used to securely transmit information and authenticate users." -ChatGPT

2. ##### When should we use JSON Web Tokens?

"JSON Web Tokens are useful in various scenarios. One common scenario is for authorization purposes. Once a user is logged in, subsequent requests can include a JWT, allowing access to routes, services, and resources that the user is permitted to access. JWTs are also useful for securely exchanging information between parties, as the sender's identity can be verified and the content can be checked for tampering." - ChatGPT

3. ##### Claims are expected in which structural component of a JWT?

"Claims are expected in the payload component of a JWT. The payload contains statements about an entity, such as the user, and additional data. Claims can be registered, public, or private. Registered claims are predefined and provide useful interoperable claims, while public and private claims can be defined by the parties using the JWT." - ChatGPT

 #### [Are JWTs Secure](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)?

" JWTs can provide security when used properly. They can verify the integrity of the claims and ensure that the sender is authentic. However, it's important to be cautious with sensitive information and not include it in the payload or header of a JWT unless it is encrypted. Care should also be taken to handle and store tokens securely to prevent unauthorized access." - ChatGPT

1. #### If I get a JWT and I can decode the payload, how can we call that secure?

"If you can decode the payload of a JWT, it means that you have access to the information contained within it. However, the security of a JWT lies in its integrity and authenticity, rather than its confidentiality. The fact that you can decode the payload does not compromise the security of the token itself. The signature component of the JWT ensures that the token has not been tampered with and that it was issued by a trusted entity. By verifying the signature, you can trust the claims within the payload and be confident that the token has not been modified." - ChatGPT

2. #### If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.

"When sending a JWT, both the sender and the receiver must know the shared secret or key. The shared secret is used to calculate the signature of the JWT. The sender signs the JWT using the secret, and the receiver can verify the signature using the same secret. By having the shared secret, the receiver can validate the authenticity and integrity of the JWT. It's important to keep this secret confidential and share it securely between the sender and receiver to prevent unauthorized access to the tokens." -ChatGPT

3. #### Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.

"
If you can decode the payload of a JWT, it means that you have access to the information contained within it. However, the security of a JWT lies in its integrity and authenticity, rather than its confidentiality. The fact that you can decode the payload does not compromise the security of the token itself. The signature component of the JWT ensures that the token has not been tampered with and that it was issued by a trusted entity. By verifying the signature, you can trust the claims within the payload and be confident that the token has not been modified.

When sending a JWT, both the sender and the receiver must know the shared secret or key. The shared secret is used to calculate the signature of the JWT. The sender signs the JWT using the secret, and the receiver can verify the signature using the same secret. By having the shared secret, the receiver can validate the authenticity and integrity of the JWT. It's important to keep this secret confidential and share it securely between the sender and receiver to prevent unauthorized access to the tokens.

When explaining how concatenated content and a secret can be sent and received securely to a non-technical recruiter, it's important to focus on the high-level concept rather than technical details. You can use an analogy to explain the process. For example:

Imagine you have a special lockbox that can only be opened with a unique key. To securely send a message, you put the message inside the lockbox and lock it with the key. Then, you can send the locked box to the recipient. When the recipient receives the locked box, they can use the same key to open it and access the message. The key acts as the shared secret between the sender and the receiver.

In the case of JWTs, the content (payload) is like the message, and the secret is like the key. The sender creates a JWT by combining the content and the secret, creating a locked token. This token can then be sent to the receiver. The receiver, who knows the secret, can unlock the token and access the content securely.

It's important to emphasize that the secret should be shared securely and not disclosed to unauthorized parties. By using this approach, the sender can securely transmit information to the receiver without compromising its integrity or authenticity." -ChatGPT


### Videos
___

#### [JWTs Explained](https://www.youtube.com/watch?v=926mknSW9Lo)

*This useful video demonstrates the implementation of JWT*

##### Why use JWT?
 "By using JWTs, you can enjoy a more convenient and secure online experience. They provide a streamlined way to communicate, ensure the integrity of your data, and simplify authentication processes. So, the next time you encounter a website or application that offers JWT-based authentication, it's worth considering using them for a safer and smoother experience.

##### JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

1. **Compactness:** JWTs are designed to be compact, which means they are small in size compared to other formats like XML-based tokens. This compactness is beneficial because it makes JWTs easier to transmit and share over the internet. It's like sending a small and lightweight package instead of a bulky one. This can result in faster communication and less bandwidth usage, making it more efficient for applications and services.

2. **Self-contained:** JWTs are self-contained, meaning they contain all the necessary information within the token itself. This is similar to having a complete package that includes everything you need, without relying on external resources. In the case of JWTs, the token holds the relevant data or claims about a user or entity. It eliminates the need for additional database or server lookups to validate or fetch user information. This self-contained nature makes JWTs easy to work with and reduces the reliance on external systems, making them more portable and flexible.



##### What are the three components (the structure) of a JWT signature?

1. **Header:** The header of a JWT contains information about the type of token (JWT) and the signing algorithm used. It provides metadata about the token itself.

2. **Payload:** The payload carries the claims or statements about an entity (such as a user) and additional data. Claims can be predefined (registered claims), user-defined (public claims), or private claims agreed upon between parties. This is where the actual information resides.

3. **Signature:** The signature component of a JWT is created by taking the encoded header, the encoded payload, a secret key, and the specified algorithm from the header. It ensures the integrity and authenticity of the token. The signature is used to verify that the token hasn't been tampered with and that it was generated by a trusted party. The signature is appended to the encoded header and payload, forming the complete JWT.

By understanding these components, one can see that the header provides important metadata, the payload contains the relevant information, and the signature guarantees the token's integrity. Together, these components make up a secure and self-contained JWT." -ChatGPT


### Bookmark and Review

[npm jsonwebtoken docs](https://www.npmjs.com/package/jsonwebtoken)
To install : `npm i jsonwebtoken`

### Reflection
What are your learning goals after reading and reviewing the class [README](https://codefellows.github.io/code-401-javascript-guide/curriculum/class-07/)?

I am hoping to become more familiar with implementing Authorizations in my projects. 


## Things I want to know more about

What are some of the newer sources of authorization?

