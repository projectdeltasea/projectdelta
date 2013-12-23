Rebuild a million customer company in Haskell
============

TL;DR: rewrite an entire PHP shop into Haskell. We're hiring 6 Haskellers. Contact us on projectdeltasea@gmail.com.

##Summary

We are an online retail shop with millions of customers, and 9 digit USD funding. The PHP core is failing. We have budget and backing to rebuild everything, starting with the core and moving to the external service providers, in Haskell, taking the time to do it properly. A Haskell skeleton team is already in place and built a few things very well and very fast which is why this is happening. There's even a new CTO as the old one was a bit too vocal with his view that "Haskell is an impractical, niche academic language that will disappear in a couple of years". Now we are hiring half a dozen robust, experienced Haskellers to execute the project.

Build the largest customer facing Haskell company yet, and prove that Haskell truly is a general purpose programming language. We mean it. EVERYTHING gets rebuilt. Aside from showing the world that Haskell is practical and a great choice in such a setting, you're also showing that it's possible to do it as a rewrite, and developing and open sourcing libraries to help other companies transition quickly and robustly.

##Details

In a low tax, very comfortable first world city with warm weather, loads of trees and clean air. No project management structure - work directly with the users. No corporate bureaucracy - wear shorts to work and turn up at lunchtime if you want. Remote work will be considered - the technical lead has experience managing a remote team. 

The work stream will be up to you as a team. The current codebase is a single spaghetti-like 200k-line PHP repo, inherited from outside the company and a perpetual source of mystery even to those who worked on it here. The new infrastructure will be modular and as close to purely functional as possible (think service-oriented architecture). 
We think the following will happen:

1. rewrite of shop core, front end, and everything currently in PHP;

2. rewrite of every external solution: activity tracking, inventory management, buying planning, financial reporting...;

3. build and improve the above, for example by making the shop adapt to the customer with every action they take.

We all contribute to the open source community, as such you will be encouraged to open source a lot of your code and blog about your work. 

We do not care about your CV, educational institution, cover letter or hobbies. We estimate ability, and will measure your future performance, based on your code and experience. As such, you have three options:

1. solve the below and email your code and results; 

2. link us to your existing, substantial open source contributions in Haskell;

3. best of 7 StarCraft II HoS matches with one of the Haskellers here (not recommended if your APM < 200).

Send your choice to projectdeltasea@gmail.com. We will respond quickly and HR is not involved except post-offer to get your visa.

##Task

Write a program for authenticating employees of a company for access to various internal tools. The company has decided that:
- users are identified by an email address;
- each user belongs to 1 or more groups;
- each group is granted certain privileges.

For example, user `haskell.curry@projectdelta.com` belongs to `math` group. Group `math` has the following permissions:

- can read and send emails to the `math@projectdelta.com` mailing list
- can reserve conference rooms via `https://scheduling.office.projectdelta.com/`
- has read-only access to financial reports at `https://reports.finance.projectdelta.com/`

Administrators should be able to:

- create new users and groups
- grant permissions to a group
- list the permissions a user has
...and anything else you see fit to implement

The design and implementation is up to you, including the structure of the data and the interface you expose. For example, you could write a commandline tool, a TCP daemon, or a RESTful web service. The only other requirements are that the permissions must be persistent and it must be written in Haskell.
