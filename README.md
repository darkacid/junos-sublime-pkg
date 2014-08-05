junos-sublime-pkg
=================

**Junos Config Syntax Highlighting for Sublime Text**  

### Description  
This is a Sublime Text 2 package to highlight the syntax for configurations on Juniper Junos (EX, MX, SRX) devices. It will work for configurations both in set mode and stanza form.  

### Installation
Currently I am waiting for this package to be accepted into [Package Control](https://sublime.wbond.net/installation). If it is accepted, then this would be the easiest method of installation. To install manually, simply download the lastest release [here](https://github.com/nprintz/junos-sublime-pkg/tags), and drop the two `.tmLanguage` files into your `Packages/User` folder. The Packages folder can be found by going to the `Sublime Text 2` > `Preferences` > `Browse Packages` menu option. 

### Matches  
Name  | Description  
------|------------  
Comment Block or Annotation | For annotations in stanza mode: `/* Some Text */`  
Line Comment | Anything after a number sign, `#`, on a line  
Major Sections | Matches major sections of the config and the preceeding keyword (if set mode). For example, `set system host-name` would highlight `set` as a control keyword, and `system` as a major category (entity.name.function.junos)  
Minor Sections | Same as major sections, just for more of the less common sections of Junos config  
Interface names | Highlights interface names  
IPv4 and IPv6 addresses | All addresses get highlighted as a number  
Unit numbers | Unit numbers get highlighted as a number  
User defined arbitrary names | These get highlighted as a variable. Examples include the names of logical-systems, filters, prefix-lists, policies, NAT rules, security zones, policers, etc  
Strings | Anything between single- or double-quotes ( ' or " ) gets marked as a string. This also includes any word block after the keyword description, which may not be quoted  

### Examples  
Examples with the `Twilight` color scheme:

Set mode:  
![Set Mode](https://cloud.githubusercontent.com/assets/7231007/3803665/5fb3e326-1c1d-11e4-80fd-9b222f8a1abf.png)

Stanza mode:  
![Stanza Mode](https://cloud.githubusercontent.com/assets/7231007/3803687/81b640e0-1c1d-11e4-9dd6-f228e4c4275d.png)