# Test Component Report "Enhancement"

## General Information

|Title|Value|
|-----|-----|
Report Generation Date: |29.09.2023
Application Name: |Football Team Game
Version: |1.29
Env| https://en.footballteamgame.com/
Objective:| Testing the Enhancement Component



*All information was found in the [FAQ](https://en.footballteamgame.com/faq/1/33).* 

I relied on them to create this documentation. Initially, I had a problem with the fact that in the Character -> Locker -> Enhancements section, there are only three categories of items, while in the FAQ, there were many more. I assumed that all items rarer than red fit into the last category (golden).

## Test Case Development
Based on the gathered information and analytical thinking, I created test cases to check the fundamental functions of Enhancement, which are available here:
[Google Docs Link](https://docs.google.com/document/d/1-r62fWgcUO5aM_QHMnEO3a_7GdVIhQ9AB2UW7sf_8p8/edit)

## Test Execution
I performed a series of enhancements on various items with different risks and success rates. I didn't find any errors, whether it was different screen resolutions or with throttling enabled.
The first tab in the link:
[Google Docs Link](https://docs.google.com/document/d/1-r62fWgcUO5aM_QHMnEO3a_7GdVIhQ9AB2UW7sf_8p8/edit)

## Bug Collection
I found one bug, and it wasn't related to the component itself.

## Summary
### Component Status
The component seems to be foolproof in its operation. There are no inputs that a user could use to insert strange values, and the principle of "Enhancement" is simple. I didn't encounter any issues with the functioning of this component given the items assigned to me. Where I see potential problems that could emerge with more attempts is the incorrect result of expected success chances and risk levels. A potential problem could be a too high frequency of enhancement failures or an item with a high risk of degradation not being downgraded adequately.

Also, from the back-end perspective, the component appears to be well-made, as indicated by the quality of responses to the executed requests.

### Strategies:

#### Automated Testing:
 To save time, consider automating the simplest cases, such as checking the availability of the Enhancement options, the possibility of Enhancements in various configurations, and those on the edge with the rarest items in the game.

#### Regression Testing: 
To ensure that new updates do not have an undesirable impact on this component, pay special attention to code changes related to items, euros, Golden Balls, and Special Balls.
#### Manual Testing: 
To replicate user interactions and assess UX and overall navigation through the application.
#### Exploratory Testing: 
To discover new unexpected errors, use different devices, time zones, and open and perform actions in two different windows.
### Tools:
To create this report and conduct tests, I used:

- **Google Chrome** and built-in dev tools for inspecting the site in terms of HTML and CSS and network, for browsing requests,
- **Postman** for sending requests to the endpoint,
- **Miro**,
- **Google Sheets and Docs**.