# Nearfield scenario map: moveit2

Date: 2026-06-05

This fork-local note records how moveit2 can inform Nearfield's robot readiness evaluation work. It is a project-specific research note, not an upstream authorship claim and not a request to merge changes upstream.

## Relevance

moveit2 is relevant to readiness evaluation because it touches motion planning, manipulation execution, collision checking, and task-space constraints. Nearfield uses this kind of open-source stack review to identify where deployment evidence can be captured before a robot is trusted in shared human spaces.

## Evaluation hooks

- planning success/failure reasons
- trajectory smoothness and clearance scoring
- execution deviation against planned path

## Scenario candidates

- service handoff pose selection
- tabletop reachability under human proximity constraints
- manipulation plan comparison across scene layouts

## Nearfield use

For Nearfield, the important question is not whether a robot succeeds once. The useful signal is whether a scenario can be replayed, scored, compared, and turned into evidence that operators can inspect. This repository helps map one part of that evidence pipeline.
