# Triggers

* Standard Trigger Syntax

```java
trigger TriggerName on ObjectName (trigger_events) { code_block
}
```
* The following are the trigger events
	* before insert 
	* before update 
	* before delete 
	* after insert
	* after update
	* after delete
	* after undelete

* Use **addError(errorMessage)** on the Trigger object lists to add an error


| Trigger Context                Trigger.new       Trigger.newMap    Trigger.Old     Trigger.OldMap  |
|----------------------------------------------------------------------------------------------------|
|                                                                                                    |
| Before Insert                     Yes                    No          No                       No   |
|                                                                                                    |
| Before Update                     Yes                    Yes        Yes                     Yes    |
|                                                                                                    |
| Before delete                     Yes                    Yes        Yes                      Yes   |
|                                                                                                    |
| After Insert                      Yes                    Yes        No                        No   |
|                                                                                                    |
| After Update                      Yes                    Yes        Yes                        Yes |
|                                                                                                    |
| After Delete                      No                     No         Yes                        No  |
|                                                                                                    |
| After Undelete                    Yes                    Yes        No                        No   |

