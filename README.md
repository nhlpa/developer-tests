# NHLPA Developer Test

This repo contains a tab-delimited file of game results for an entire regulation season called `team_stats.txt`. The object is to parse and aggregate the results of this file.

Solutions are welcome in whatever programming language you are most comfortable with, though preferred in either C#, F# or PowerShell.

## Objectives


1. Programmatically download the file from GitHub.
2. Parse results and aggregate to produce a single object per team.
    - Note: The scoring system is shown below.
3. Output results for the following:     
    - Teams in descending order by **total points**.
    - Top 5 teams by **goal differential**.
    - Top 5 teams by **shooting percentage**.

> For the purpose of this task a simple, naive download and `System.Console` output is perfectly acceptable.

## Scoring System 

| Outcome | Points |
|---|---|
| Regulation win | 2 |
| Overtime loss | 1 |
| Loss | 0 |

> Overtime is defined as any game which *exceeds 3 periods*.

## Formulas

`Goal Differential = Goals For - Goals Against`

`Shooting Percentage = Goals For / Shots For`
