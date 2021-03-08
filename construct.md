## The construction: ##

- `<!doctype html>`
- `<head>`
- `<meta ...>`
- `<style  src="data:base64,...">additionals as plain-text here</style>`
- `<script src="data:base64,...">additionals as plain-text here</script>`
- `</head>`
- `<frameset name="so" id="what" rows="*,...">`
- `<frame src='data:base64,...'>`
- `<frame src='data:base64,...'>`
- `...`
- `</frameset>`
- `</html>`

*That's a very very simple thing:* While reading all these manuals, comments, specifications, references and so on... you will notice the little universal mind inside. So it's the easiest way, to bringup the happy-bytes into a regular functionality out as one file. Any essentials should be inside the base64 data. 

*Remember:* Every frame maybe like a autonomous window. So we have a good base to split the requirements into that, whats needed in every of it. 

If you think, it's crypted, maybe! There are many ways to format a content. We use it as technic tactical, not really as a encryption. This part is a part of the deeper parts. Let's get it step by step! 

---

- HTML FRAMESET 0

---

- FRAME 1 SRC DATA:BASE64
- \ -> HTML JS DATA:BASE64
-  |-> CONTENT DATA:(AES256, SHA512)
-  |-> CONFIG5 DATA:(AES256, SHA512)
- - \ -> HTML5 DATA:BASE64
- - - \ -> APP DATA:BASE64
- - - | -> APP CONTENT DATA:(AES256, SHA512)
- - - | -> APP CONFIG DATA:(AES256, SHA512)

---

- FRAME 2 SRC DATA:BASE64
- \ -> HTML JS DATA:BASE64
-  |-> CONTENT DATA:(AES256, SHA512)
-  |-> CONFIG5 DATA:(AES256, SHA512)
- - \ -> HTML5 DATA:BASE64
- - - \ -> APP DATA:BASE64
- - - | -> APP CONTENT DATA:(AES256, SHA512)
- - - | -> APP CONFIG DATA:(AES256, SHA512)

---

- FRAME 3 SRC DATA:BASE64
- \ -> HTML JS DATA:BASE64
-  |-> CONTENT DATA:(AES256, SHA512)
-  |-> CONFIG5 DATA:(AES256, SHA512)
- - \ -> HTML5 DATA:BASE64
- - - \ -> APP DATA:BASE64
- - - | -> APP CONTENT DATA:(AES256, SHA512)
- - - | -> APP CONFIG DATA:(AES256, SHA512)

---

...and so on. 

Right, it's a n-dimensional replicatable. But it's not really useful for the most, to use more than 10 frames per frameset. Notice, that every of it must not be visible! We can show, hide and resize it. If a frame is hidden, it's active too against visibility. Nice, if you like to process some jobs and services hiddenly. Very nice too, that we can interact between the frames. 

The great little one will be a base, to set up own services like a fused IPC-Y to any device. 

Next step will be the applications. By the princip we can put anything there. It's not our mission to embed any frameworks there. We make our own as soon as possbile. 

*First the basics, we need:*
- LOCAL_STORAGE DB that contains just DB of DB's in crypted, keyless content
- \ ->USER, GROUP, ANONYMOUS
- | ->READ, WRITE, UPDATE, REPLACE, DELETE, PRIVACY
- | ->IPC-Y, NOTIFIER, ...
- | ->GROUPS, BOARDS, BLOGS, CHATS, ...
- | ->NETWORK, MESH, ...

The BASE64 will be a stablizer, to taint the AES256 DATA through the transport. It will need more traffic per process, but we reduce the rate of failed transmissions.

*The Network as a phantom:*

Most popular platforms require a central server. We bypass that and are our own one! 

Building friendships or equivalent relationships contains different options to share different contents between the servers and clients. So the servers coordinates the information transport. 

*Shortenly said:* The essentials to build up a infrastructure.
