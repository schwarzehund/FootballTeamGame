
# TEST CASES

## Test Case 1: Access to the Enhancement Feature
**Steps:**

1. Log in to the game.
2. Go to the Character (left panel) > Locker tab.
3. Check the availability of the Enhancement feature.

**Expected Result:** The Enhancement feature should be available in the Locker tab.

## Test Case 2: Checking Items for Enhancement
**Steps:**

1. Log in to the game.
2. Go to the Character (left panel) > Locker > Enhancement tab.
3. Check if the appropriate items are in the correct color sections.

**Expected Result:** Enhancement should be allowed for green, red, and gold items, while the presence of blue and gray items is an error.

## Test Case 3: Enhancement Options
**Steps:**

1. Log in to the game.
2. Go to the Character (left panel) > Locker > Enhancement tab.
3. Select an item.
4. Verify that the item appears in the "Enhancement" section, a cost for enhancement is displayed, the "Enhance" button is highlighted, and the checkbox for using Golden Balls is available to check.

**Expected Result:** 
1. The item should appear in the "Enhancement" section
2. Cost for enhancement should be displayed, 
3. The "Enhance" button should be highlighted,
4. Checkbox for using Golden Balls should be available to check, but only for previously enhanced items. T
5. he dropdown for selecting special balls should be clickable, with the only displayed value being — in case of a lack of balls.

## Test Case 4: Enhancement
**Steps:**

1. Log in to the game.
2. Go to the Character (left panel) > Locker > Enhancement tab.
3. Select a never-upgraded item.
4. Click "Enhance."

**Expected Result:** The enhanced item should receive skill and UM bonuses. With each subsequent attempt, the enhancement chance decreases, and there is a risk of lowering the level in case of a failed enhancement.

## Test Case 5: Failed Enhancement
**Steps:**

1. Log in to the game.
2. Go to the Character (left panel) > Locker > Enhancement tab.
3. Select an item with a low chance of enhancement.
4. Attempt to enhance an item with a specified risk level (Low).
5. Verify the result of the enhancement attempt.

**Expected Result:** A failed enhancement should leave the item at its current level.

### Test Case 5a: Item Degradation
**Steps:**

1. Log in to the game.
2. Go to the Character (left panel) > Locker > Enhancement tab.
3. Select an item with a high chance of enhancement.
4. Attempt to enhance an item with a specified risk level (HIGH/MEDIUM).
5. Verify the result of the enhancement attempt.

**Expected Result:** In case of a successful enhancement but a high risk of failure, the item should be degraded by one level, and UM points should be deducted. After the item's degradation, the risk level should decrease for the next enhancement attempt.

### Test Case 5b: Insufficient Euro
**Steps:**

1. Log in to the game.
2. Go to the Character (left panel) > Locker > Enhancement tab.
3. Select a green item.
4. Click "Enhance."

**Expected Result:** An error toast message should appear stating "Insufficient Euro," and the enhancement should not proceed.

### Test Case 5c: Insufficient Golden Balls
Steps:

1. Log in to the game.
2. Go to the Character (left panel) > Locker > Enhancement tab.
3. Select a green item.
4. Check the checkbox for using Golden Balls (the user should have fewer Golden Balls than required).
5. Click "Enhance."

**Expected Result:** An error toast message should appear stating "Insufficient Golden Balls."

## Test Case 6: Use of Golden Balls
**Steps:**

1. Log in to the game.
2. Go to the Character (left panel) > Locker > Enhancement tab.
3. Attempt to enhance an item with a specified risk level (HIGH/MEDIUM).
4. Check the checkbox for using Golden Balls.
5. Verify if Golden Balls prevent the loss of bonuses in case of a failed enhancement.

**Expected Result:** The use of Golden Balls should prevent the loss of bonuses in case of a failed enhancement.

## Test Case 7: Enhancement to Higher Levels
**Steps:**

1. Log in to the game.
2. Go to the Character (left panel) > Locker > Enhancement tab.
3. Attempt to upgrade a gold item to Platinum level.
4. Attempt to upgrade a special platinum item to Diamond level.
5. Attempt to upgrade a gold item to Diamond level.

**Expected Result:** Upgrading gold items to Platinum level and special platinum items to Diamond level should be possible. Upgrading gold items to Diamond level should be impossible.

## Test Case 8: Enhancement on Two Open Tabs
**Steps:**

1. Log in to the game.
2. Go to the Character (left panel) > Locker > Enhancement tab.
3. Select an item for enhancement.
4. Duplicate the tab.
5. Enhance the item on both open tabs.

**Expected Result:** Two enhancement actions should be executed, one after the other. It should be impossible to enhance on the

## Test Case 9: Enhancement Using Special Balls
**Steps:**

1. Log in to the game.
2. Go to the Character (left panel) > Locker > Enhancement tab.
3. Select an item.
4. Use a special ball.
5. Click "Enhance."

**Expected Result:** Using a special ball should increase the enhancement chance.