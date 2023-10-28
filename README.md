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

## 1. Install .NET

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

## 2. Install Java 8 (JDK)

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

## 3. Install compression software

Apache Spark is downloaded as a compressed .tgz file. 

Use an extraction program, like 7-Zip or WinZip, to extract the file.

## 4. Install Apache Spark

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

## 5. Install Microsoft.Spark.Worker

Download the Microsoft.Spark.Worker release from the .NET for Apache Spark GitHub. 

For example if you're on a Windows machine and plan to use .NET Core, download the Windows x64 netcoreapp3.1 release.

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/98225162-39db-47bf-90be-850983f4ee27)

After downloading the compressed file "Microsoft.Spark.Worker.netcoreapp3.1.win-x64-2.1.1" place it in C:\bin\ 

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/fda049e2-c7c5-4310-9cbd-80ad3de2e6d5)

## 6. Create a new environmental variable DOTNET_WORKER_DIR to store the Microsoft.Spark.Worker installation folder

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/dd26111d-3f64-4d9e-b3f8-8b1fade7fec3)

## 7. Install WinUtils (Windows only)

.NET for Apache Spark requires WinUtils to be installed alongside Apache Spark. 

Download winutils.exe

https://github.com/steveloughran/winutils/tree/master

Then, copy WinUtils into C:\bin\spark-3.0.1-bin-hadoop2.7\bin

![image](https://github.com/luiscoco/.NET-for-Apache-Spark/assets/32194879/cb2db9b6-caf4-4409-b969-d99c72cae2e9)

## 8. Create a .NET console application

Open a command prompt window and run the following command to create a console .NET application

```
dotnet new console -o MySparkApp
cd MySparkApp
```
The dotnet command creates a new application of type console for you. 

The -o parameter creates a directory named MySparkApp where your app is stored and populates it with the required files. 

The cd MySparkApp command changes the directory to the app directory you created.


## 9. Install NuGet package

To use .NET for Apache Spark in an app, install the Microsoft.Spark package. 

In your command prompt or terminal, run the following command:

```
dotnet add package Microsoft.Spark
```

## 10. Write your app

Open Program.cs in Visual Studio Code, or any text editor, and replace all of the code with the following:

```csharp
using Microsoft.Spark.Sql;
using static Microsoft.Spark.Sql.Functions;

namespace MySparkApp
{
    class Program
    {
        static void Main(string[] args)
        {
            // Create Spark session
            SparkSession spark =
                SparkSession
                    .Builder()
                    .AppName("word_count_sample")
                    .GetOrCreate();

            // Create initial DataFrame
            string filePath = args[0];
            DataFrame dataFrame = spark.Read().Text(filePath);

            //Count words
            DataFrame words =
                dataFrame
                    .Select(Split(Col("value")," ").Alias("words"))
                    .Select(Explode(Col("words")).Alias("word"))
                    .GroupBy("word")
                    .Count()
                    .OrderBy(Col("count").Desc());

            // Display results
            words.Show();

            // Stop Spark session
            spark.Stop();
        }
    }
}
```

**SparkSession** is the entrypoint of Apache Spark applications, which manages the context and information of your application. 

Using the **Text method**, the text data from the file specified by the filePath is read into a DataFrame. 

A **DataFrame** is a way of organizing data into a set of named columns. Then, a series of **transformations** is applied to split the sentences in the file, group each of the words, count them and order them in descending order. The result of these operations is stored in another DataFrame. 

Note that at this point, no operations have taken place because .NET for Apache Spark **lazily evaluates the data**. 

It's not until the **Show** method is called to display the contents of the words transformed DataFrame to the console that the **operations** defined in the lines above **execute**.

Once you no longer need the Spark session, use the **Stop** method to stop your session.

## 11. Create data file

Your app processes a file containing lines of text. 

Create a file called **input.txt** file in your **MySparkApp directory**, containing the following text:

```
Hello World
This .NET app uses .NET for Apache Spark
This .NET app counts words with Apache Spark
Save the changes and close the file.
```

