# Challenge Name: Javascript - Authentication 2

![Github](https://img.shields.io/badge/date-20.07.2021-brightgreen)  
![Github](https://img.shields.io/badge/category-Web-blueviolet)  
![Github](https://img.shields.io/badge/value-10-blue)  

## Description
Yes folks, Javascript is damn easy :)

## Detailed Solution
Opening the challenge link: http://challenge01.root-me.org/web-client/ch11/

![Screenshot 2021-07-20 134749](https://user-images.githubusercontent.com/79667858/126371409-dec305aa-4216-4cfd-b7b6-2d998a0f35ca.jpg)

We are directed to a page with two options: a login button and an option to close the tab

When the login button is clicked, we are alerted and prompted to enter a username and password. We don't know the username/password

Let's use the inspect element to view the files of this page

![Screenshot 2021-07-20 135735](https://user-images.githubusercontent.com/79667858/126372606-5e2cb83e-74ce-4321-a090-78924ea3e26d.jpg)

The index file doesn't seem to have anything of interest to us

Let's check out the javascript file

![Screenshot 2021-07-20 140056](https://user-images.githubusercontent.com/79667858/126373027-b98a71f2-d470-4e9b-958d-00976c0d39d7.jpg)

The variable TheLists consists of the value "GOD:HIDDEN"

Later on in the javascript file, we find that they split the TheLists value, separating the TheLists value into two parts by the colon

We find that the username equals the first part of the split, and the password equals the second part of the split

When logging in, the username should be "GOD" and the password "HIDDEN"

## Password
```
HIDDEN
```
