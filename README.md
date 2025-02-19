my-utility-library

Overview

my-utility-library is a lightweight Java utility designed to measure the execution time of code blocks for benchmarking and performance analysis. It provides a simple API for integrating performance measurement into Java applications.

Features

-  Simple API for benchmarking execution time
-  Lightweight and easy to use
-  Well-documented with Javadoc comments
-  Available as a Maven and Gradle dependency

Installation

Maven

```xml
<dependency>
    <groupId>com.mylib</groupId>
    <artifactId>my-utility-library</artifactId>
    <version>1.0</version>
</dependency>

dependencies {
    implementation 'com.my-utility-library:1.0'
}

import com.mylib.utils.TimeUtils;

public class Main {
    public static void main(String[] args) {
        TimeUtils.measureTime(() -> {
            long sum = 0;
            for (int i = 0; i < 1_000_000; i++) {
                sum += i;
            }
            System.out.println("Final sum: " + sum);
        });
    }
}

Repository and Download

GitHub Repository: my-utility-library
