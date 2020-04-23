﻿# Prism

Prism is a framework for building loosely coupled, maintainable, and testable XAML applications in WPF, and Xamarin Forms. Separate releases are available for each platform and those will be developed on independent timelines. Prism provides an implementation of a collection of design patterns that are helpful in writing well-structured and maintainable XAML applications, including MVVM, dependency injection, commands, EventAggregator, and others. Prism's core functionality is a shared code base supported in .NET Standard 2.0, .Net Core 3, and .NET Framework 4.5. Those things that need to be platform specific are implemented in the respective libraries for the target platform. Prism also provides great integration of these patterns with the target platform. For example, Prism for Xamarin Forms allows you to use an abstraction for navigation that is unit testable, but that layers on top of the platform concepts and APIs for navigation so that you can fully leverage what the platform itself has to offer, but done in the MVVM way.

Prism 7 is a fully open source version of the Prism guidance [originally produced by Microsoft patterns & practices](https://devblogs.microsoft.com/dotnet/prism-grows-up/). The core team members were all part of the P&amp;P team that developed Prism 1 through 5, and the effort has now been turned over to the open source community to keep it alive and thriving to support the .NET community. There are thousands of companies who have adopted previous versions of Prism, and we hope they will continue to move along with us as we continue to evolve and enhance the framework to keep pace with current platform capabilities and requirements.

## Help Support Prism

As most of you know, it takes a lot of time and effort for our small team to manage and maintain Prism in our spare time. Even though Prism is open source and hosted on GitHub, there are a number of costs associated with maintaining a project such as Prism.  Please be sure to Star the Prism repo and help sponsor Dan and Brian on GitHub.

- Sponsor [Brian Lagunas](https://xam.dev/sponsor-prism-brian)
- Sponsor [Dan Siegel](https://xam.dev/sponsor-prism-dan)

## Build Status

|          | Status |
| -------- | ------ |
| Full Build | [![Build Status](https://dev.azure.com/prismlibrary/Prism/_apis/build/status/Prism-CI?branchName=master&stageName=Build%20Prism%20Library)](https://dev.azure.com/prismlibrary/Prism/_build/latest?definitionId=9&branchName=master) |
| Prism.Core | [![Build Status](https://dev.azure.com/prismlibrary/Prism/_apis/build/status/Prism-CI?branchName=master&stageName=Build%20%26%20Test&jobName=Prism.Core)](https://dev.azure.com/prismlibrary/Prism/_build/latest?definitionId=9&branchName=master) |
| Prism.Wpf | [![Build Status](https://dev.azure.com/prismlibrary/Prism/_apis/build/status/Prism-CI?branchName=master&stageName=Build%20%26%20Test&jobName=Prism.Wpf)](https://dev.azure.com/prismlibrary/Prism/_build/latest?definitionId=9&branchName=master) |
| Prism.Forms | [![Build Status](https://dev.azure.com/prismlibrary/Prism/_apis/build/status/Prism-CI?branchName=master&stageName=Build%20%26%20Test&jobName=Prism.Forms)](https://dev.azure.com/prismlibrary/Prism/_build/latest?definitionId=9&branchName=master) |

### E2E Build Status

| E2E App | Status |
|---------|:------:|
| WPF | [![Build Status](https://dev.azure.com/prismlibrary/Prism/_apis/build/status/Prism-CI?branchName=master&stageName=End%20to%20End&jobName=E2E%20WPF%20App)](https://dev.azure.com/prismlibrary/Prism/_build/latest?definitionId=9&branchName=master) |
| Xamarin iOS | [![Build Status](https://dev.azure.com/prismlibrary/Prism/_apis/build/status/Prism-CI?branchName=master&stageName=End%20to%20End&jobName=E2E%20iOS%20App)](https://dev.azure.com/prismlibrary/Prism/_build/latest?definitionId=9&branchName=master) |
| Xamarin Android | [![Build Status](https://dev.azure.com/prismlibrary/Prism/_apis/build/status/Prism-CI?branchName=master&stageName=End%20to%20End&jobName=E2E%20Android%20App)](https://dev.azure.com/prismlibrary/Prism/_build/latest?definitionId=9&branchName=master) |

## Support

- Documentation is maintained in [the Prism-Documentation repo](https://github.com/PrismLibrary/Prism-Documentation) under /docs and can be found in a readable format on [the website](http://prismlibrary.com/docs/).
- For general questions and support, post your questions on [StackOverflow](http://stackoverflow.com/questions/tagged/prism).
- You can enter bugs and feature requests in our [Issues](https://github.com/PrismLibrary/Prism/issues/new/choose).

## Videos &amp; Training

By watching our courses, not only do you help support the project financially, but you might also learn something along the way.  We believe this is a win-win for everyone.

- [Introduction to Prism](https://app.pluralsight.com/library/courses/prism-introduction/table-of-contents)
- [What's New in Prism 5.0](https://app.pluralsight.com/library/courses/prism-50-whats-new/table-of-contents)
- [Prism Problems & Solutions: Showing Multiple Shells](https://app.pluralsight.com/library/courses/prism-showing-multiple-shells/table-of-contents)
- [Prism Problems & Solutions: Mastering TabControl](https://app.pluralsight.com/library/courses/prism-mastering-tabcontrol/table-of-contents)
- [Prism Problems & Solutions: Loading Modules Based on User Roles](https://app.pluralsight.com/library/courses/prism-loading-modules-user-roles/table-of-contents)
- [Prism Problems & Solutions: Loading Dependent Views](https://app.pluralsight.com/library/courses/prism-problems-solutions/table-of-contents)

We appreciate your support.

### Twitch

Both Brian and Dan are streaming live on a regular basis covering topics for WPF and Xamarin.Forms developers. Be sure to follow and subscribe to find out when they go live.

- [Brian Lagunas](https://twitch.tv/brianlagunas)
- [Dan Siegel](https://twitch.tv/dansiegel)

## NuGet Packages

Official Prism releases are available on NuGet. Prism also has a MyGet feed which will be updated with each merged PR. If you want to take advantage of a new feature as soon as it's merged into the code base, or if there is a critical bug you need fixed we invite you to try the packages on this feed. Our feed is a public feed in the MyGet Gallery.

Simply add `https://www.myget.org/F/prism/api/v3/index.json` as a package source to either Visual Studio or Visual Studio for Mac.

### Core Packages

These are the base packages for each platform, together with the Prism's Core assembly as a cross-platform PCL.

| Platform | Assembly | Package | NuGet | MyGet | Targets |
| -------- | -------- | ------- | ------- | ----- | ------ |
| Cross Platform | Prism.dll | [Prism.Core][CoreNuGet] | [![CoreNuGetShield]][CoreNuGet] | [![CoreMyGetShield]][CoreMyGet] | net45, net47, netstandard2.0 |
| WPF | Prism.Wpf.dll | [Prism.Wpf][WpfNuGet] | [![WpfNuGetShield]][WpfNuGet] | [![WpfMyGetShield]][WpfMyGet] | net461, net47, net48, netcoreapp3.1 |
| Xamarin.Forms | Prism.Forms.dll | [Prism.Forms][FormsNuGet] | [![FormsNuGetShield]][FormsNuGet] | [![FormsMyGetShield]][FormsMyGet] | netstandard2.0 |

### Container-specific packages

Each supported IoC container has its own package assisting in the setup and usage of that container together with Prism. The assembly is named using this convention: Prism.*Container.Platform*.dll, e.g. **Prism.Unity.Wpf.dll**. Starting with version 7.0, Prism is moving to separate packages for each platform. Be sure to install the package for the Container and the Platform of your choice.

#### WPF

| Package | NuGet | MyGet |
|---------|-------|-------|
| [Prism.DryIoc][DryIocWpfNuGet] | [![DryIocWpfNuGetShield]][DryIocWpfNuGet] | [![DryIocWpfMyGetShield]][DryIocWpfMyGet] |
| [Prism.Unity][UnityWpfNuGet] | [![UnityWpfNuGetShield]][UnityWpfNuGet] | [![UnityWpfMyGetShield]][UnityWpfMyGet] |

#### Xamarin Forms

| Package | NuGet | MyGet |
|---------|-------|-------|
| [Prism.DryIoc.Forms][DryIocFormsNuGet] | [![DryIocFormsNuGetShield]][DryIocFormsNuGet] | [![DryIocFormsMyGetShield]][DryIocFormsMyGet] |
| [Prism.Unity.Forms][UnityFormsNuGet] | [![UnityFormsNuGetShield]][UnityFormsNuGet] | [![UnityFormsMyGetShield]][UnityFormsMyGet] |

#### Package Notices

- For developers using Unity with Prism 6, take note that the new Unity maintainer has made major breaking changes. This includes changing namespaces and the package structure. These changes were NOT made by the Prism team nor do we have any control over it. When upgrading to Prism 7 you will need to uninstall the existing Unity package as we now reference the Unity.Container NuGet.

![NuGet package tree](images/NuGetPackageTree.png)

A detailed overview of each assembly per package is available [here](http://prismlibrary.github.io/docs/getting-started/NuGet-Packages.html).

## Prism Template Pack

Prism now integrates with Visual Studio and Xamarin Studio to enable a highly productive developer workflow for creating WPF, and native iOS and Android applications using Xamarin.Forms.  Jump start your Prism apps with code snippets, item templates, and project templates for your IDE of choice.

### Visual Studio Gallery

The Prism Template Pack is available on the [Visual Studio Gallery](https://visualstudiogallery.msdn.microsoft.com/e7b6bde2-ba59-43dd-9d14-58409940ffa0).  To install, just go to Visual Studio -> Tools -> Extensions and Updates... then search for **Prism** in the online gallery:

![Visual Studio Gallery](images/prism-visual-studio-gallery.jpg)

## Plugins

There are certain things that cannot be added directly into Prism for various reasons. To handle these common tasks such as supporting PopupPage's in Xamarin Forms, there are Prism Plugins. You can find a number of Plugins available on NuGet from our maintainer [@DanJSiegel](https://twitter.com/DanJSiegel).

- [Prism.Plugin.Popups](https://github.com/dansiegel/Prism.Plugin.Popups) (Forms Only)
- [Prism.Plugin.Logging](https://github.com/dansiegel/Prism.Plugin.Logging) (Works on all Platforms)
  - Adds support for Syslog, Loggly, Graylog, Application Insights, &amp; App Center
- [Prism.Container.Extensions](https://github.com/dansiegel/Prism.Container.Extensions)
  - Adds advanced Container Registration abstractions
  - Adds DryIoc ContainerExtension with support for Microsoft.DependencyInjection.Extensions &amp; Splat. Uses a singleton pattern to allow initialization from a native platform
  - Provides an extended PrismApplication with additional error handling and platform specifics support for Prism.Forms

## Samples

For stable samples be sure to check out the samples repo for the platform you are most interested in.

- [Prism for WPF Samples](https://github.com/PrismLibrary/Prism-Samples-Wpf)
- [Prism for Xamarim.Forms](https://github.com/PrismLibrary/Prism-Samples-Forms)

## Contributing

We strongly encourage you to get involved and help us evolve the code base.

- You can see what our expectations are for pull requests [here](https://github.com/PrismLibrary/Prism/blob/master/.github/CONTRIBUTING.md).

### .NET Foundation

This project is part of the [.NET Foundation](http://www.dotnetfoundation.org/projects).

[CoreNuGet]: https://www.nuget.org/packages/Prism.Core/
[WpfNuGet]: https://www.nuget.org/packages/Prism.Wpf/
[FormsNuGet]: https://www.nuget.org/packages/Prism.Forms/

[DryIocWpfNuGet]: https://www.nuget.org/packages/Prism.DryIoc/
[UnityWpfNuGet]: https://www.nuget.org/packages/Prism.Unity/

[UnityFormsNuGet]: https://www.nuget.org/packages/Prism.Unity.Forms/
[DryIocFormsNuGet]: https://www.nuget.org/packages/Prism.DryIoc.Forms/

[CoreNuGetShield]: https://img.shields.io/nuget/vpre/Prism.Core.svg
[WpfNuGetShield]: https://img.shields.io/nuget/vpre/Prism.Wpf.svg
[FormsNuGetShield]: https://img.shields.io/nuget/vpre/Prism.Forms.svg

[DryIocWpfNuGetShield]: https://img.shields.io/nuget/vpre/Prism.DryIoc.svg
[UnityWpfNuGetShield]: https://img.shields.io/nuget/vpre/Prism.Unity.svg

[DryIocFormsNuGetShield]: https://img.shields.io/nuget/vpre/Prism.DryIoc.Forms.svg
[UnityFormsNuGetShield]: https://img.shields.io/nuget/vpre/Prism.Unity.Forms.svg

[CoreMyGet]: https://myget.org/feed/prism/package/nuget/Prism.Core
[WpfMyGet]: https://myget.org/feed/prism/package/nuget/Prism.Wpf
[FormsMyGet]: https://myget.org/feed/prism/package/nuget/Prism.Forms

[DryIocWpfMyGet]: https://myget.org/feed/prism/package/nuget/Prism.DryIoc
[UnityWpfMyGet]: https://myget.org/feed/prism/package/nuget/Prism.Unity

[UnityFormsMyGet]: https://myget.org/feed/prism/package/nuget/Prism.Unity.Forms
[DryIocFormsMyGet]: https://myget.org/feed/prism/package/nuget/Prism.DryIoc.Forms

[CoreMyGetShield]: https://img.shields.io/myget/prism/vpre/Prism.Core.svg
[WpfMyGetShield]: https://img.shields.io/myget/prism/vpre/Prism.Wpf.svg
[FormsMyGetShield]: https://img.shields.io/myget/prism/vpre/Prism.Forms.svg

[DryIocWpfMyGetShield]: https://img.shields.io/myget/prism/vpre/Prism.DryIoc.svg
[UnityWpfMyGetShield]: https://img.shields.io/myget/prism/vpre/Prism.Unity.svg

[DryIocFormsMyGetShield]: https://img.shields.io/myget/prism/vpre/Prism.DryIoc.Forms.svg
[UnityFormsMyGetShield]: https://img.shields.io/myget/prism/vpre/Prism.Unity.Forms.svg
