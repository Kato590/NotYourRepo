# Project 7 - WordPress Pentesting

Time spent: **30** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) Exploit Using XSS 
  - [ ] Summary: 
  This exploit is using XSS. You have to enter a malcious comment with more than 62kb in size. After that, log in as the admin and click on or move the mouse over the comment, depending on which XSS method you use. Then, you the attacker can access the backdoor.
  But My Virtual machine was acting up and could not access the backdoor. 
    - Vulnerability types: 
    XSS
    - Tested in version: 
    4.2
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  ![GIF](https://giphy.com/gifs/1mgnbgjGX5bsAR2c2R)
  - [ ] Steps to recreate: 
  >Enter a comment like the following: `<a title='x onmouseover=alert(unescape(/hello%20world/.source)) style=position:absolute;left:0;top:0;width:5000px;height:5000px  AAAAAAAAAAAA...[64 kb]..AAA'></a>`
  (It has to have more than 65,000 characters.)
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)


## Assets


## Resources
- [WordPress 4.2 - Persistent Cross-Site Scripting](https://www.exploit-db.com/exploits/36844/)
- [GIPHY](https://giphy.com/)
- [YouTube](https://www.youtube.com/watch?v=OCqQZJZ1Ie4)
- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Since there was no clear and solid explanation on how to set up the envinroment for Week 7 on a Windows host machine, it took me more than 10 hours to just set it up. I hope no one assumes every student has a Linux or Mac OS host computers. It was totally unfair.


## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
