### Questions:

**Why is access control important?**

Access control regulates which users, applications, and devices can view, edit, add, and delete resources in an organization’s environment. Controlling access is one of the key practices to protect sensitive data from theft, misuse, abuse, and any other threats.

*Source: https://www.ekransystem.com/en/blog/mac-vs-dac*

**Describe an application that would need access control.**

Social media apps are a good example of access control.  Generally, a user is able to view, post, edit and delete their own information, but will only be able to view a small portion of the information that belongs to others (information that has been specifically deemed 'viewable').  However, website administrators are able to see more/all of the the information and often have the authority to remove content deemed unacceptable.

**What is a role used for?**

A role describes a category a user falls into - this term is used often in Role Based Access Control, where roles determine what is and is not deemed necessary access for individuals who fill that role.

**Why is role based access control more scalable than discretionary or mandatory access control?**

RBAC is highly scalable because it does not require (and actually actively avoids) exceptions and customizations.  If one is assigned a role but it later becomes clear that they require access beyond what is associated with that role, then rather than tweak their individual permissions they should be assigned a more appropriate role with the correct permissions.  If that role doesn't yet exist, then it must be created.  Should that person later leave the work environment, nothing has to change because no permissions were tied specifically to them as a person

MAC is arguably more secure, but also more rigid.  It works by assigning security levels to both people and content - a persons security level must meet or exceed that of the content that they wish to access.

DAC is more flexible in that it lets users control access permissions to their data

In both these models, each individual piece of data has to have permissions or security requirements set around it, while RBAC works by declaring which roles have access to specific types of actions.

*Source: https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html*
*Source: https://www.ekransystem.com/en/blog/mac-vs-dac*

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|Authorization|A security mechanism to determine access levels or user/client privileges related to system resources|https://economictimes.indiatimes.com/definition/authorization#:~:text=Definition%3A%20Authorization%20is%20a%20security,programs%2C%20data%20and%20application%20features.&text=Key%20factors%20contain%20user%20type,and%20related%20actions%20and%20roles.|
|Role Based Access Control|The idea of assigning system access to users based on their role within an organization|https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html|
|Capabilities|A communicable, unforgeable token of authority. A value that references an object along with an associated set of access rights. A user program on a capability-based operating system must use a capability to access an object|https://en.wikipedia.org/wiki/Capability-based_security#:~:text=A%20capability%20(known%20in%20some,capability%20to%20access%20an%20object.|

---

[Home](https://jchinzi.github.io/reading-notes/)