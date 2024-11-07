# modelingThis state machine controls the behavior of a traffic light system, cycling through three states: Green, Yellow, and Red. Each state transition is triggered by a timer, simulating a timed traffic light sequence commonly used in road intersections.

States and Transitions
Initial State:

Green: The traffic light starts in the Green state, allowing vehicles to proceed.
State Transitions:

Green to Yellow:

Trigger: Timer expires (e.g., 30 seconds).
Action: The light changes from Green to Yellow, signaling caution as the light will soon turn Red.
Yellow to Red:

Trigger: Timer expires (e.g., 5 seconds).
Action: The light changes from Yellow to Red, indicating vehicles must stop.
Red to Green:

Trigger: Timer expires (e.g., 30 seconds).
Action: The light changes from Red back to Green, allowing vehicles to proceed once again.
Timers:

Each transition is controlled by a specific timer:
Green to Yellow Timer: Determines how long the light remains Green before changing to Yellow.
Yellow to Red Timer: Sets the duration for which the light stays Yellow.
Red to Green Timer: Controls the duration for which the light remains Red before turning back to Green.
State Diagram
plaintext
Copy code
[*] --> Green
Green --> Yellow : Timer Expires
Yellow --> Red : Timer Expires
Red --> Green : Timer Expires
