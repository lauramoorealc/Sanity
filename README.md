Sanity Check - Setpoint Adjust Solution
============

Modify Sanity Check so that it lists any Location where the Heating or Cooling Setpoint has been adjusted by an occupant.
```
Heating Floor 09 * / HVAC / Conference *	1.0
Cooling Floor 09 * / HVAC / Conference *	1.0
```

Step 1.  Explore the API
1. What version of the API does this project build with?
2. What access aspects are defined in this version? [Hint](http://alcshare.com/contentprotector/files/sdk/ver1.0.8/javadoc/index.html)

Step 2. Modify NamedFloatValueAcceptor
Change the NamedFloatValueAcceptor to accept SetpointAdjust instead of PresentValue
* where else do you need to change so the code builds and deploys?

Deploy and Test
* Adjust a Setpoint at location #floor09_hvac_conference/setpt
* What Display name do you need to match to find this changed setpoint?
* Did you see results?

Troubleshooting
* Add a System.out.println statement in the NamedFloatValueAcceptor
* What locations are being matched by the Aspect?
* How does the Physical Point Enabled check in the Acceptor interact with SetpointAdjust?









