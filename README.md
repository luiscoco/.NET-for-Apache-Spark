# .NET for Apache Spark

## What is Apache Spark?

https://dotnet.microsoft.com/en-us/apps/data/spark

https://github.com/dotnet/spark

Apache Spark™ is a general-purpose **distributed processing** engine for analytics over large data sets—typically, terabytes or petabytes of data. 

Apache Spark can be used for processing batches of data, real-time streams, machine learning, and ad-hoc query.

Processing tasks are distributed over a cluster of nodes, and data is cached in-memory, to reduce computation time.

## What is .NET For Apache Spark?

![image](https://github.com/luiscoco/.NET_Spark/assets/32194879/54287c5b-d414-44d3-b475-4027a87f4219)

The .NET bindings for Spark are written on the Spark interop layer, designed to provide high performance bindings to multiple languages.

.NET for Apache Spark is compliant with .NET Standard—a formal specification of .NET APIs that are common across .NET implementations. 

This means you can use .NET for Apache Spark anywhere you write .NET code.


# Tutorial: Get started with .NET for Apache Spark 

https://learn.microsoft.com/es-es/previous-versions/dotnet/spark/tutorials/get-started?tabs=windows

## Install .NET

To start building .NET apps, you need to download and install the .NET SDK (Software Development Kit).

Download and install the .NET Core SDK. Installing the SDK adds the dotnet toolchain to your PATH.

https://dotnet.microsoft.com/es-es/download/dotnet/3.1

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/512328f1-e253-4055-90b6-0f6bfbd3dc16)

Run the command to check the .Net Core SDK installation:

```
dotnet --version
```

**IMPORTANT NOTE**
.NET for Apache Spark targets an out-of-support version of .NET (.NET Core 3.1).

![image](https://github.com/luiscoco/.NET_Spark/assets/32194879/85b903e8-ece3-46d9-bd7f-1a17ef156fe2)

## Install Java 8 (JDK)

Install Java 8.1 for Windows and macOS, or OpenJDK 8 for Ubuntu.

Select the appropriate version for your operating system. For example, select **jdk-8u201-windows-x64.exe** for a Windows x64 machine

https://www.oracle.com/java/technologies/downloads/#java8-windows

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/47152403-443c-41cb-9d5a-95c3a6e3eea3)

## Install compression software

Apache Spark is downloaded as a compressed .tgz file. 

Use an extraction program, like 7-Zip or WinZip, to extract the file.

## Install Apache Spark

Download and install Apache Spark. You'll need to select from version 2.3.* or 2.4.0, 2.4.1, 2.4.3, 2.4.4, 2.4.5, 2.4.6, 2.4.7, 3.0.0, 3.0.1, 3.0.2, 3.1.1, 3.1.2, 3.2.0, or 3.2.1 

(.NET for Apache Spark is not compatible with other versions of Apache Spark).
