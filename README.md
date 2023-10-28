# .NET for Apache Spark

## What is Apache Spark?

https://spark.apache.org/

Apache Spark™ is a general-purpose **distributed processing** engine for analytics over large data sets—typically, terabytes or petabytes of data. 

Apache Spark can be used for processing batches of data, real-time streams, machine learning, and ad-hoc query.

Processing tasks are distributed over a cluster of nodes, and data is cached in-memory, to reduce computation time.

## What is .NET For Apache Spark?

https://dotnet.microsoft.com/en-us/apps/data/spark

https://github.com/dotnet/spark

The .NET bindings for Spark are written on the Spark interop layer, designed to provide high performance bindings to multiple languages.

.NET for Apache Spark is compliant with .NET Standard—a formal specification of .NET APIs that are common across .NET implementations. 

This means you can use .NET for Apache Spark anywhere you write .NET code.

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/ff57a80e-1aa2-42ef-a994-890e77963f37)

# Tutorial: Get started with .NET for Apache Spark 

https://learn.microsoft.com/es-es/previous-versions/dotnet/spark/tutorials/get-started?tabs=windows

## Install .NET

To start building .NET apps, you need to download and install the .NET SDK (Software Development Kit).

Download and install the .NET Core SDK. Installing the SDK adds the dotnet toolchain to your PATH.

https://dotnet.microsoft.com/es-es/download/dotnet/3.1

Run the command to check the .Net Core SDK installation:

```
dotnet --version
```

**IMPORTANT NOTE**
.NET for Apache Spark targets an out-of-support version of .NET (.NET Core 3.1).

But I have .NET 7 installed in my laptop and .NET for Apache Spark is working fine.

## Install Java 8 (JDK)

Install Java 8.1 for Windows and macOS, or OpenJDK 8 for Ubuntu.

Select the appropriate version for your operating system. For example, select **jdk-8u201-windows-x64.exe** for a Windows x64 machine

https://www.oracle.com/java/technologies/downloads/#java8-windows

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/8859949c-8411-4b11-8bf4-4ffe17f16e53)

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/e1b1330d-90c8-4afe-85a7-e0b656960dc3)

Now set the environmental variable JAVA_HOME poiting the bin folder in the Java installation

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/1fcb4714-105e-4e09-9daa-4501e181eb6b)

And add the JAVA_HOME to the PATH variable

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/1b2e2313-23da-4f1d-90f3-93c13fe69958)

Restart you laptop and check the Java 8 (JDK) installation is fine

Open a command prompt window an run the command

```
java -version
```

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/a6e42723-6925-4273-a5a5-805bfe8a7015)

## Install compression software

Apache Spark is downloaded as a compressed .tgz file. 

Use an extraction program, like 7-Zip or WinZip, to extract the file.

## Install Apache Spark

Download and install Apache Spark. You'll need to select from version 2.3.* or 2.4.0, 2.4.1, 2.4.3, 2.4.4, 2.4.5, 2.4.6, 2.4.7, 3.0.0, 3.0.1, 3.0.2, 3.1.1, 3.1.2, 3.2.0, or 3.2.1 

(.NET for Apache Spark is not compatible with other versions of Apache Spark).

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/407568b5-0ef6-48e1-a9e1-61821ef0f93d)

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/d72ed255-d1e6-485a-9b44-02488eb65573)

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/2ec5f1fb-4f97-43b2-a9ca-6860c2df1a47)

After downloading the spark-3.2.0-bin-hadoop2.7.tgz file unZip it and place it in the following path: C:\bin\spark-3.2.0-bin-hadoop2.7

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/66c94d89-1d08-41a3-84dd-4fd843048abf)

Then we set the SPARK_HOME and the HADOOP_HOME environmental variables and we add them to the PATH variable

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/a8e85edf-3c95-49e4-a0f4-d3a448df6b6f)

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/f28317de-9a18-45dd-bc20-d847ea91ef5c)

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/50650f5e-9ea1-4a8e-b51f-5dce79a0b3ca)

Now we restart our computer.

We open a new command prompt and run the following command to confirm Spark is installed fine

```
spark-submit --verion
```

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/c17e6941-1fe2-49be-b25e-71622bf0ed13)


