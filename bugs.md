## Introduction
Despite thorough testing, manual, BE, using DevTools Device toolbar I wasn't able to find any bug related to that component. Paths that I created were tested and time established for the tests has passed. 
Though I found something else that raised my attention. 

|Title                      | Values                         |
|------------               |--------------------------------|
|Reporter:  	            |Hubert Woźniak                  |
|Date:	                    |28.09.2023                      |
|Env: 	                    |https://en.footballteamgame.com/|
|Version:                   |	1.29                         |
|Browser:                   | 	Chrome Version 117.0.5938.92 |(Official Build) (64-bit)
|**Title:**	                |**Wrong email validation**	     |
|Description:	            | While registering mail with two dots in not allowed                                          |
|Priority:	                |Medium
|**Steps to reproduce:**	|1. Register to the game         |
|                           |2. Type mail: hubert.wozniak.    m@gmail.com
|                           |3. Provide passworde
|                           |4. Register
 Actual result	            | "error: ""Enter a valid e-mail address (E-mail aliases are not        supported) Too much dots in alias""   User is unable to create account. |
|Expected result	|A user with such an email should be able to register for the game, especially since the email hubert.wozniak@gmail.com is permissible. The validation rules for this field are unclear to me. Not allowing the creation of accounts for such emails may result in a potential loss of players. However, I understand that this validation may have been introduced for security purposes or to prevent misuse.
Attachement:                |	https://calip.io/J5uZ3jTR#DX7Kejtg


