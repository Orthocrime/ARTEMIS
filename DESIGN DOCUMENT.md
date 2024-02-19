- Expected features and functionality before moving to 0600
  - should have a button that saves the table in the detailed view to clipboard with table formatting intact
  - should make the sum of highlighted cells selectable for copying
    - it is desirable for user to edit a cell in a way that allows to create as many or as little units of numerical values within the single cell as needed while retaining the summation function;
  - should further test whether loading a new excel file actually purges the dataframe and sets the new source as editable from the dataframe / DOESN'T WORK at 0550 
  - should make `\` automatically break line;
  - should have some form of backup creation for rollbacks
    - suggestion:
      possibly the source file should be copied once the program is run, deleted if no edits made upon program termination
      the backup file should be retained for a number days and deleted when program is run after the set day count is up
      the user should be able to replace the source file with back up file if so chosen in a context menu (??)

- moved to a future 06xx build
  - should be able to distinguish between general database view and a search bar view which only shows results for queried phrases or numbers
  - should be able to retain past database iterations for rollbacks
  - should have user account system for accountability logging
  - should be able to retain formatting from source excel file
  - search bar should only appear when an excel file is imported
  - search bar should a have a cursor indicating whether it has been clicked and is ready for user input

- already implemented ahead of schedule:
  - should be able to show what values are summed from data located in cells that have more than one numerical value in them upon data clean up; implemented in 0550
  - general redundancy check-up; minor decluttering done in 0550
  - should further test whether edit function in the program can actually create more than one numerical value within a cell or can is able only edit the values (the precise number of value units) present at the        moment of excel file import / DOESN'T WORK at 0550 / WORKS AS OF 0554
  - should allow to create new rows / SINCE 0554 /also fixed the problem with adding new columns, can also add new sheets;
  - should make each row higher and each column narrower for more compact look;
    all contents up to a character count should be fully visible in the dataframe / each cell size is adjustable within UI and made fit to size with double clicking / 0554
  - should be able to discard any decimals that are either equal to 0 or would round down to less than .01; implemented in 0550

- specific future xxxxLAD fork
  - Works only with one specific excel file
  - based upon login information provided by the user (not saved in the app) within the program (this should check what browser user has set as default and use that; should also check whether these webpages have saved login information and try to use it automatically, if it doesn't or the saved login doesn't work, the user should be queried)
      - can populate a specific row within a column with DVS search results relevant to the case contained within the row
      - can update numerical values contained in specific columns based on results from a tab in IAKS
