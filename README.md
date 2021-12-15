
#  <img src="https://github.com/Ginger-Automation/Ginger/blob/master/GingerLogo.png" width="64"> Ginger Automation 
[![Build status](https://ci.appveyor.com/api/projects/status/1wcp41xf6q49988m/branch/master?svg=true)](https://ci.appveyor.com/project/ginger/ginger/branch/master)
[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/Ginger-Automation/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

Linux: [![Build Status](https://dev.azure.com/GingerByAmdocs/GingerByAmdocs/_apis/build/status/Ginger%20Linux%20Build?branchName=master)](https://dev.azure.com/GingerByAmdocs/GingerByAmdocs/_build/latest?definitionId=7?branchName=master) Windows: [![Build Status](https://dev.azure.com/GingerByAmdocs/GingerByAmdocs/_apis/build/status/Ginger%20Windows%20Build?branchName=master)](https://dev.azure.com/GingerByAmdocs/GingerByAmdocs/_build/latest?definitionId=6?branchName=master) Mac: [![Build Status](https://dev.azure.com/GingerByAmdocs/GingerByAmdocs/_apis/build/status/Ginger%20Mac%20Build?branchName=master)](https://dev.azure.com/GingerByAmdocs/GingerByAmdocs/_build/latest?definitionId=11&branchName=master)

Ginger is an Automation IDE, Drag & Drop automation, Can be used by users with or without coding skills, open platform with plugin capabilities.
- ### [Source Code](https://github.com/Ginger-Automation/Ginger)
- ### [Download Ginger](https://github.com/Ginger-Automation/Ginger/releases)
- ### [Ginger YouTube Channel](http://www.youtube.com/channel/UCQ2TRVoBhYi6zSU9r395EtQ/videos)
- ### [Online Help](https://ginger-automation.github.io/Ginger-Web-Help)


# Ginger Container Images for Execution
Available Images 


### [Ginger-Automation/GingerRuntime (ghcr.io/ginger-automation/gingerruntime)](https://github.com/orgs/Ginger-Automation/packages/container/package/gingerruntime) 
Light Weight image to run backend execution (Based on Alpine)<br/>
To Pull Image use : docker pull ghcr.io/ginger-automation/gingerruntime:latest 

### [Ginger-Automation/GingerRuntime - With Browsers (ghcr.io/ginger-automation/gingerruntime-browsers)](https://github.com/orgs/Ginger-Automation/packages/container/package/gingerruntime-browsers)
Created on top of Ginger-Runtime Image with Firefox and Chromium<br/>
To Pull Image use : docker pull ghcr.io/ginger-automation/gingerruntime-browsers:latest 

### [Ginger-Automation/Ginger: (ghcr.io/ginger-automation/ginger)](https://github.com/orgs/Ginger-Automation/packages/container/package/ginger) 
Windows Image used for executing backend automation on Windows <br/>
To Pull Image use : docker pull ghcr.io/ginger-automation/ginger:latest 
 

## To view help  
docker run {image Name} run --help  



## To Execute Runset from source control repository 
docker run {image Name} run -r "RunSetName"   -t SourceControlType --url "RepositoryUrl" --user "UserNameforSourcecontrol" --pass "Password for sourcecontrol" --solution "Foldert to dwonload solution "

### Arguments to Build run command 
-s, --solution             Required. Set solution folder

  -r, --runset               Required. Set runset name

  -e, --env                  (Default: Default) Set environment name

  -d, --do-not-analyze       runAnalyzer

  -i, --showui               (Default: false) Show Auto Run Window UI - Windows
                             only

  -a, --artifacts-path       Select Artifacts output directory

  -t, --type                 Source Control Management type i.e: GIT, SVN

  -h, --url                  Source Control URL

  -u, --user                 Source Control User

  -p, --pass                 Source Control Pass

  -g, --encrypted            password is encrypted

  -c, --ignoreCertificate    Ignore certificate errors while cloning solution

  -v, --verbose              (Default: normal) Select Verbose level: normal,
                             debug
