# cURL COMMAND
  * cURL is a computer software project providing a library and command-line tool for transferring data using various network protocols. The name stands for "Client URL"
  
### INSTALLATION OF cURL :
  * cURL can be installed using the following command
  
  ```console
  sudo apt install curl
  ```
  
### Getting started with cURL :
  - Accept Requests send by the server :
    ###### NOTE: cURL command when executed will return the body of the response sent by the server
    ```console
    fiesta@fiesta-VirtualBox:~/Desktop$ curl https://www.example.com
    <!doctype html>
    <html>
    <head>
      <title>Example Domain</title>
      <meta charset="utf-8" />
      <meta http-equiv="Content-type" content="text/html; charset=utf-8" />
    ....
    ```
  
    ###### NOTE: '--head' option will display only the head of the response
    ```console
    fiesta@fiesta-VirtualBox:~/Desktop$ curl --head http://www.example.com
    HTTP/1.1 200 OK
    Accept-Ranges: bytes
    Age: 413251
    Cache-Control: max-age=604800
    Content-Type: text/html; charset=UTF-8
    D ate: Tue, 11 Feb 2020 09:55:06 GMT
    Etag: "3147526947"
    Expires: Tue, 18 Feb 2020 09:55:06 GMT
    Last-Modified: Thu, 17 Oct 2019 07:18:26 GMT
    Server: ECS (nyb/1D13)
    X-Cache: HIT
    Content-Length: 1256

    fiesta@fiesta-VirtualBox:~/Desktop$
    ```
    ###### NOTE: '-o' option is used to save the response in a file
    ```console
    fiesta@fiesta-VirtualBox:~/Desktop$ curl -o output.txt http://www.example.com
      % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                     Dload  Upload   Total   Spent    Left  Speed
    100  1256  100  1256    0     0    437      0  0:00:02  0:00:02 --:--:--   437
    fiesta@fiesta-VirtualBox:~/Desktop$ cat output.txt
    <!doctype html>
    <html>
    <head>
        <title>Example Domain</title>
        <meta charset="utf-8" />
        <meta http-equiv="Content-type" content="text/html; charset=utf-8" />
    ....
    ```
    
    ###### NOTE: '-O' will download the response file,as in the example it downloads the manual.html file 
    ```console
    fiesta@fiesta-VirtualBox:~/Desktop$ ls
    output.txt
    fiesta@fiesta-VirtualBox:~/Desktop$ curl -O https://curl.haxx.se/docs/manual.html
      % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                     Dload  Upload   Total   Spent    Left  Speed
    100 44194  100 44194    0     0   9781      0  0:00:04  0:00:04 --:--:--  9783
    fiesta@fiesta-VirtualBox:~/Desktop$ ls
    manual.html  output.txt
    fiesta@fiesta-VirtualBox:~/Desktop$ cat manual.html
    <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
    <html>
    <head> <TITLE>curl - Tutorial</TITLE>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta content="text/html; charset=UTF-8" http-equiv="Content-Type">
    <link rel="stylesheet" type="text/css" href="https://curl.haxx.se/curl.css">
    .....
    ```
  
  - Refer for more: [Link to cURL Documentation](https://curl.haxx.se/docs/httpscripting.html)
  
  - Refer for more: [Link to cURL Options](https://curl.haxx.se/docs/manual.html)
