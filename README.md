[![](https://img.shields.io/badge/organization-nikoschalikias-blue.svg)](https://github.com/nikoschalikias) 
[![](https://img.shields.io/badge/remote-ProjectBook-green.svg)](https://github.com/nikoschalikias/ProjectBook) 
[![](https://img.shields.io/badge/local-F:\ProjectBook-orange.svg)](https://github.com/iotmodular) 



# ProjectBook


Integration of multiple projects README.md to a single document

## Using gget
> *  For windows gget is a small downloadable **.exe** file
> *  For gget to work, a Release must exist in the remote github repo
> *  git Releases are based on tags  
> *  git tags are created locally and then pushed to github remote repo  
> *  A git Release can be created from gitHub web interface or from the locally installed gh-cli


### Worked gget examples

1.cmd
```
gget github.com/nikosLab/tubeToolHolder --type=blob hexagon-01.stl
```

2.cmd
```
gget github.com/nikosLab/tubeToolHolder --type=blob hexagon-02.stl
gget github.com/nikosLab/tubeToolHolder --type=blob hexagon-03.stl
gget github.com/nikosLab/tubeToolHolder --type=blob hexagon-05.stl
```

3.cmd
```
gget github.com/nikosLab/tubeToolHolder --type=blob tubeToolHolder01.stl
rename tubeToolHolder01.stl renamed.stl
```

----

## Using curl to get a single file from github

This worked for a [public repository](https://github.com/nikoschalikias/STM32F103C6_CAN2) :heavy_check_mark: 

```
curl -o eee.md  https://raw.githubusercontent.com/nikoschalikias/STM32F103C6_CAN2/master/README.MD
```

<p align="center">
<img
src="img/01.PNG"
width = 900
/>
</p>

### Worked curl example


This example gets a readme.md and renames it with the repository name.  
Makes exactly what needed for the ProjectBook concept, but only works for public repos.


```
5.cmd
curl -o STM32F103C6_CAN2.md  https://raw.githubusercontent.com/nikoschalikias/STM32F103C6_CAN2/master/README.MD
```

### cURL tasks

- [ ] Research if cURL can work with private github repos
- [ ] Review cURL documentation
- [ ] Review cURL github examples / videos
- [ ] Review how to call cURL from Python

#### cURL links
* [Python Curl Example](https://linuxhint.com/python-curl-example/)
* [PycURL -- A Python Interface To The cURL library](https://github.com/pycurl/pycurl)
* [How can I download a single raw file from a private github repo using the command line?](https://stackoverflow.com/questions/18126559/how-can-i-download-a-single-raw-file-from-a-private-github-repo-using-the-comman)
* [Creating a personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)


## Links

*  [gget](https://gget.io/#install)
*  [tubeToolHolder](https://github.com/nikosLab/tubeToolHolder)
*  [git  tag](https://git-scm.com/book/en/v2/Git-Basics-Tagging)
*  [Git Releases](https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases)
