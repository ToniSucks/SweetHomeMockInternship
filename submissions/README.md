# Acceptance evidence

Verified on Windows with JDK 11.

- `task1-running.jpg`: the application running with the supplied sample.
- `task2-description.jpg`: an edited Description in Modify furniture. Confirmed the text persists after OK and reopening the dialog.
- `task3-volume.jpg`: populated Volume column and Furniture > Sort by > Volume.
- `task3-context-menu.jpg`: Volume in the table's Display column context submenu. Verified ascending and descending sorting.
- `task4-all-levels.jpg`: print preview Page 1/4, showing furniture from Levels 0, 1, and 2 and a print-only Level column.
- `task4-level0.jpg`, `task4-level1.jpg`, `task4-level2.jpg`: the three plan pages in home level order.

Printing was started with Level 2 selected and Level hidden in the on-screen table. After preview, Level 2 remained selected and the on-screen table still had no Level column.

Validation: all six provided Maven tests and `python test_submission.py` pass. Additional checks covered description undo/redo, catalog volume, volume after resizing, ascending/descending sorting, CSV export, hidden-level exclusion, and selected-level/table-column restoration after simulated render/print failures. The provided `assignment-tests` were not edited.

Feature commits reference GitHub issues #1 (Task 2), #2 (Task 3), and #3 (Task 4).
