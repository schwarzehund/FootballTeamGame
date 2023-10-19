# API Test Cases

## Test Case 1: Enhancing Non-User Items (API)
**Steps:**

1. Open Postman.
2. Create a request and add x-auth-id and x-auth-token to the headers.
3. In the request URL, select POST method
 https://api.en.footballteamgame.com/character/enchanting(itemid)
4. The item id should not belong to the current user.
5. In the request body, use:
   ```
   { 
    "use_golden_balls": 1,
   "special_item_id": 0
   }
   
6. Let's add some tests 

*Since we're trying to do something we're should be allowed to, probably status of the response should be 422.*
In **Test** tab add simple test 
```
pm.test("Status code is 422", function () {
   pm.response.to.have.status(422);
});
```
<img src ="https://github.com/schwarzehund/FootballTeamGame/blob/main/images/image (21).png">


7. Send the request 

**Expected Result:**
 
 **Status code 422**

 The response should be:
 ```
 {
    "error": "Selected item does not exist"
}
 ```
<img src ="https://github.com/schwarzehund/FootballTeamGame/blob/main/images/image3.png">

 ## Test Case 2: Enhancing Items Not Meant for Enhancement
**Steps:**

1. Open Postman.
2. Add a request, x-auth-id, and x-auth-token.
3. In the request URL, select POST method 
https://api.en.footballteamgame.com/character/enchanting/(itemid)
   The item id should belong to user but should be enchantable, for example, a blue item with id=4045123
5. In the request body, use: 
```
{
  "use_golden_balls": 1,
  "special_item_id": 1
}
```
6. Let's add some tests 

*Since we're trying to do something we're should be allowed to, probably status of the response should be 422.*
In **Test** tab add simple test 
```
pm.test("Status code is 422", function () {
   pm.response.to.have.status(422);
});
```
<img src="https://github.com/schwarzehund/FootballTeamGame/blob/main/images/image (21).png">

7. Send the request. 

**Expected result:**

**Status code 422**
Response: 
```
{
    "error": "Selected item does not exist"
}
```

<img src ="https://github.com/schwarzehund/FootballTeamGame/blob/main/images/image7.png">