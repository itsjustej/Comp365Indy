# Labeling conventions (play_dataset_v1.csv)
Roster (fictional): Marcus #7, Jaylen #4 (Jay, J-Money), Devon #12 (Dev), Tasha #9 (Tash), Riley #2 (Ri), Sam #15 (Sammy).
- play_type: pass | run | penalty | no_play (timeouts, period ends, anything with no play). no_play rows: all names empty, yards 0, result none.
- Pass: passer set (if named), receiver set if a target is named, runner empty. Thrown away / no target: receiver empty.
- Run: runner set; passer and receiver empty (a handoff giver is not recorded). QB scramble = run.
- Penalty: names empty. yards positive for defensive penalties, negative for offensive penalties. No yards stated = 0.
- yards: yards gained by the offense; negative for losses. Unstated yards = 0. Incomplete and interception = 0. A distance like "from the 30" or "on 3rd and 8" is not yards gained.
- result: complete | incomplete | interception | touchdown | none (runs and penalties without a score = none). Touchdown keeps the yards of the play.
- Player not on the roster: leave that name field empty.
- Two plays in one sentence: label only the final play described.
- Splits: dev (prompt examples only), test (written after prompt frozen), hard (stress cases by category).
