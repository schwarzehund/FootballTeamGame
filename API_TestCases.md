# API Test Cases

## Test Case 10: Enhancing Non-User Items (API)
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
6. Send the request 

**Expected Result:**
 The response should be:
 ```
 {
    "error": "Selected item does not exist"
}
 ```

 ## Test Case 11: Enhancing Items Not Meant for Enhancement
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
  "special_item_id": 0
}
```
6. Send the request. 
**Expected result:**
Response: 
```
{
    "error": "Selected item does not exist"
}
```