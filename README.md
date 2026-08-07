# Date & Time Utility Library + Event Scheduler

A hand-built date/time engine and event scheduler in modern C++ — leap-year-safe
arithmetic, live conflict detection, and self-healing schedules that clean up
after themselves. Built from scratch without relying on `<chrono>` shortcuts,
covering everything a real calendar app handles internally: validating dates,
comparing and adding to them correctly across month and year boundaries, and
using that foundation to power a scheduler with conflict detection and file
persistence.

## Clone and run

1. Clone the repo:
```bash
   git clone https://github.com/KTejash/Date-and-Time---Event-Scheduler.git
```

2. Move into the project folder (the actual source files live inside
   `DateTimeScheduler`, not the repo root):
```bash
   cd Date-and-Time---Event-Scheduler/DateTimeScheduler
```

3. Open it in VS Code:
```bash
   code .
```

4. Build it — press `Ctrl+Shift+B` (`Cmd+Shift+B` on Mac). This runs the
   pre-configured build task and produces a `scheduler` executable
   (`scheduler.exe` on Windows).

   Or skip VS Code entirely and build by hand in any terminal:
```bash
   g++ -std=c++17 -Wall -o scheduler main.cpp DateTime.cpp Event.cpp Scheduler.cpp
```

5. Run it:
```bash
   ./scheduler        # Mac/Linux
   scheduler.exe       # Windows
```

6. First thing to try: pick option `8` from the menu to run the self-tests
   — this confirms the leap-year and date-arithmetic logic is working
   correctly before you start adding events.

**Note:** once you save a schedule, it writes a `schedule.csv` file into
this same folder. That file is gitignored on purpose — it's your local
test data, not part of the source code.

## To add it: open README.md in VS Code, paste this in, save, then:
bashgit add README.md
git commit -m "Add clone and run instructions"
git push


# it's a -
C++ date/time utility library + event scheduler with conflict detection, leap-year handling, and file persistence.
#cpp
#event-scheduler "date-time" 
#college-project
#Cipher-School


