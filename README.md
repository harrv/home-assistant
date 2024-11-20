# Home Assistant Automations

I'm currently working on a to-do list utility automation blueprint that gives
you the option of doing any of the following. I'll make it available soon.

- Normalize task names
  - trim leading and trailing whitespace
  - reduce inner contiguous whitespace to a single space
  - apply a case rule
    - sentence case (Take out trash)
    - title case (Take Out Trash)
    - lowercase (take out trash)
    - uppercase (TAKE OUT TRASH)
- If multiple tasks have the same name, remove all but one
  - one that remains will have `status` = `needs_action` if _any_ of the
    duplicates did
- Sort tasks
  - by task name
  - by due date
  - by description (useful if you begin that field with an alphabetical priorty
    scheme)
- Strip due dates from all tasks
- Strip descriptions from all tasks
- Remove completed tasks
- Remove all tasks (leaving an empty to-do list)
- Do a "dry run" without making modifications so you can see what _would_ happen
- Optional system logging

[//]: # (
SPDX-FileCopyrightText: © 2024 Stephen Harvey Trottier
SPDX-License-Identifier: MIT
)
