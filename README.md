# Objective

From a master English word list, filter to only keep words that:

* Are exactly 5 characters long.
* All characters are lower-case.  This eliminates people and place names that wouldn't be considered in a game such as **wordle**.

The master word file was copied from a **[gist file](https://gist.githubusercontent.com/sdao/12ccaf20722a61d401e2ff284b5a28a2/raw/ada848f737fb79fc4e1fbeac958cf520f6004d6e/words)**.

# Installation

This has been tested on an **iMac** running MacOS **Monterey**.  These instructions will largely work for **Linux**; on **Windows**, YMMV.

1. Clone this repo to your PureScript projects folder
    ```bash
    git clone https://github.com/oldfartdeveloper/wordle-generate-word-list.git
    ```
1. Follow the **[GitHub instructions](https://github.com/purescript/documentation/blob/master/guides/Getting-Started.md)**. There are simple examples of how to perform the most important PureScript development operations.
1. `cd` into the new repo's directory.
1. `spago build`.  It should build successfully

# Running the Application

To generate the text file containing the 5-letter words:

1. Be sure you are in the project directory.
1. Run `spago run`
1. Verify that the file has been generated as `doc/words.txt`.  It should have the current time stamp.

If you haven't already, clone and install the `wordle-solver` repo which will use this project's generated file.
