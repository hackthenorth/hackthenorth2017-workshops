# Android 2 Workshop

Android Lifecycle 
- onCreate() - activity created, all the normal setup happens (views, data population), Bundle from activity’s previously frozen state is obtained, followed by onStart()
- onRestart() - if activity stopped and started again
- onStart() - activity is visible to user 
- onResume() - activity is interacting with user, activity is at the top of the activity stack
- onPause() - activity is in background, but not killed 
- onStop() - activity no longer visible to user, next is either onRestart() or onDestroy()
- onDestroy() - last call before activity is destroyed 
Opening another activity
- Create a new intent with the class of the activity that you want to go to 
- Call startActivity(intent) to push the user to the new activity
- To carry any data over to the new activity from the old one, put it in a Bundle and add it to the intent 
  - `intent.putExtras(“key”, “value”);`
- In the new activity, call getIntent().getExtras() to get the Bundle with the information and parse the data you passed 
