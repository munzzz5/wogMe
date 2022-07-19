# wogMe
 *This is a daily logger that completely invades your privacy by telling you the truth about yourself that you didnt want to hear.*
## Functionality Assumed:
 - Connect user Google account
 - Get Chrome History
 - Get Time slots or use API if google calender account created
 - Implement Visualisations mentioned below
 
### Perceived Pseudo
```
reminders=reminderModel.get_all_reminders():
reminders.sort(by=scheduledTime)
timePeriods=[(i.scheduledTime,(i+1).scheduledTime) for i in reminders]

googleHistory=chrome.user.getTodaysHistory(from 12 am to next day 11:59 am)
userActivity={'Activity':[],'TimeSlot:[]}
for startTime,endTime in timePeriods:
  userActivity['Activity'].add(googleHistory.getHistoryByTime(startTime,endTime))
  userActivity['TimeSlot'].add((startTime,endTime))


# show visual for usage during task time
# show wordcloud for searches titles
# show Titles of activity using summarization tools
```


          
          
  
