1. Your GitHub repository link (Step 3).
https://github.com/kianacalylcompra/kianas_project.git

2. The last three build() called lines from Activity 2.
build() called: 4 glasses
build() called: 5 glasses
build() called: 6 glasses

3. Your observations from the experiments in Activities 2, 3 and 5.
ACTIVITY 2 
- When I tapped + without 'setState()', nothing changed on the screen because Flutter was not told to update it.

ACTIVITY 3 
- Without Expanded, the StatBox becomes too small, and the code gets syntax errors if missing its wrapper.

ACTIVITY 5
- The button corners became much rounder after changing the radius in buildTheme().

4. Your answers to the ten review questions.

1. What is the difference between a StatelessWidget and a StatefulWidget? Give one example of each from this lab.
- A StatelessWidget cannot change once it shows on the screen, but a StatefulWidget can change its data and update while the app is running. In this lab, ProfileCard is an example of StatelessWidget, and WaterTracker is an example of StatefulWidget.

2. Why is a StatefulWidget written as two classes? What does each class do?
- A StatefulWidget is written as two classes to keep settings separate from changing data. The first class sets up the widget, and the second class holds the data and updates the screen when things change.

3. In Activity 2, what happened when you changed _glasses outside setState()? Why?
- The glasses count stayed at 0 on the screen when I tapped +, because without 'setState()' Flutter was not told to update the screen.

4. Looking at the Debug Console in Activity 2, when is build() called?
- build() runs when the app starts. It also runs every time setState() is used. That is every time I tap +, − or Reset.

5. Explain the main axis and the cross axis of a Row and of a Column.
- For a Row, the main axis goes left-to-right, and the cross axis goes up-and-down. For a Column, the main axis goes top-to-bottom, and the cross axis goes left-to-right.

6. In Activity 3, what happened when you removed Expanded from a StatBox? What does Expanded do?
- When Expanded was removed, the box became small and the four boxes were no longer the same size. The Expanded widget forces a widget to use all the remaining space, which is why the boxes were equal before.

7. Why do we use GridView.builder for the menu instead of a Column with many children?
- GridView.builder only makes the items I can see on the screen, this is faster. A Column makes all the items at the same time.

8. How do Stack and Positioned create the Best seller badge in Activity 4?
- Stack places widgets on top of each other like layers. Positioned moves the badge layer to an exact spot, like the top corner of an image.

9. What is the difference between customizing with ThemeData and with a style on one widget? Give one example of each from Activity 5.
- ThemeData changes the whole app. Example: elevatedButtonTheme changes all ElevatedButtons. A style on one widget changes only that widget. Example: the TextStyle on one Text.

10. When you flip the dark-mode switch in Activity 5, which widget holds the state, and how does the change reach MaterialApp?
- _ThemeDemoAppState keeps the state _isDark. When I flip the switch, it runs _setDark. This changes _isDark with setState(). Then MaterialApp picks the dark theme or the light theme using themeMode. So the whole app changes.
