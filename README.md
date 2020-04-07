# AAE_Notebook_022_TrackStateChanges
Now that we understand the system, we're going to test that understanding by implementing a way to track the changes of states over time.

In glancing at the ```advance_state_uncontrolled(self, dt)``` (tracking the state of a monorotor in free-fall), we better notice the correlations between z, z_dot, and z_dot_dot (wherein z_dot_dot is simply the acceleration due to gravity -- 9.81 m/s^2).

Using this, we can now implement an ```advance_state(self, )``` to track changes of state over time for our monorotor.
