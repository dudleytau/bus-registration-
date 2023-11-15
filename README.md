# Bus Registration System

Online Bus registration system for registering learners and securing a place in a bus. 

# Description

Impumelelo High School offers bus transport to and from school.

Learners who are currently registered to ride buses must re-register early (before or
on 1 November 2023) for the following year.

New learners must register early (before or on 1 November 2023) to secure a place
on a bus.

The fully completed bus registration form must be sent to
dnkosi@impumelolo.high.school.co.za OR handed in by hand.

Buses will run from the first day of school in the new school year.
Bus times may move approximately 10 minutes earlier OR later due to traffic
pressure or weather conditions.

Bus 1-3 use red tickets in 2024 (R420 for 20 journeys)
Tickets are available at Mrs. D Nkosi and payment can be made in cash or by card.

# Table of contents

1. [Application Name](#bus-registration-system)
2. [Description](#description)
3. [Pre-requisites](#pre-requisites)
4. [Tech specification](#tech-specification)
5. [How to Install and Run the Project](#how-to-install-and-run-the-project)
6. [Business Rules](#business-rules)

# Pre-requisites

##### XAMPP:
XAMPP is an easy to install Apache distribution containing MariaDB, PHP, and Perl. Just [download](https://www.apachefriends.org/download.html ) and start the installer. It's that easy.

##### Text Editor/IDE:
* Notepad++ - Download [here](https://notepad-plus-plus.org/downloads/)
* Intellij - Download [here](https://www.jetbrains.com/idea/download/?section=windows)
* Visual Studio Code (VSCode) - Download [here](https://code.visualstudio.com/). 

##### Git
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
Download [here](https://git-scm.com/). 


# Tech specification

##### HTML:
HTML is the standard markup language for Web pages.
##### PHP:
A popular general-purpose scripting language that is especially suited to web development.
Fast, flexible and pragmatic, PHP powers everything from your blog to the most popular websites in the world.

##### PHP Composer
A Dependency Manager for PHP for downloading dependencies and compiling PHP sources for 
autoload (injection of dependencies php classes)

##### MySQL/MariaDB:
MySQL is an open-source relational database management system.

##### Gitbub:
The AI-powered developer platform to build, scale, and deliver secure software. 

# How to Install and Run the Project

## Start up:
Open XAMPP Control Panel and start the following:

![img_1.png](img_1.png)

## Build

Change directory on your terminal to `C:\xampp\htdocs\bus-registration`. Make sure you completed the installation for [PHP composer](#php-composer)

Run:

```shell
composer dump-autoload
```
## Testing

### Online Bus Registration System
Click [here](http://localhost/bus-registration/public/index.php) to access the system and you should be presented with the login page:

![img.png](img.png)

### Test data:

#### Admin access: 

```text
Email: dnkosi@impumelolo.high.school.co.za
Password: admin
```

#### Parent access:

```text
Email: dudleytau@outlook.com
Password: parent
```

## Business Rules:

Business and system rules that demonstrate the functionality of the system. 


### Parent: 
```text
ONLY Parents are allowed to register themselves to have access to the bus application system.

A parent MUST register at least one learner after gaining access to the system and the learner will be associated to the parent that is registered them.

A parent can ONLY view and maintain their existing learnersâ€™ details.

A parent is NOT allowed to have access to management reports.

A parent can ONLY apply for a bus ticket(s) on behalf of learner(s) associated to them.
```


## System:

```text
An applicant (parent/admin) can ONLY apply for bus ticket(s) for learner(s) after the 1st of November every year for the following year.

An applicant is NOT allowed to apply multiple times for the same learner and for the same year. A system error will be presented.

An applicant is ONLY allowed to choose different time slots for morning PICK UPs/ afternoon DROP OFFs for the same route.

An application be will be automatically approved ONLY if a payment is made and there is capacity on the bus based on:

The year the  application is submitted for;
The route and time slot the bus is associated to.
The applicantâ€™s route and time slot they are choosing for the learner.

The system will generate a ticket with the right colour and a successful email WILL be sent to the parent.

The system will automatically place an application on waiting list if there is no capacity on the bus applied for and a waiting list email will be sent to the parent.

```

## Administrator:

```text
Administrator will have access to:
management reports,
system user management
Parents and learners registration
Applying for bus tickets for learnerâ€™s on behalf of parents.
