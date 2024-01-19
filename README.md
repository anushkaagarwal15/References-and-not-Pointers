# References-and-not-Pointers

Reasons Why Pointers are not Used in Java?
There are a few reasons why pointers are not used in Java, and let’s learn about them one by one.

1. Security Loss
As we know, Pointers variables refer to the memory address location of the data directly, and that’s why security will be significantly less in the case of pointers. Any modification can be made using the Memory address locations if someone gets access to it, resulting in a loss of security. But Java is a very secure programming language, so it has to provide very good security for its application data, and that is why Pointers are not supported in Java.
2. Complex Nature of Pointers
Under C and C++ programming languages, Pointers are somewhat confusion-oriented features. They increase confusion among the programmers. Not only the single-level pointers but when we go for multi-level pointers, which means one pointer is pointing to another pointer, another pointer is referring to some another pointer and some another pointer is referring to some another pointer, thus creating a chain of pointers.

Multi-level pointers automatically create confusion and complexity for the developers. They complicate the language and make it more difficult to learn and to use. And due to the complex nature of pointers and hard-to-understand, Java has eliminated the feature of pointers because Java is a very simple language. It focuses on code simplicity, and the usage of pointers can make it challenging.

3. Pointer Arithmetic is Unsafe 
Memory access via pointer arithmetic is known to be insecure. By manipulating pointers using pointer arithmetic, one could potentially access sensitive information or jeopardize the security of a system. It is fundamentally unsafe and can lead to memory corruption or vulnerabilities. Java has a robust security model, which is why it disallows pointer arithmetic for this reason.

4. Platform-Dependent 
Pointers are primarily suitable in platform-dependent programming languages such as C, C++ etc. But Java is a platform-independent programming language, and one of its major features. Allowing pointers would make it much less platform-independent, which would be a severe drawback, which is why pointers are not used in Java.

5. Manipulation of Pointers can be Dangerous 
Manipulation of pointers can be dangerous if you’re not careful. If you try to access a pointer that’s not been initialized, you can end up with all sorts of undefined behavior. Dereferencing a null pointer can cause your program to crash. Trying to write to a read-only memory location can also cause undefined behavior.

Bottom line: Manipulating pointers can be dangerous. If you’re not careful, you can easily create a situation where your program crashes or behaves unexpectedly.
6. Manual Memory Management 
Pointes can be used to allocate and deallocate blocks of memory which is a great feature. But sometimes, it can be a pain for programmers who have to manage memory manually. If memory isn’t managed carefully, it can lead to headaches in the form of leaks and other memory-related issues.

To solve this problem, Java provides built-in Garbage Collection(GC), one of the language’s most lauded features. This allows developers to focus on creating new objects instead of worrying about memory allocation and deallocation. The garbage collector automatically reclaims memory for reuse, which Java developers appreciate because it enables faster development with less boilerplate code. Additionally, it eliminates memory leaks and other memory-related problems.

7. Pointers can be used for Hacking and Viruses 
The use of pointers is a common technique for hacking and viruses. By using a pointer, hackers and viruses can change the value of a data item without changing the data item itself. It can be used to hack into systems and create viruses, as the pointer can access memory that is not normally accessible. It can also be used to point to sensitive data, such as passwords or credit card numbers, which can be stolen by a hacker.

So these were some of the reasons why pointers are not used in Java. Overall, they are not necessary for general-purpose OOP programming and adding them in Java Programming Language can actually compromise security and lead to more complexity
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
What is used instead of Pointers in Java?


In Java, References are used instead of pointers. A reference variable is a value that points to an object. A reference can be thought of as a pointer to memory, but it is not possible to manipulate a reference directly. Java uses the concept of pointers implicitly for the manipulation of references, and they are not available for outside use.

The reference variable stores the reference value of an object. The reference value is nothing but the hexadecimal form of hash code. Hash code is a unique identity for the object prepared by the heap manager in the form of an integer value.
