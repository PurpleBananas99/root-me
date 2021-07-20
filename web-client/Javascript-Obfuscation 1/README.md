# Challenge Name: Javascript - Obfuscation 1

![Github](https://img.shields.io/badge/date-20.07.2021-brightgreen)  
![Github](https://img.shields.io/badge/category-Web-blueviolet)  
![Github](https://img.shields.io/badge/value-10-blue)  

## Description
None

## Detailed Solution
Opening the challenge link: http://challenge01.root-me.org/web-client/ch4/ch4.html

![Screenshot 2021-07-20 141922](https://user-images.githubusercontent.com/79667858/126375321-d388b19d-334c-4ea9-b865-d31ab59178df.jpg)

We are directed to enter a password, but we don't know the password

Let's open up inspect element to find anything interesting

![Screenshot 2021-07-20 143024](https://user-images.githubusercontent.com/79667858/126376841-1a0243b8-8e36-4f2e-bc90-c05f9959d9dd.jpg)

```javascript
pass = '%63%70%61%73%62%69%65%6e%64%75%72%70%61%73%73%77%6f%72%64';
h = window.prompt('Entrez le mot de passe / Enter password');
if(h == unescape(pass)) {
    alert('Password accepté, vous pouvez valider le challenge avec ce mot de passe.\nYou an validate the challenge using this pass.');
} else {
    alert('Mauvais mot de passe / wrong password')
}
```
This snippet looks pretty interesting, as the password seems to be hexadecimal

The unescape function will convert hexadecimal sequences to the character(s) that they represent

Let's go to https://beautifier.io to unescape the hexadecimal sequence

```
%63%70%61%73%62%69%65%6e%64%75%72%70%61%73%73%77%6f%72%64
```

![Screenshot 2021-07-20 143612](https://user-images.githubusercontent.com/79667858/126377437-a78f216f-61b4-4765-b594-e81bef88861e.jpg)

Paste this hexadecimal sequence into the text-box, and it should return your password: 'cpasbiendurpassword'

## Password
```
cpasbiendurpassword
```
