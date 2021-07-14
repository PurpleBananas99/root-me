# Challenge Name: Javascript - Authentication

![Github](https://img.shields.io/badge/date-14.07.2021-brightgreen)  
![Github](https://img.shields.io/badge/category-Web-blueviolet)  
![Github](https://img.shields.io/badge/value-5-blue)  

## Description
None

## Detailed Solution
Opening the challenge link: http://challenge01.root-me.org/web-client/ch9/

![Screenshot 2021-07-14 090712](https://user-images.githubusercontent.com/79667858/125627218-5bdf9c51-09dd-4871-83a2-d526efec1891.jpg)

When you try to log in, we see an alert saying "wrong password"

![Screenshot 2021-07-14 090858](https://user-images.githubusercontent.com/79667858/125627437-a07a2e23-cdf4-4b2d-9617-bd97ee36fea8.jpg)

Let's open up inspect element to view the files

We can see an index and a js file

![Screenshot 2021-07-14 091040](https://user-images.githubusercontent.com/79667858/125627649-262c4faf-082e-47d6-b092-89e158c9c67d.jpg)

The index file doesn't seem to have anything of interest to us

Let's look at the js file

![Screenshot 2021-07-14 091152](https://user-images.githubusercontent.com/79667858/125627839-05eac835-f1de-484a-a54c-a4588f1accf8.jpg)

Looking inside the if statement, we find that it asks for the username to be '4dm1n' and the password to be 'sh.org'

When logging in with these values, we are alerted that we can "validate the challenge using this password"

![Screenshot 2021-07-14 091410](https://user-images.githubusercontent.com/79667858/125628156-0c932205-1dd7-490b-badf-7a16db84c332.jpg)

## Password
```
sh.org
```
