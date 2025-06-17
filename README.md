Analysis of Certificate Pinning in Android Apps

Overview
This project, submitted for INSE 6110: Foundations of Cryptography (Winter 2023), analyzes the implementation of TLS certificate pinning in Android applications to prevent man-in-the-middle (MITM) attacks. The report investigates both static and dynamic analysis techniques across 100 Android apps.

Certificate Pinning
Certificate pinning is a security measure that binds an SSL/TLS certificate or public key to a specific server or domain, ensuring that client applications only communicate with servers that have the predefined certificate or key.

Types of Certificate Pinning

1. Hard Pinning: Hardcoding the server's certificate's public key or hash directly into the client's code.
2. Soft Pinning: Utilizing the client's trust store to verify the server's certificate chain.

Methodology
Static Analysis

* Download APK Files: APK files were downloaded from the web.
* Extract Build Files: Using apktool to extract and inspect network configurations.
* Code Inspection: Searching for certificates and related configurations within the application files.

Dynamic Analysis
We utilized Burp Suite Community Edition and Android Emulator API for dynamic analysis. For proxy configuration, we followed the setup method provided by Burp Suite here. We analyzed each app to determine if certificate pinning was enabled based on the app's behavior during login or account creation attempts.

Tools and Technologies

* Kali Linux: Used for security auditing and penetration testing.
* Android Emulator: Simulates Android devices for testing.
* Burp Suite: An integrated platform for security testing of web applications.
* Atom: A text editor used for inspecting code.
* Apktool: A tool for reverse engineering Android apps.

Application Analysis and Details
The study categorized various mobile applications and analyzed them using both static and dynamic methods. Detailed results and application specifics can be found here.

Findings and Conclusion
Certificate pinning can enhance security by preventing MITM attacks but introduces operational complexities. Proper implementation, regular updates, and fallback mechanisms are essential for effective certificate pinning.

Benefits

* Prevents MITM attacks
* Enhances security

Challenges

* Operational complexity
* Service disruptions
* Development and maintenance overhead
* Compatibility issues

Best Practices

* Implement backup pins
* Use soft pinning
* Monitor certificate expiry
* Graceful degradation
* Evaluate risks and benefits

Authors

* Deep Bhavesh Gajiwala
* Yash Khosla
* Devina Shah
* Meet Rakeshbhai Patel
* Pratiksha Ashok Kumar Pole
* Rohan Yogeshkumar Modi
* Simran Kaur
* Snehpreet Kaur

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
Special thanks to Dr. Amr Youssef for guidance and support throughout this project.


