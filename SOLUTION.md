# Lab 04: Troubleshooting with build scans solution

## Steps
-----
1. **How much time is being spent on garbage collection?**

   Open the build scan link in your console and click "Performance"
   Under the "Build" heading, the answer is next to "Total Garbage Collection Time".

2. **What is the peak memory usage?**

    On the "Performance" tab, under the "Build" heading just below "Total Garbage Collection Time" peak usage of the JVM's different memory spaces are shown.

3. **Fix the issue degrading build performance:**

    The issue degrading build performance is an extremely low memory limit set within the `gradle.properties` file.
      Setting a higher limit, or removing the line entirely will allow gradle to use a sufficient amount of memory
