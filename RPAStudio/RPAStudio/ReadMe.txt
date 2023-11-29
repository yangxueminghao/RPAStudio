1.在RPA.Core.Activities下bin/Debug下粘贴nuget.exe
2.Warning NU5133: NuGet.exe file on path \Downloads\nuget.exe needs to be unblocked after downloading.
问题:下载Windows上的文件时，在这种情况下，nuget.exe通过 Web 浏览器添加该文件Mark Of The Web。 这使得Windows认为，尽管来自已知来源，如 nuget.org，但标志可能很危险。因此，某些nuget.exe pack操作可能无法正常工作。
解决方案 1-->右键单击下载的副本 nuget.exe 并选择“属性”。-->NuGet Properties-->现在勾选 Unblock ，然后按应用。-->NuGet Unblock-->现在重试包操作。