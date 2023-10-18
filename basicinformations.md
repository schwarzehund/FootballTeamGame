# Gather basic informations about the "Enchantment" module.

Informations about how it works can be found in [FAQ](https://en.footballteamgame.com/faq/1/39)

Based on those informations I've created a component description: 
>The Enhancement function allows users to strengthen the skill bonuses of items they possess in the game. The strength of the bonus depends on the rarity of the item, and there is a risk of failure during the enhancement process. Using Golden Balls can prevent the loss of bonuses in case of failure.

## INPUT PARAMETERS 

1. Access to a web browser and logging into the game
2. Items
```
   1. # common
   2. blue - enhanced
   3. green - rare
   4. red - epic
   5. gold - legendary
   6. platinum
   7. diamond
   8. historical
   ```
3. Golden Balls
4. Currency - Euro 

## ACCEPTANCE CRITERIA

1. Users can access the Enhancement feature in the **Character> Locker tab**.

2. Enhancement is possible for **green, red, gold, platinum, diamond, and historical** items.

3. The chance of a failed enhancement attempt is correctly marked as **HIGH/MEDIUM/LOW**, depending on the rarity of the item.

4. The **risk** of lowering the item's level in case of a failed enhancement is correctly marked as **HIGH/MEDIUM/LOW**, depending on the rarity of the item.

5. Using **Golden Balls** can **prevent the loss of bonuses** in case of a failed enhancement.

6. **Gold items** can be upgraded to **Platinum leve**l, and special **platinum items** (eg. leg pads, balls, and bands) can be upgraded to **Diamond level**.

7. Upgrading a **Gold** item to **Diamond level** (raising it by two levels) **is not possible**.

Based on those Acceptance Criteria I created [Test Cases](TestCases.md) and [API_TestCases](API_TestCases.md)
