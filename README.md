# UWPFullScreenAcrylicApp
Sample to show Full Screen Acrylic App appearance

I noticed that on UWP, That background Window Acrylic effect does not work on a Page started at Full screen. Only after you restore it, the effect appears. Can you check this?

When start in Full Screen it seems that Acrylic effect is not drawn; Then try to restore the window, you will notice that the Acrylic effect works.

Microsoft Windows [versão 10.0.17133.1]

Target version:
Windows 10, version 1803 (10.0; Build 17125)

Min version:
Windows 10, version 1803 (10.0; Build 17125)

Microsoft Visual Studio Community 2017 Preview
Version 15.7.0 Preview 2.0

I Enabled it using

        public App()
        {
            Windows.UI.ViewManagement.ApplicationView.PreferredLaunchWindowingMode =
                Windows.UI.ViewManagement.ApplicationViewWindowingMode.FullScreen
                ;

            this.InitializeComponent();
            this.Suspending += OnSuspending;
        } 
        
and on the page:

    <Page
    x:Class="FullScreenAcrylicApp.MainPage"
    xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
    xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
    xmlns:local="using:FullScreenAcrylicApp"
    xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
    xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
    mc:Ignorable="d"
    Background="{StaticResource SystemControlAcrylicWindowBrush}">

    <Grid>
        <TextBlock>HELLO WORLD. 
            Check if the Acrylic Background is working.
            Restore window, maximize it.
        </TextBlock>

    </Grid>
    </Page>

Microsoft Visual Studio Community 2017 Preview
Version 15.7.0 Preview 2.0
VisualStudio.15.Preview/15.7.0-pre.2.0+27520.0
Microsoft .NET Framework
Version 4.7.03056

Installed Version: Community

Visual C++ 2017   00369-60000-00001-AA914
Microsoft Visual C++ 2017

Visual F# Tools 10.1 for F# 4.1   00369-60000-00001-AA914
Microsoft Visual F# Tools 10.1 for F# 4.1

Advanced Installer Extension   14.7
Advanced Installer Extension. For more information visit the Advanced Installer website at www.advancedinstaller.com. Copyright © Caphyon LTD. All rights reserved.

Application Insights Tools for Visual Studio Package   8.11.10212.1
Application Insights Tools for Visual Studio

ASP.NET and Web Tools 2017   15.0.40313.0
ASP.NET and Web Tools 2017

ASP.NET Core Blazor Language Services   0.1.0-rtm-10142

ASP.NET Core Razor Language Services   1.0
Provides languages services for ASP.NET Core Razor.

ASP.NET Web Frameworks and Tools 2017   5.2.60308.0
For additional information, visit https://www.asp.net/

AWS Toolkit for Visual Studio 2017   1.14.2.0
AWS Toolkit for Visual Studio 2017.
Copyright 2011-2018 Amazon.com, Inc. or its affiliates. All Rights Reserved.

Release notes: https://aws-vs-toolkit.s3.amazonaws.com/versioninfo.html

