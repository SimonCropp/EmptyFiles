<!--
GENERATED FILE - DO NOT EDIT
This file was generated by [MarkdownSnippets](https://github.com/SimonCropp/MarkdownSnippets).
Source File: /readme.source.md
To change this file edit the source file and then run MarkdownSnippets.
-->

# <img src="/src/icon.png" height="30px"> EmptyFiles

[![Build status](https://ci.appveyor.com/api/projects/status/dpqylic0be7s9vnm/branch/master?svg=true)](https://ci.appveyor.com/project/SimonCropp/EmptyFiles)
[![NuGet Status](https://img.shields.io/nuget/v/Verify.Xunit.svg?label=EmptyFiles)](https://www.nuget.org/packages/EmptyFiles/)

A collection of minimal binary files.

<!-- toc -->
## Contents

  * [NuGet package](#nuget-package)
  * [Usage](#usage)
    * [GetPathFor](#getpathfor)
    * [IsEmptyFile](#isemptyfile)
    * [AllPaths](#allpaths)<!-- endtoc -->

## NuGet package

 * https://nuget.org/packages/EmptyFiles/


## Usage


### GetPathFor

Gets the path to an empty file for a given extension

<!-- snippet: GetPathFor -->
<a id='snippet-getpathfor'/></a>
```cs
var path = EmptyFiles.GetPathFor("jpg");
```
<sup><a href='/src/EmptyFiles.Tests/Tests.cs#L12-L14' title='File snippet `getpathfor` was extracted from'>snippet source</a> | <a href='#snippet-getpathfor' title='Navigate to start of snippet `getpathfor`'>anchor</a></sup>
<!-- endsnippet -->


### IsEmptyFile

Returns true if the target file is an empty file.

<!-- snippet: IsEmptyFile -->
<a id='snippet-isemptyfile'/></a>
```cs
var path = EmptyFiles.GetPathFor("jpg");
Assert.True(EmptyFiles.IsEmptyFile(path));
var temp = Path.GetTempPath();
Assert.False(EmptyFiles.IsEmptyFile(temp));
```
<sup><a href='/src/EmptyFiles.Tests/Tests.cs#L22-L27' title='File snippet `isemptyfile` was extracted from'>snippet source</a> | <a href='#snippet-isemptyfile' title='Navigate to start of snippet `isemptyfile`'>anchor</a></sup>
<!-- endsnippet -->



### AllPaths

Enumerates all empty files

<!-- snippet: AllPaths -->
<a id='snippet-allpaths'/></a>
```cs
foreach (var path in EmptyFiles.AllPaths)
{
    Trace.WriteLine(path);
}
```
<sup><a href='/src/EmptyFiles.Tests/Tests.cs#L34-L39' title='File snippet `allpaths` was extracted from'>snippet source</a> | <a href='#snippet-allpaths' title='Navigate to start of snippet `allpaths`'>anchor</a></sup>
<!-- endsnippet -->


## Release Notes

See [closed milestones](../../milestones?state=closed).


## Icon

[Hollow](https://thenounproject.com/term/hollow/51835/) designed by [Michael Senkow](https://thenounproject.com/mhsenkow/) from [The Noun Project](https://thenounproject.com).
