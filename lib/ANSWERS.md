1. Your GitHub repository link (Step 3).
https://github.com/kianacalylcompra/kianas_project.git

2. The last three build() called lines from Activity 2.
build() called: 4 glasses
build() called: 5 glasses
build() called: 6 glasses

3. Your observations from the experiments in Activities 2, 3 and 5.
ACTIVITY 2 
  // Dart requires a semicolon (;) at the end of statements like _glasses++.
  // Without it, the code causes a syntax error and fails to compile.

ACTIVITY 3 
    // Without Expanded, the StatBox becomes too small,
    // and the code gets syntax errors if missing its wrapper.

ACTIVITY 5
    // The button corners became much rounder after changing the radius in buildTheme().

4. Your answers to the ten review questions.

1. What is the difference between a StatelessWidget and a StatefulWidget? Give one example of each from this lab.
- A StatelessWidget cannot change once it shows on the screen, but a StatefulWidget can change its data and update while the app is running. In this lab, ProfileCard is an example of StatelessWidget, and WaterTracker is an example of StatefulWidget.

2. Why is a StatefulWidget written as two classes? What does each class do?
- A StatefulWidget is written as two classes to keep settings separate from changing data. The first class sets up the widget, and the second class holds the data and updates the screen when things change.

3. In Activity 2, what happened when you changed _glasses outside setState()? Why?
4. Looking at the Debug Console in Activity 2, when is build() called?
5. Explain the main axis and the cross axis of a Row and of a Column.
6. In Activity 3, what happened when you removed Expanded from a StatBox? What does Expanded do?
7. Why do we use GridView.builder for the menu instead of a Column with many children?
8. How do Stack and Positioned create the Best seller badge in Activity 4?
9. What is the difference between customizing with ThemeData and with a style on one widget? Give
one example of each from Activity 5.
10. When you flip the dark-mode switch in Activity 5, which widget holds the state, and how does the
change reach MaterialApp?