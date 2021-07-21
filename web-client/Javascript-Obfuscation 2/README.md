# Challenge Name: Javascript - Obfuscation 2

![Github](https://img.shields.io/badge/date-21.07.2021-brightgreen)
![Github](https://img.shields.io/badge/category-Web-blueviolet)
![Github](https://img.shields.io/badge/value-10-blue)

## Description
Going down 3 floors.....

## Detailed Solution
Opening the challenge link: http://challenge01.root-me.org/web-client/ch12/ch12.html

When we open up the link, we are just directed to a blank web page

Let's view the page source by doing 'ctrl + u'

![Screenshot 2021-07-21 172528](https://user-images.githubusercontent.com/79667858/126562258-a9836b17-a765-4624-9d5a-024f700b685e.jpg)

```javascript
unescape%28%22String.fromCharCode%2528104%252C68%252C117%252C102%252C106%252C100%252C107%252C105%252C49%252C53%252C54%2529%22%29
```

Let's copy whatever is in double quotes

Go to: http://www.utilities-online.info/urlencode/ since the js code said to unescape everything in the double quotes

Paste what was in the double quotes into the input and click 'Decode'

```javascript
unescape("String.fromCharCode%28104%2C68%2C117%2C102%2C106%2C100%2C107%2C105%2C49%2C53%2C54%29")
```

We only need to select this phrase:
```javascript
%28104%2C68%2C117%2C102%2C106%2C100%2C107%2C105%2C49%2C53%2C54%29
```

Put this into the decoder to get this:
```javascript
(104,68,117,102,106,100,107,105,49,53,54)
```
We now want to convert our decimals to string values

Go to: https://www.rapidtables.com/convert/number/ascii-hex-bin-dec-converter.html

In the Decimal section, copy & paste the list of numbers above, and you should get your password in the ASCII text section

## Password
```
hDufjdki156
```
