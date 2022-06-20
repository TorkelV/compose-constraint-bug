If a FragmentContainerView contains only a ComposeView and is constrained to a toolbar with layout_height=0dp and layout_constraintHeight_min="60dp" , the ComposeView behaves like the toolbar is always 0dp, even though the actual size is 60dp. The ComposeView is still constrained to the toolbar, but its height will be +60dp and draw below the screen.
The layout works fine if I add a height to the toolbar instead of using app:layout_constraintHeight_min.

See [activity_main.xml](app/src/main/res/layout/activity_main.xml)

![screenshot](https://i.ibb.co/hfNB3w2/Screen-Recording-2022-06-20-at-08-47-47.gif)

