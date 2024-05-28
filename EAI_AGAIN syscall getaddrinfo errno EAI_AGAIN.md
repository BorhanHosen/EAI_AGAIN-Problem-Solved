# npm ERR! code EAI_AGAIN
## I was browsing internet using a proxy address. When I wanted to create vite app for my react project, I faced this problem. 
``` create vite@latest     
npm ERR! code EAI_AGAIN
npm ERR! syscall getaddrinfo
npm ERR! errno EAI_AGAIN
npm ERR! request to https://registry.npmjs.org/create-vite failed, reason: getaddrinfo EAI_AGAIN registry.npmjs.org
npm ERR! A complete log of this run can be found in: C:\Users\borhan06344\AppData\Local\npm-cache\_logs\2024-05-28T06_50_36_004Z-debug-0.log 
   
## Then I was trying to solve this problem by some research, and finaly I got the solution. The solution was I had set in npm config. 

``` npm config set proxy http://10.32.20.40:8080 
```
![Screenshot (1)](https://github.com/BorhanHosen/EAI_AGAIN-Problem-Solved/assets/138838370/826c43d5-9ae9-4b99-a17a-d332f5c259fb)


![Screenshot (2)](https://github.com/BorhanHosen/EAI_AGAIN-Problem-Solved/assets/138838370/2885ab7d-429c-4f2d-b431-3eea08153cef)

Reference Link: [npm ERR! code EAI_AGAIN error when trying to install express](https://stackoverflow.com/questions/63010779/npm-err-code-eai-again-error-when-trying-to-install-express).
