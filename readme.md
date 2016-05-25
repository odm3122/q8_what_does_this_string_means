<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN">
<html>
  <head>

    <meta http-equiv="content-type" content="text/html; charset=UTF-8">
    <title>readme.md</title>
  </head>
  <body>
    <h1><span style="font-family:
Calibri;font-size:12pt;color:rgb(0,0,0);font-style:normal;font-variant:normal;">Q8
      </span></h1>
    <span style="font-family:
Calibri;font-size:12pt;color:rgb(0,0,0);font-style:normal;font-variant:normal;">What
      does follow string means?<span style="font-family:
        ;font-size:12pt;color:rgb(0,0,0);font-style:normal;font-variant:normal;">
        T3JkZXIgaXMgZm9yIGlkaW90cywgZ2VuaXVzIGNhbiBoYW5kbGUgY2hhb3M<br
          style=" font-style: normal; font-variant: normal; font-weight:
          normal; letter-spacing: normal; line-height: normal; orphans:
          2; text-align: -webkit-auto; text-indent: 0px; text-transform:
          none; white-space: normal; widows: 2; word-spacing: 0px;
          -webkit-text-size-adjust: auto; -webkit-text-stroke-width:
          0px; ">
      </span></span><span style="font-family:
Calibri;font-size:12pt;color:rgb(0,0,0);font-style:normal;font-variant:normal;"><br>
      <br style=" font-style: normal; font-variant: normal; font-weight:
        normal; letter-spacing: normal; line-height: normal; orphans: 2;
        text-align: -webkit-auto; text-indent: 0px; text-transform:
        none; white-space: normal; widows: 2; word-spacing: 0px;
        -webkit-text-size-adjust: auto; -webkit-text-stroke-width: 0px;
        ">
    </span>Answer:<br>
    <br>
    <span style="font-family:
Calibri;font-size:12pt;color:rgb(0,0,0);font-style:normal;font-variant:normal;">Your
      String has 61 characters and two "=" on the end first I thought it
      is a ssh public key but:<br>
      <br>
      ssh-keygen -l -f ~/temp/key<br>
      key_read: uudecode
      T3JkZXIgaXMgZm9yIGlkaW90cywgZ2VuaXVzIGNhbiBoYW5kbGUgY2hhb3M==
      testkey failed<br>
      line 1 too long: ssh-rsa T3JkZXIgaXMgZm9yIGlkaW90cywgZ2Vu...<br>
      <br>
      The I realized, that "openssl rand -base64 60" gives us always two
      "=" on the end... but "openssl rand -base64 44" (That is your
      string lenght) only&nbsp; one "="<br>
      <br>
      It must be a openssl generatet string but I did't found the exact
      meaning.<span style="font-family:
        ;font-size:12pt;color:rgb(0,0,0);font-style:normal;font-variant:normal;"><br
          style=" font-style: normal; font-variant: normal; font-weight:
          normal; letter-spacing: normal; line-height: normal; orphans:
          2; text-align: -webkit-auto; text-indent: 0px; text-transform:
          none; white-space: normal; widows: 2; word-spacing: 0px;
          -webkit-text-size-adjust: auto; -webkit-text-stroke-width:
          0px; ">
      </span></span><br>
    <br>
    <br>
    <br>
  </body>
</html>
