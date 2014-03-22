Planning Calendar - Full-sized drag & drop planning calendar
====================================================

Rather than keeping track of an exact time of an event, this is a general planning calendar for major deliveries. This calendar includes the ability to place events into buckets (For example: Front page, Sports, Business). In addition, you will be able to drag events onto the calendar from an unscheduled list.

Getting Set Up to contribute to Project
--------------

You will need [Git][git], [Node][node], and NPM installed. For clarification, please view the [jQuery readme][jq-readme], which requires a similar setup.

Also, you will need the [grunt-cli][grunt-cli] and [bower][bower] packages installed globally (`-g`) on your system:

	npm install -g grunt-cli bower

Then, clone FullCalendar's git repo:

	git clone git://github.com/samfromashburn/planningcalendar.git

Enter the directory and install FullCalendar's development dependencies:

	cd planningcalendar && npm install


Development Workflow
--------------------

After you make code changes, you'll want to compile the JS/CSS so that it can be previewed from the tests and demos. You can either manually rebuild each time you make a change:

	grunt dev

Or, you can run a script that automatically rebuilds whenever you save a source file:

	./build/watch

You can optionally add the `--sourceMap` flag to output source maps for debugging.

When you are finished, run the following command to write the distributable files into the `./build/out/` and `./build/dist/` directories:

	grunt

If you want to clean up the generated files, run:

	grunt clean


Writing Tests
-------------

When fixing a bug or writing a feature, please make a corresponding HTML file in the `./tests/` directory to visually demonstrate your work. If the test requires user intervention to prove its point, please write instructions for the user to follow. Explore the existing tests for more info.
