# ASCOM-safety-monitor-via-text-file
A simple ASCOM Safety driver deriving its status from a file source:

It was designed to work with my observatory controller, roll-off-roof ASCOM driver and Arduino control system.
The Arduino controller has its own sensitive rain sensor and broadcasts its status over serial line.
The observatory controller reads this status and updates a file   ...//documents/ASCOM/obsy/safety.txt  if the rain sensor status changes.
The simple "safe" or "unsafe" text in the file is read by this ASCOM driver in response to a status request.
I combine this and other safety devices into a more complete safety status using an ASCOM hub written by dehilster.
