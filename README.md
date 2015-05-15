# Chess Timer

The ChessTimer class provides a timer which measures elapsed time on a
given task.  There is no limit to the number of tasks, but only one task
accumulates time at any given moment.

All times are in floating-point seconds.

Requires Python ≥ 3.3 because it uses time.monotonic().TODO: Write a project description

## Installation

Just download ChessTimer.py and include it in your project.

## Usage

    johnny = ChessTimer()
    johnny.switch_to('A')

    ...

    johnny.switch_to('B')

    ...

    johnny.switch_to('A')

    ...

    johnny.switch_to(7)

    ...

    johnny.switch_to(None)
    print(johnny.all_elapsed_time(reset=True))
      # e.g. {'A': 2.14158, 'B': 0.33546, 7: 1.25665}

    print(johnny.all_elapsed_time())
      # {}