This software includes third party software subject to the following copyrights:
- Logging from log4net, Apache License 
  [http://logging.apache.org/log4net/license.html]
- Putty for PPK to PEM conversion, MIT license 
  [http://www.chiark.greenend.org.uk/~sgtatham/putty/licence.html]
- NGit for AWS Elastic Beanstalk incremental push
  [https://github.com/mono/ngit/blob/master/NGit.license.txt]
- NSch dependency for NGit
  [https://github.com/mono/ngit/blob/master/NSch.license.txt]
- Sharpen dependency for NGit
  [https://github.com/mono/ngit/blob/master/Sharpen/AssemblyInfo.cs]
- ICSharpCode.SharpZipLib dependency for NGit
  [http://www.icsharpcode.net/opensource/sharpziplib/]
- Mono.Posix.dll and Mono.Security.dll dependencies for NGit
  [http://mono-project.com/FAQ:_Licensing#Licensing]
- MPFProj for Visual Studio Project Framework
  [http://mpfproj10.codeplex.com/license]
- JSON Checker for JSON validation
  [http://www.raboof.com/projects/jsonchecker/]
- Newtonsoft Json.NET
  [http://www.newtonsoft.com/json] 
- YamlDotNet
  [http://aaubry.net/pages/yamldotnet.html] 
    

Azure App Service Tools v3.0.0   15.0.40308.0
Azure App Service Tools v3.0.0

Azure Data Lake Node   1.0
This package contains the Data Lake integration nodes for Server Explorer.

Azure Data Lake Tools for Visual Studio   2.3.3000.1
Microsoft Azure Data Lake Tools for Visual Studio

Azure Functions and Web Jobs Tools   15.0.40322.0
Azure Functions and Web Jobs Tools

Azure Stream Analytics Tools for Visual Studio   2.3.3000.1
Microsoft Azure Stream Analytics Tools for Visual Studio

C# Tools   2.8.0-beta1-62716-11. Commit Hash: e205ae181b97f10453eb1a21fa825637040c43b9
C# components used in the IDE. Depending on your project type and settings, a different version of the compiler may be used.

Common Azure Tools   1.10
Provides common services for use by Azure Mobile Services and Microsoft Azure Tools.

Conveyor by Keyoti   1.0
Allows you to access your web applications from other machines, even if hosted on the development web server.

DotNetForHtml5.VisualStudioExtension.ShellIntegration   1.0
DotNetForHtml5.VisualStudioExtension.ShellIntegration

Fabric.DiagnosticEvents   1.0
Fabric Diagnostic Events

GitHub.VisualStudio   2.4.3.1737
A Visual Studio Extension that brings the GitHub Flow into Visual Studio.

JavaScript Language Service   2.0
JavaScript Language Service

JavaScript Project System   2.0
JavaScript Project System

JavaScript UWP Project System   2.0
JavaScript UWP Project System

Merq   1.1.17-rc (cba4571)
Command Bus, Event Stream and Async Manager for Visual Studio extensions.

Microsoft Azure HDInsight Azure Node   2.3.3000.1
HDInsight Node under Azure Node

Microsoft Azure Hive Query Language Service   2.3.3000.1
Language service for Hive query

Microsoft Azure Service Fabric Tools for Visual Studio   2.0
Microsoft Azure Service Fabric Tools for Visual Studio

Microsoft Azure Stream Analytics Language Service   2.3.3000.1
Language service for Azure Stream Analytics

Microsoft Azure Stream Analytics Node   1.0
Azure Stream Analytics Node under Azure Node

Microsoft Azure Tools   2.9
Microsoft Azure Tools for Microsoft Visual Studio 2017 - v2.9.10222.3

Microsoft Continuous Delivery Tools for Visual Studio   0.3
Simplifying the configuration of continuous build integration and continuous build delivery from within the Visual Studio IDE.

Microsoft JVM Debugger   1.0
Provides support for connecting the Visual Studio debugger to JDWP compatible Java Virtual Machines

Microsoft MI-Based Debugger   1.0
Provides support for connecting Visual Studio to MI compatible debuggers

Microsoft Visual C++ Wizards   1.0
Microsoft Visual C++ Wizards

Microsoft Visual Studio Tools for Containers   1.1
Develop, run, validate your ASP.NET Core applications in the target environment. F5 your application directly into a container with debugging, or CTRL + F5 to edit & refresh your app without having to rebuild the container.

Microsoft Visual Studio VC Package   1.0
Microsoft Visual Studio VC Package

Mono Debugging for Visual Studio   4.10.4-pre (05a888d)
Support for debugging Mono processes with Visual Studio.

NuGet Package Manager   4.6.0
NuGet Package Manager in Visual Studio. For more information about NuGet, visit http://docs.nuget.org/.

ProjectServicesPackage Extension   1.0
ProjectServicesPackage Visual Studio Extension Detailed Info

RelayCommand Extension   1.0
RelayCommand Visual Studio Extension Detailed Info

SQL Server Data Tools   15.1.61801.210
Microsoft SQL Server Data Tools

ToolWindowHostedEditor   1.0
Hosting json editor into a tool window

TypeScript Tools   15.7.20307.2005
TypeScript Tools for Microsoft Visual Studio

Visual Basic Tools   2.8.0-beta1-62716-11. Commit Hash: e205ae181b97f10453eb1a21fa825637040c43b9
Visual Basic components used in the IDE. Depending on your project type and settings, a different version of the compiler may be used.

Visual Studio Code Debug Adapter Host Package   1.0
Interop layer for hosting Visual Studio Code debug adapters in Visual Studio

Visual Studio Tools for Unity   3.6.0.5
Visual Studio Tools for Unity

Visual Studio Tools for Universal Windows Apps   15.0.27520.00
The Visual Studio Tools for Universal Windows apps allow you to build a single universal app experience that can reach every device running Windows 10: phone, tablet, PC, and more. It includes the Microsoft Windows 10 Software Development Kit.

VisualStudio.Mac   1.0
Mac Extension for Visual Studio

Windows Machine Learning Generator Extension   1.0
Windows Machine Learning Visual Studio Extension Detailed Info

Xamarin   4.10.0.263 (bc1dc413e)
Visual Studio extension to enable development for Xamarin.iOS and Xamarin.Android.

Xamarin Designer   4.12.99 (3cb91a67f)
Visual Studio extension to enable Xamarin Designer tools in Visual Studio.

Xamarin.Android SDK   8.3.0.5 (HEAD/1a8ed5388)
Xamarin.Android Reference Assemblies and MSBuild support.

Xamarin.iOS and Xamarin.Mac SDK   11.10.0.32 (4d8c4e3)
Xamarin.iOS and Xamarin.Mac Reference Assemblies and MSBuild support.

XAML Editor (C#/XAML for HTML5)   1.0
(...)
