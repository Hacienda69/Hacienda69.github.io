# Static Code Analysis - Dani Mañas

## Systems for static code analysis to catch more errors in code

Static Code Analysis (SCA) is a method of analyzing source code without executing it. It involves examining the code's structure, syntax, and other characteristics to identify potential defects, security vulnerabilities, coding mistakes, and adherence to coding standards. The analysis is performed by specialized tools known as Static Code Analyzers or Static Analysis Tools.

### key points

* **Automated Analysis:** Static Code Analysis is an automated process where specialized tools scan the source code files to identify issues. It helps to catch potential problems early in the development cycle. (SUPER IMPORTANT, IF A PROJECT STARTS WITH ITS CODE HAVING ISSUES THOSE PROBLEMS WILL EXPONENTIALLY INCREASE)

* **No Execution Required:** Unlike dynamic analysis methods that involve executing the code, Static Code Analysis works directly on the source code files. It does not require compiling or running the code, making it efficient and less time-consuming. (FAST AND EASY TO PERFORM)

* **Wide Range of Checks:** Static Code Analyzers can perform a variety of checks, including syntax errors, coding standards violations, potential bugs, security vulnerabilities, performance bottlenecks, and other software quality-related issues. (WIDE RANGE OF FUNCTIONALITY)

* **Coding Standards Compliance:** SCA tools can enforce coding standards and guidelines, ensuring that the codebase adheres to established best practices. This helps in maintaining code consistency, readability, and maintainability. (THIS HELPS IMPROVING THE TEAMWORK AND THE QUALITY OF THE CODE)

* **Bug Detection:** Static Code Analysis can identify common coding mistakes that may lead to bugs or unexpected behavior. It can detect issues such as null pointer dereferences (HUGE MISTAKE AMONG CLASSMATES), memory leaks, buffer overflows, and other potential sources of runtime errors. (TO HELP FOR EXAMPLE CREAR ALL THE OBJECTS THEY CREATE AND CANNOT DESTROY)


**NOTE:** By using Static Code Analysis, developers and organizations can proactively identify and address potential issues in their codebase, leading to improved software quality, enhanced security, and more maintainable code but Static Code Analysis tools may occasionally generate false positives (warnings for code that is actually correct) or false negatives (missing actual issues). It is important for developers to review the analysis results critically and use their judgment to address the identified issues.


## Address sanitizers in C/C++

Address sanitizers are dynamic analysis tools that help catch memory-related bugs and vulnerabilities during program execution. They are part of the GCC and Clang compilers and provide additional runtime checks. Here are two commonly used address sanitizers:

* **AddressSanitizer (ASan):** a memory error detector designed to catch issues like buffer overflows, use-after-free, and other memory-related bugs. It adds instrumentation to the compiled code to perform runtime checks and report errors.

* **UndefinedBehaviorSanitizer (UBSan):** focuses on detecting undefined behavior in C/C++ code. It helps identify problematic code constructs that may lead to unexpected program behavior. UBSan reports violations during runtime.

Both ASan and UBSan provide valuable feedback during program execution, making it easier to identify memory-related issues and undefined behavior. They are commonly used alongside static code analysis tools to provide a comprehensive approach to code quality and security.

## Example for online: coverity, other tools?

### Online Static Code Analysis Tools:

* **Coverity:** (now part of Synopsys) is a widely used commercial static code analysis tool. It performs in-depth analysis of C, C++, Java, and other languages, helping to identify defects, security vulnerabilities, and quality issues.

* **CodeClimate:** online platform that offers static code analysis for multiple languages, including JavaScript, Python, Ruby, and more. It provides insights into code quality, duplication, security vulnerabilities, and test coverage.

* **SonarQube:** an open-source platform that offers static code analysis for various languages. It provides a comprehensive range of checks for bugs, vulnerabilities, code smells, and technical debt. SonarCloud is the cloud-based version of SonarQube.

* **LGTM:** (short for "Looks Good To Me") is an online platform for static code analysis that supports multiple languages. It focuses on finding security vulnerabilities, code quality issues, and coding standards violations.

## Example for oﬄine: cppcheck, other tools?

### Offline Static Code Analysis Tools:

* **Cppcheck:** open-source C/C++ static code analysis tool. It performs a wide range of checks, including detection of null pointer dereferences, memory leaks, and incorrect use of standard library functions.

* **Pylint:** static code analysis tool for Python. It checks for coding standards violations, potential bugs, unused variables, and other common issues. It integrates well with popular Python development environments.

* **FindBugs:** open-source static code analysis tool for Java. It detects common programming errors, potential bugs, and bad coding practices. FindBugs has been integrated into many Java development environments.

* **ESLint:** widely used static code analysis tool for JavaScript. It helps identify coding errors, potential bugs, and adherence to coding standards. It can be customized with various rules and integrated into popular JavaScript development environments.
