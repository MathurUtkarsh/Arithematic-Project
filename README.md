# Arithematic-Project

1. This Project is a partially built project on Simple Arithmetic Game for single player.
2. Most of the coding part is already done, however, some clues are left in between (comments //) where students can write their codes.
3. matchCounter will keep track of how many matches are played. A match is akin to answer one question.
4. If a player correctly answers a match, a one is added in the score array; otherwise, a zero will be added.
5. When matchCounter reaches a value 3, the sum of last three matches will be added to the performance array, which is initially set with -1 at all places. For example, the performance array at the start of your app will be like [-1, -1, -1, -1, -1, -1], but after the completion of three matches let the score array be like [1, 0, 1] then the performance array would be like [-1, -1, -1, -1, -1, 2]. Each time the performance array will be updated, the new value will be added at the last element of the array, and all previous values will be shifted one place left. The first value will be lost, as we have to analyze the performance of the last six games only.
6. The performance array will be stored in a SharedPreferences object. The SharedPreferences object is fetched at the start of the activity and an alert dialog is presented to the user suggesting on his or her performance based on the last six games.
7. sumOfScore method should summing up the values of score array.
8. A class LR is also provided with this project. The LR class has a getSlope method to provide the slope fromo the given data. The data must be input to the getSlope method as a two-dimensional array (dataFrame). The first dimension will be the predictor values 1, 2, 3, 4, 5, 6 and the corresponding response values will be performance values. The getSlope method is a static method, so you won't need to create objects of the LR class to obtain slope. Just use the name of the class LR. For example: LR.getSlope(dataFrame) would return a slope as a double value.
9. dataPrep method generates a data-frame AKA two-dimensional array to be passed to the getSlope method.
10. getInterpretation method returns a string based on the analysis of slope obtained from analysis of past six
