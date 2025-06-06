# soundboard
SoundBoard – Collaborative Jam Session Recorder
Scenario
Remote musicians want a simple way to record audio loops, layer tracks, and create collaborative jams without complex DAWs.

🎯 Objective
Build a web app where users create “Jam Rooms,” record short audio loops, share them with collaborators, and mix multiple tracks into a final export.

👤 User Role: user
All users can host or join Jam Rooms.

🔐 Auth & Authorization
Login required to record or join sessions
Only invited users can access a private session; host can toggle public
🧱 Core Modules
Jam Room Management
Host creates room with title, BPM, key signature, room code/link
Loop Recording
Web Audio API: record up to 30 sec loops
Save loop with track name and order index
Track Mixer
List of recorded loops per room
Enable/disable individual loops and adjust volume sliders
Collaborative Sync
Poll for new loops every 5 sec; display in UI without reload
Timestamped per user
Export Mixdown
Combine active loops into single downloadable audio file (client-side render or mocked)
Profile Analytics
On each user’s profile, show aggregated stats across all rooms:
Total Jam Rooms hosted
Total loops recorded
Total mixdown exports
Average loops per session
