# Work shift scheduler

This is my final project for the [Building AI course](https://buildingai.elementsofai.com). The idea is a work shift scheduler for automating the creation of work shift schedules.

## Summary

The scheduler will create alternative versions of possible work shift schedules based on the collective labour agreement, the applicable labour legislation, and the individual preferences of the employees. You can create the schedule for a week or for a whole month, or longer if needed.

## Background

Drafting and creating work shift schedules in any field where the work is done in shifts - e.g. retail, health care, manufacturing - is time and labour consuming and often results in compromise schedules where no one is really happy with the shifts they're assigned. It usually takes the labour input of one entire employee just to create the schedule. The work shift scheduler automates this task and produces alternative versions of possible schedules, of which the employee in charge of shift scheduling can then choose the best one.

## How is it used?

In fields where the work is done in shifts, the terms of the collective labour agreement of the field and the applicable labour legislation of the country determine the boundary conditions for the shifts:
* on how many successive days can an employee work before they need to have a day off
* how many morning, day, or night shifts can one employee have in succession, and how many days off do they need to have afterwards
* public holidays
* how many employees are needed fora a shift
* when does a shift start or end

In addition, the employees have individual preferences that need to be taken into account:
* requested days off
* preference for morning/day/night shifts

## Data sources and AI methods

The scheduler uses the terms of the collective labour agreement of the given field, the applicable labour legislation of the country, and the individual preferences of the employees as data, using supervised machine learning.

## Challenges

The scheduler will not determine what is the best work schedule - it only produces alternatives which are possible given the conditions. The employee in charge of shift scheduling must choose the most appropriate one and tweak it if needed. (Of course, if there are many restricting conditions, there might be only one possible solution - or none.) Executing the idea requires consulting a labour legislation or HR professional. Considering the multitude of different kinds of labour agreements, it would be best to start with the labour terms and conditions of only one field and try to get that to work before venturing onto others.
