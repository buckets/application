<!-- THIS FILE IS AUTOMATICALLY UPDATED. SEE THE README -->
## v0.54.0 - 2019-02-28

- **NEW:** Removed Beta preference (since there's now a separate Buckets Beta application)

- **NEW:** Your email address is remembered when you report a bug (so you don't have to enter each time you report a bug).

## v0.53.1 - 2018-12-13

- **FIX:** Fix erroneous SignMismatch error ([#323](https://github.com/buckets/application/issues/323))

## v0.53.0 - 2018-12-12

- **NEW:** Accounts and balances can now optionally be shown in the side bar if you want.  Use the per-budget settings page to toggle.  ([#99](https://github.com/buckets/application/issues/99))

- **NEW:** Total Want is now shown for each bucket group.  ([#274](https://github.com/buckets/application/issues/274))

- **NEW:** This change might annoy you at first, but once you get used to it, you'll like it :)  When entering transactions, the amount now defaults to a **negative** amount since most transactions are expenses.  You can enter positive amounts by clicking the big *minus* button or by entering a negative number.  ([#307](https://github.com/buckets/application/issues/307))

- **NEW:** Money inputs now stay the same width even when doing math inside of them.  Computed values are displayed in a floating tag above the input rather than to the side.

- **FIX:** Fix CSV import error when CSV contains blank header cells.  ([#316](https://github.com/buckets/application/issues/316))

- **FIX:** Top bar expenses are no longer red so that red is reserved for problem-like situations.  ([#291](https://github.com/buckets/application/issues/291))

- **FIX:** Clicking account names now opens up the account details rather than editing the account name.  You can still edit account names by clicking on the name in the details pane.  ([#244](https://github.com/buckets/application/issues/244))

- **FIX:** When importing from YNAB4, you can choose the YNAB4 file or as a convenience to users, any file inside it ([#318](https://github.com/buckets/application/issues/318))

## v0.52.1 - 2018-11-26

- **FIX:** Fixed a bug where calculator wouldn't work if you had whitespace ([#313](https://github.com/buckets/application/issues/313))

- **FIX:** Dutch translation corrections

- **FIX:** French translation corrections

## v0.52.0 - 2018-09-17

- **FIX:** Attempted fix at unreproducible account deletion error. ([#301](https://github.com/buckets/application/issues/301))

- **FIX:** Attempted fix of goal date inconsistency ([#288](https://github.com/buckets/application/issues/288))

- **FIX:** Errors related to entering licenses are better logged now.  ([#229](https://github.com/buckets/application/issues/229))

- **FIX:** OFX files with multiple accounts inside can now be imported. ([#302](https://github.com/buckets/application/issues/302))

- **FIX:** Make sure newly-created budget files end with the correct extension. ([#304](https://github.com/buckets/application/issues/304))

- **FIX:** Fixed bug where tooltip would flicker at the edge of the screenstatus ([#299](https://github.com/buckets/application/issues/299))

- More internal refactoring for mobile apps.

## v0.51.1 - 2018-08-08

- **FIX:** Pressing Enter while editing bucket details will close the details. ([#235](https://github.com/buckets/application/issues/235))

- **FIX:** Fix false warning about using an older version of buckets on a newer budget file. ([#280](https://github.com/buckets/application/issues/280))

- **FIX:** You can now import transactions for off-budget accounts. ([#284](https://github.com/buckets/application/issues/284))

## v0.51.0 - 2018-08-06

- **NEW:** Added some Net Wealth charts ([#171](https://github.com/buckets/application/issues/171))

- **NEW:** When transactions are created for a month other than the one you're looking at, a notification will pop up to let you know that it was successfully created.  ([#283](https://github.com/buckets/application/issues/283))

- **NEW:** Added shortcut keys for going to next and previous month.  Also included them in the Budget, Go To... menu. ([#266](https://github.com/buckets/application/issues/266))

- **NEW:** Using an old version of Buckets to open a newer budget file displays a warning now.  ([#280](https://github.com/buckets/application/issues/280))

- **FIX:** Restored Buckets License bucket for the trial version.  It accidentally got removed a few versions back.

- **FIX:** Fixed a bug so that now, when you change a transaction's date to another month, the transaction will disappear from the current month as it should.  ([#275](https://github.com/buckets/application/issues/275))

- **FIX:** Fixed bug where Linux Beta installations would offer to downgrade to latest non-beta version.  ([#279](https://github.com/buckets/application/issues/279))

- **FIX:** Fewer characters are swallowed when searching on the page. ([#270](https://github.com/buckets/application/issues/270))

## v0.50.0 - 2018-07-30

- **NEW:** Paying off credit cards and some other debt is now easier with the addition of Debt accounts.  ([#277](https://github.com/buckets/application/issues/277))

- More internal refactoring to prepare for mobile apps

## v0.49.0 - 2018-07-16

- **FIX:** Added DD/MMM/YY as date format for CSV importing.  Also made it so you can type in whatever format you want. ([#263](https://github.com/buckets/application/issues/263))

- **FIX:** Fixed a bug that would clear a transaction's income/transfer designation if you changed the amount. ([#265](https://github.com/buckets/application/issues/265))

## v0.48.0 - 2018-07-09

- **NEW:** You can now kick buckets right from the buckets list view. ([#225](https://github.com/buckets/application/issues/225))

- **FIX:** Possible duplicate transaction detection is now limited to transactions that have nearby dates and is expanded to look for transactions in adjacent months.  ([#261](https://github.com/buckets/application/issues/261))

## v0.47.0 - 2018-07-02

- **NEW:** Added a calculator for doing quick calculations.  ([#255](https://github.com/buckets/application/issues/255))

- **NEW:** You can now see the cleared balance and uncleared total on individual accounts.  ([#194](https://github.com/buckets/application/issues/194))

- **NEW:** You can now dismiss notifications if they are covering up some things you want to see.  ([#223](https://github.com/buckets/application/issues/223))

- **NEW:** Pressing escape while focused on the Buckets In/Out field will clear the selected field now.  ([#241](https://github.com/buckets/application/issues/241))

- **NEW:** Added a new 'Go To This Month' menu option and shortcut key.  ([#246](https://github.com/buckets/application/issues/246))

- **NEW:** Individual account views now include the amount in/out for that account for the current month.  ([#216](https://github.com/buckets/application/issues/216))

- **NEW:** Now available in Polski, thanks to Piotr Bielaska!

- **FIX:** Amazon reconciliation is much easier to use now.  ([#124](https://github.com/buckets/application/issues/124))

- **FIX:** Fixed bug where budget failed to load after error. ([#253](https://github.com/buckets/application/issues/253))

- **FIX:** Fixed the situation where sometimes the update available window would get covered up by the last opened budget window.  ([#177](https://github.com/buckets/application/issues/177))

- It's now a little more clear how (Budget Specific) Settings differ from (Application) Preferences.

- Clearly indicated to translators which instances of *Buckets* refers to the application rather than buckets within the program.  ([#173](https://github.com/buckets/application/issues/173))

## v0.46.2 - 2018-06-27

- **FIX:** Fix missing locale bug ([#252](https://github.com/buckets/application/issues/252))

## v0.46.1 - 2018-06-26

- **FIX:** Renamed bucket transaction "Misc" column to "Account" ([#245](https://github.com/buckets/application/issues/245))

- **FIX:** Fixed bug that prevented removing categories while editing a transaction ([#239](https://github.com/buckets/application/issues/239))

## v0.46.0 - 2018-06-25

- **NEW:** Now available in Deutsch!

- **FIX:** Added more verbose logging for Linux file read/write issues, including a message to instruct the user about how to possibly fix the problem. ([#224](https://github.com/buckets/application/issues/224))

- **FIX:** Override number format set in Preferences is now honored ([#237](https://github.com/buckets/application/issues/237))

- Massive code refactoring to get ready for the mobile app.

- Added a little more context for translators.  ([#234](https://github.com/buckets/application/issues/234))

## v0.45.0 - 2018-06-18

- **NEW:** Added a preference for getting Beta releases of Buckets.

- **FIX:** You can now negate values when importing from CSV files.  This allows you to handle banks that list both debits and credits as positive values.  ([#222](https://github.com/buckets/application/issues/222))

## v0.44.2 - 2018-06-04

- **NEW:** When you create a new account, the account's details are shown ([#176](https://github.com/buckets/application/issues/176))

- **FIX:** Fix the bug where a category is removed when editing a transaction in the account view.  ([#217](https://github.com/buckets/application/issues/217))

- **FIX:** Exclude off-budget accounts from analysis ending balance field.  Don't worry, there will be more reports later that include off-budget accounts :) ([#220](https://github.com/buckets/application/issues/220))

- **FIX:** [afcu.com-209 4cf27da] Fixed bank macro bug where a bank's short HTTP-only domain did not properly redirect to the full HTTPS domain.  ([#209](https://github.com/buckets/application/issues/209))
 1 file changed, 1 insertion(+), 1 deletion(-)

- **FIX:** You can now transfer to/from off-budget accounts when making transactions.  ([#213](https://github.com/buckets/application/issues/213))

- **FIX:** Prevent accidentally opening the same file twice (as with a double click) from the starting file-chooser pane ([#211](https://github.com/buckets/application/issues/211))

- **FIX:** You can now unlink accounts from import files so that the next time you import a file for that account, you will be prompted to choose which account the file belongs to.  ([#210](https://github.com/buckets/application/issues/210))

- Internal refactorings to get ready for mobile app

## v0.44.1 - 2018-05-25

- **FIX:** Fix analysis reports so that they no longer include off-budget accounts.  There will be other reports for off-budget accounts.  ([#206](https://github.com/buckets/application/issues/206))

- **FIX:** Handle non-unicode CSV files.  ([#202](https://github.com/buckets/application/issues/202))

- **FIX:** Potential fix for update error on start on Ubuntu ([#207](https://github.com/buckets/application/issues/207))

## v0.44.0 - 2018-05-10

- **NEW:** Buckets is now signed for macOS and Windows!  This means you shouldn't get as many warnings when trying to install it.  ([#150](https://github.com/buckets/application/issues/150))

- **FIX:** Indicate that you might have to download the new version manually ([#203](https://github.com/buckets/application/issues/203))

- Switched out sqlite for sqlite3-offline ([#183](https://github.com/buckets/application/issues/183))

## v0.43.1 - 2018-05-08

- **FIX:** Fix bug preventing the remapping of CSV files ([#199](https://github.com/buckets/application/issues/199))

- **FIX:** Fix for bug with CSV importing where numbers were multiplied by 100 because the chosen language's default number format was not honored. ([#200](https://github.com/buckets/application/issues/200))

## v0.43.0 - 2018-05-07

- **NEW:** You can now choose a currency symbol to be displayed with the top summary numbers.  Go to the new *Settings* tab (look on the bottom left corner) and type in your favorite symbol. ([#107](https://github.com/buckets/application/issues/107))

- **FIX:** Fixed alignment on Buckets table headings.  ([#193](https://github.com/buckets/application/issues/193))

- **FIX:** Fix CSV import bug ([#190](https://github.com/buckets/application/issues/190))

- **FIX:** Dates are properly formatted according to your chosen locale again.  ([#186](https://github.com/buckets/application/issues/186))

- **FIX:** "Save X by depositing Z/mo" buckets no longer keep wanting after the goal has been reached ([#192](https://github.com/buckets/application/issues/192))

- **FIX:** When launching from the command line, look for custom BUCKETS_LANG environment variable instead of LANG.

- **FIX:** Fix no-internet false positive error ([#195](https://github.com/buckets/application/issues/195))

- **FIX:** The Recurring Expenses month slider is no longer impossible to use ([#188](https://github.com/buckets/application/issues/188))

- **FIX:** Fix Starting over bug when you want to delete everything, including buckets ([#191](https://github.com/buckets/application/issues/191))

## v0.42.0 - 2018-04-30

- **NEW:** Transactions can now be marked as cleared or not. ([#172](https://github.com/buckets/application/issues/172))

- **NEW:** CSV importing supports CSVs where the postive/negative amount is broken out into a column separate from the amount.  ([#185](https://github.com/buckets/application/issues/185))

- **NEW:** Now translated into Nederlands!

- **FIX:** Fixed CSV parsing bug with Amazon Reconiler ([#178](https://github.com/buckets/application/issues/178))

- **FIX:** You can now import CSV files that don't have a header row ([#119](https://github.com/buckets/application/issues/119))

- **FIX:** CSV import supports amounts that use commas for decimal points.  ([#184](https://github.com/buckets/application/issues/184))

- **FIX:** Fix date picker problem with macOS High Sierra ([#112](https://github.com/buckets/application/issues/112))

- **FIX:** Removed 'Chat' as an option when an error occurs.

- **FIX:** Semicolon-delimited CSVs (so SSV?) are now supported.  ([#181](https://github.com/buckets/application/issues/181))

- **FIX:** You can now set the timezone in Preferences in case Buckets detects your timezone incorrectly.

## v0.41.0 - 2018-04-24

- **NEW:** You can now click on a bucket's want to fill in the remaining amount.  ([#ZFU7DkdT](https://trello.com/c/ZFU7DkdT))

- **NEW:** French translation now available!  Merci, Raoul de Limézy !

- **NEW:** Loading screen is nicer ([#7q3euALq](https://trello.com/c/7q3euALq))

- **NEW:** Accounts can now be designated as *Off Budget.*  Currently, it is of little use, but makes the way for tracking assets and debts (such as mortgages and investment accounts) over time.  ([#6Vo5DIEu](https://trello.com/c/6Vo5DIEu))

- **NEW:** After importing from YNAB4, a list of transactions to review is now shown.  Also there's a progress bar.  ([#KS5dedMe](https://trello.com/c/KS5dedMe))

- **FIX:** Now 'About Buckets' works consistently on macOS, Windows and Linux ([#Hvkf87aR](https://trello.com/c/Hvkf87aR))

- **FIX:** Balance as of date listed in account detail view now lists the date of the latest transaction instead of the end of the month.  ([#hMSy6JbF](https://trello.com/c/hMSy6JbF))

- **FIX:** A different icon is now used for the *clear-the-categories* button.  It was an X; now it's a circle with a line through it.  ([#Iz84zvni](https://trello.com/c/Iz84zvni))

- **FIX:** Fixed bug where kicking a bucket would change the top right month.  ([#qTNqjNav](https://trello.com/c/qTNqjNav))

- **FIX:** Safety switches (the ones that require to clicks to do the action) don't bleed now.  ([#1zvGUn99](https://trello.com/c/1zvGUn99))

- **FIX:** When you create a transaction without a category, it won't flash a warning anymore ([#YwcStIKB](https://trello.com/c/YwcStIKB))

- **FIX:** Transactions are sorted by date first, instead of account also.  This will make transfers that happen at the same time appear next to each other.  ([#D6Ftd0rZ](https://trello.com/c/D6Ftd0rZ))

- **FIX:** Notes with just whitespace are considered empty now ([#RZBnnlKJ](https://trello.com/c/RZBnnlKJ))

- Slimmed down and alphabetized translation files to make it easier for translators and to make fewer conflicts. ([#wMIaJ47X](https://trello.com/c/wMIaJ47X))

- Upgraded internal libraries and platform. ([#hcyvkiIZ](https://trello.com/c/hcyvkiIZ), [#dwtG0GDO](https://trello.com/c/dwtG0GDO))

## v0.40.1 - 2018-03-29

- **FIX:** Let us check for updates again if an update fails to download.  ([#Qtufqzis](https://trello.com/c/Qtufqzis))

- **FIX:** Fix YNAB4 import error for transactions with mixed-sign categorizations ([#KiDm6dZS](https://trello.com/c/KiDm6dZS))

## v0.40.0 - 2018-03-26

- **NEW:** Added a 'Start Over' tool.  ([#gMedmoLD](https://trello.com/c/gMedmoLD))

- **FIX:** Letters are no longer eaten when writing a note on *any* object.  ([#ZQa6alQo](https://trello.com/c/ZQa6alQo))

- **FIX:** You can choose a number format independent of your language. ([#ZaP9MCUO](https://trello.com/c/ZaP9MCUO))

## v0.39.2 - 2018-03-23

- **FIX:** Fix white on white text in transaction dropdown on Windows ([#Cb24GGRR](https://trello.com/c/Cb24GGRR))

## v0.39.1 - 2018-03-22

- **FIX:** Fixed a bug in CSV importing ([#2KYzgBet](https://trello.com/c/2KYzgBet))

- **FIX:** Sync time range alert is not correct.

## v0.39.0 - 2018-03-21

- **NEW:** It's now much easier to record transfers between accounts.  When creating a transaction, simply mark it as a transfer and choose the account the funds are coming from or going to.  ([#W1s6v7WU](https://trello.com/c/W1s6v7WU))

- **NEW:** The Buckets tab is cleaner (less busy) through the following changes.  The balance of each bucket is now the first number.  "Out" and "Transfer" columns have been combined into a single "Activity" column.  When there is an amount in the "In/Out" field, the current and future balance no longer make the table expand horizontally. The heading labels are repeated for each bucket group.  Effective balance is no longer shown when in debt.  ([#VSy1vj99](https://trello.com/c/VSy1vj99), [#6T7u0kWO](https://trello.com/c/6T7u0kWO))

- **NEW:** You can now categorize transactions as you enter them, instead of having to categorize them after adding them.

- **NEW:** The Recurring Expenses analysis chart now remembers the time period you chose. ([#2yalBubk](https://trello.com/c/2yalBubk))

- **NEW:** Names of translation contributors appear in the source file of each language.  ([#1s7TvSdi](https://trello.com/c/1s7TvSdi))

- **FIX:** For labels with a bright yellow background, black text is now used instead of white.  In other words, you can read the words now :)

- **FIX:** Simple categorization is preserved after editing transactions.  ([#L7jULmPb](https://trello.com/c/L7jULmPb))

- **FIX:** Only list recently-opened files that still exist.  ([#OvGiy3pc](https://trello.com/c/OvGiy3pc))

- **FIX:** Refunds/returns now add money to the 'Activity' column rather than the 'Rain' column on the Buckets view.  ([#zmXmsVbp](https://trello.com/c/zmXmsVbp))

## v0.38.2 - 2018-03-15

- **FIX:** Don't overwrite non-null account balances to fix daylight saving problem.

## v0.38.1 - 2018-03-14

- **FIX:** Prevent NULL amounts in transactions. ([#FJHZHCxx](https://trello.com/c/FJHZHCxx))

## v0.38.0 - 2018-03-14

- **FIX:** Handle daylight saving time ([#9MfU7pAj](https://trello.com/c/9MfU7pAj))

## v0.37.0 - 2018-03-12

- **FIX:** Several visual changes.  The Accounts view uses horizontal space better.  The Month-to-Month analysis view no longer includes the year on the first date.  ([#4MgmeJq9](https://trello.com/c/4MgmeJq9), [#5oypmRTm](https://trello.com/c/5oypmRTm), [#Ljy70cM6](https://trello.com/c/Ljy70cM6))

- **FIX:** Rain tooltip no longer has faded cents. ([#TlvT3o2a](https://trello.com/c/TlvT3o2a))

- **FIX:** When downloading an update, release notes stay visible. ([#N6ZbcQvk](https://trello.com/c/N6ZbcQvk))

## v0.36.0 - 2018-03-06

- **NEW:** Numbers are localized according to language now (i.e. in Portuguese and Spanish the decimal separator is now a comma) ([#0iXa6tJR](https://trello.com/c/0iXa6tJR))

- **FIX:** It's more obvious how to close notes. ([#2qffJJW9](https://trello.com/c/2qffJJW9))

- **FIX:** Emoji in Bucket names no longer causes height problems in macOS ([#XTu7f4EW](https://trello.com/c/XTu7f4EW))

- **FIX:** Recurring expense chart labels aren't cut off anymore.  ([#dl6Rupnn](https://trello.com/c/dl6Rupnn))

- **FIX:** Fixed an internal input warning. ([#LaBarRXx](https://trello.com/c/LaBarRXx))

- **FIX:** If there's no internet connection, an error about not being able to update is no longer displayed on start ([#hjnugHpN](https://trello.com/c/hjnugHpN))

## v0.35.1 - 2018-02-28

- **FIX:** Another fix for another kind of YNAB4 import failure.  ([#MpmFZutK](https://trello.com/c/MpmFZutK))

## v0.35.0 - 2018-02-28

- **NEW:** Added *Start with a template* button for getting started with Buckets.  ([#2kWWcMGa](https://trello.com/c/2kWWcMGa))

- **FIX:** Handle CSV files that don't have a consistent number of columns throughout.  ([#TvFClGGM](https://trello.com/c/TvFClGGM))

- **FIX:** Fixed a bug when importing YNAB4 files with transactions that are split, but not split into categories ([#rJgT119e](https://trello.com/c/rJgT119e))

## v0.34.0 - 2018-02-23

- **NEW:** Replaced confusing line and dot chart with a bar chart of historical expenses in Analysis > Recurring Expenses section.  Also, now you can choose the time period being shown.  ([#cY5uD7Y5](https://trello.com/c/cY5uD7Y5))

- **NEW:** You can now click on a bucket's balance to quickly set it to 0.  For instance, if the balance is -54 and you click it, it will prepare to deposit 54 into the bucket.  ([#WLOgdR67](https://trello.com/c/WLOgdR67))

- **NEW:** Now translated into Portuguese, graças a Carlos.  Obrigado!

- **NEW:** You can now attach screenshots to bug reports

- **NEW:** You can now undo/redo *most* actions that modify your budget.  So if you accidentally deposited $500 into the wrong bucket, press Control/Command Z to reverse the last change.  ([#JE9sINCG](https://trello.com/c/JE9sINCG))

- **FIX:** Balance chart for high numbers is now more than just a flat line ([#rYUgiuQh](https://trello.com/c/rYUgiuQh))

- **FIX:** Fixed bug where deleting an account would not always clean up associated records.

- **FIX:** Cents are shown by default now for all numbers ([#yUin1iGJ](https://trello.com/c/yUin1iGJ))

- **FIX:** Potentially fixed slowness when entering notes and goal/deposit amounts on buckets.  ([#AbqgETOV](https://trello.com/c/AbqgETOV))

- Now only the language you are using is loaded (resulting in slightly faster load times)

## v0.33.0 - 2018-02-08

- **NEW:** You can now delete bucket groups ([#02VRaU99](https://trello.com/c/02VRaU99))

- **NEW:** The Buckets view now shows the amounts put in and taken out of each bucket.  ([#wU1gc6wz](https://trello.com/c/wU1gc6wz))

- **NEW:** If you attempt to use more rain than you have available, a warning is displayed and the 'Make it so' button requires confirmation.  ([#4T1eVgov](https://trello.com/c/4T1eVgov))

- **FIX:** Bucket balance chart will divide into more than just months if it makes sense ([#fVPOUQzl](https://trello.com/c/fVPOUQzl))

- **FIX:** The Buckets view is faster(less visual lag) when entering amounts to be deposited/withdrawn.

- **FIX:** You can now edit blank group/bucket names ([#7krRuUOo](https://trello.com/c/7krRuUOo))

- **FIX:** Fixed a timezone bug in Analysis > Recurring expenses that made 'Last month' always 0.  Also changed the labels to be explicit about which month is being shown.  ([#kxaoRW0W](https://trello.com/c/kxaoRW0W))

- **FIX:** In the Transactions view, you can now click on the words 'Show uncategorized' instead of having to hit the small checkbox ([#oEuSlRsZ](https://trello.com/c/oEuSlRsZ))

- **FIX:** Bucket transactions are now sorted the same (descending date) as account transactions ([#1y6rFkMD](https://trello.com/c/1y6rFkMD))

- **FIX:** Include more verbose debugging when YNAB4 import fails.

## v0.32.0 - 2018-02-02

- **NEW:** You can delete bucket transactions (Issue [#q2PpU2iV](https://trello.com/c/q2PpU2iV))

- **NEW:** Added a 'Quit' option for Windows/Linux users.  ([#XjHhptE6](https://trello.com/c/XjHhptE6))

- **FIX:** Budget always opened to the month before the current month, by default.  Now it opens to the current month.  ([#tE6BlTgh](https://trello.com/c/tE6BlTgh))

- **FIX:** You can now adjust the Buckets License amount so that different currencies can be made to work ([#j8rA12Fu](https://trello.com/c/j8rA12Fu))

- **FIX:** Fixed math being wrong on money inputs ([#wtnk1A92](https://trello.com/c/wtnk1A92))

- **FIX:** When there are no recurring expense buckets, the analysis page no longer looks like a broken page.  ([#6snqIshs](https://trello.com/c/6snqIshs))

- **FIX:** Posted date of newly created transactions will now always be (by default) in the month you are looking at.  ([#LauMJXLI](https://trello.com/c/LauMJXLI))

## v0.31.2 - 2018-01-30

- **FIX:** Fixed *Used in future* to not include kicked buckets.

- **FIX:** Fixed future rain missed update with multiple windows ([#dXwraTOl](https://trello.com/c/dXwraTOl))

- Moved to Trello for issue/bug tracking ([#JeaRIFN9](https://trello.com/c/JeaRIFN9))

## v0.31.1 - 2018-01-29

- **FIX:** Fix error in want-to-buy message

## v0.31.0 - 2018-01-29

- **NEW:** Added a transaction export tool.  (Issue [#28](https://github.com/buckets/application/issues/28))

- **NEW:** Rain in the current month now takes into account any amount spoken for in future months.  This allows for budgeting future months.  (Issue [#38](https://github.com/buckets/application/issues/38))

- **NEW:** When reopening buckets, the last set of opened windows is restored.  (Issue [#59](https://github.com/buckets/application/issues/59))

- **FIX:** Another attempt at the off by one problem.  (Issue [#40](https://github.com/buckets/application/issues/40))

## v0.30.0 - 2018-01-25

- **NEW:** Date format is now suggested when importing from CSV

- **NEW:** Added a preference to disable money animations.

- **NEW:** When doing multiple buckets transactions at once, the math regarding what is happening now appears in the top action bar.  (Issue [#54](https://github.com/buckets/application/issues/54))

- **NEW:** Renamed 'Transact' to 'In/Out' on Buckets page.

- **FIX:** Long bucket/group names are no longer cut off (Issue [#14](https://github.com/buckets/application/issues/14))

- **FIX:** Fixed help prompt text-wrapping issue on Buckets tab Rain header.  (Issue [#57](https://github.com/buckets/application/issues/57))

- **FIX:** Default logging is more verbose

- **FIX:** Special misc group is no longer editable.  (Issue [#41](https://github.com/buckets/application/issues/41))

- **FIX:** Maybe fixed off by one month issue.  (Issue [#40](https://github.com/buckets/application/issues/40))

- **FIX:** Account-style parenthesis-delimited negative numbers are supported in CSV importing.  (Issue [#60](https://github.com/buckets/application/issues/60))

- **FIX:** Subheader on Buckets/Transactions/Accounts page is now always visible even when your scroll down.  (Issue [#58](https://github.com/buckets/application/issues/58))

- The Guide mentions that it's a work in progress now.  (Issue [#48](https://github.com/buckets/application/issues/48))

## v0.29.0 - 2018-01-22

- **NEW:** Added a preference to disable money animations

- **NEW:** CSV importing is now supported.  (Issue [#5](https://github.com/buckets/application/issues/5))

## v0.28.0 - 2018-01-19

- **NEW:** Now there's a way to submit bugs from within Buckets. (Issue [#43](https://github.com/buckets/application/issues/43))

## v0.27.1 - 2018-01-18

- **NEW:** Added some options in the Help menu to allow for more verbose log reports.

- **FIX:** Fix some database schema issues.

## v0.27.0 - 2018-01-17

- **FIX:** Check for updates, and version information is now available for Windows and Linux users.  (Issue [#43](https://github.com/buckets/application/issues/43))

- **FIX:** Fix a bug that prevented adding transactions in the account view.  (Issue [#44](https://github.com/buckets/application/issues/44))

- **FIX:** Make update window not be so small (especially on Windows) (Issue [#45](https://github.com/buckets/application/issues/45))

## v0.26.0 - 2018-01-17

- **NEW:** Added Amazon reconciliation tool.  (Issue [#33](https://github.com/buckets/application/issues/33))

- **FIX:** Database migrations are less flakey now.

## v0.25.1 - 2018-01-15

- **FIX:** Hopefully fix issue [#39](https://github.com/buckets/application/issues/39) so that importing from YNAB4 works.

- **FIX:** Make month selector more resilient to different timezones.  (Issue [#40](https://github.com/buckets/application/issues/40))

## v0.25.0 - 2018-01-15

- **NEW:** Numbers in most tables are now always dollar-aligned with faded cents when it's an even dollar.

- **NEW:** Transactions can now be edited.  (Issue: [#10](https://github.com/buckets/application/issues/10))

- **NEW:** The Buckets Guide (still largely unwritten) is now mirrored online and in the Buckets app through the Help menu

- **NEW:** Now you can add notes to accounts, buckets, transactions and groups.  (Issue [#31](https://github.com/buckets/application/issues/31))

- **NEW:** Added a *Possible Duplicates* section to the *Transactions* tab (in the case where there are possible dupes).  (Issue [#37](https://github.com/buckets/application/issues/37))

- **NEW:** A running balance column has been added to transaction lists for single accounts and buckets. (Issue [#17](https://github.com/buckets/application/issues/17))

- **NEW:** There's now a search tab, for searching for transactions, accounts and buckets.  (Issue [#30](https://github.com/buckets/application/issues/30))

- **FIX:** When viewing account details, the pane takes up more space so you can see more of the transactions.  (Issue [#36](https://github.com/buckets/application/issues/36))

- **FIX:** Horizontal scrolling now works on all pages.  (Issue [#18](https://github.com/buckets/application/issues/18))

- **FIX:** On the Buckets page, the *New bucket* button does not make the graph icon cell stretch anymore.

## v0.24.0 - 2018-01-08

- **FIX:** You can no longer make 0-amount bucket transactions (Issue [#22](https://github.com/buckets/application/issues/22))

- **FIX:** Include more information to distinguish between similar accounts when using SimpleFIN Sync

- **FIX:** Clarify that most U.S. banks are supported by SimpleFIN (Issue [#24](https://github.com/buckets/application/issues/24))

- NEW: Accounts can now be closed, and you can shoot yourself in the foot by completely deleting accounts and all linked transactions.  You're welcome.  (Issue [#2](https://github.com/buckets/application/issues/2))

## v0.23.0 - 2018-01-05

- **FIX:** Account balance table aligns balance to the right.

- **FIX:** Report bug feature now works on Windows (Issue [#11](https://github.com/buckets/application/issues/11))

- **FIX:** Fix YNAB importing for budgets that have categories without subcategories. (Issue [#12](https://github.com/buckets/application/issues/12))

- NEW: When updating Buckets, release notes are shown in the notification window, a progress bar shows progress and you can opt to skip a version to prevent more notifications. (Issues [#3](https://github.com/buckets/application/issues/3), [#9](https://github.com/buckets/application/issues/9))

- NEW: Under *Analysis* the *Regular Expenses* section includes helpful number line charts and groups buckets according to whether expenses appear monthly v. yearly (or somewhat yearly) and groups them by relative budgeted amount.  In short, it's prettier :)

## v0.22.1 - 2018-01-02

- **FIX:** Fix [issue #8](https://github.com/buckets/application/issues/8) by allowing users to select directories and files for import

## v0.22.0 - 2017-12-29

- NEW: Added first (experimental) version of creating macros to download transaction data from banks automatically.  (Not yet translated into Spanish).

## v0.21.0 - 2017-11-17

- **FIX:** Improved the explanation of what rain is

- NEW: Switch from bucketsisbetter.com to budgetwithbuckets.com

## v0.20.0 - 2017-11-06

- **FIX:** Light grey on charts is now less light and more visible

- **FIX:** When turning a bucket from a specialized type back into a regular bucket, the rain is now reported correctly (as zero)

- **FIX:** Set default save directory to ~/Documents (or OS equivalent) so that the default is no longer /

- NEW: All budget-related menu options have been moved to a single 'Budget' menu (rather than being dispersed over several other menus)

- NEW: Buckets can now import You Need a Budget (YNAB) v4 budget files.

## v0.19.0 - 2017-11-03

- **FIX:** Translate the preferences page

- NEW: Buckets files format is documented

- NEW: Auto-updating is now supported on Linux for AppImage installs

- NEW: Reduce license price from $40 to $29 (and intro price from $20 to $15)

## v0.18.0

- NEW: Buckets is now available in Spanish!

## v0.17.0 - 2017-09-12

- **FIX:** Fixed a bug that prevented actually linking SimpleFIN accounts

- NEW: Added better logging for times where there are silent errors

## v0.16.0 - 2017-09-01

- **FIX:** Got rid of scary balance-mismatch warnings that weren't actually actionable.  And a better explanation of what mismatches mean is included.

- **FIX:** Now, when you sync transactions, it will only sync the current month

- **FIX:** The update process is even *more* clear.

## v0.15.0

- **FIX:** If you try to open/create a file that's unreadable and error is displayed instead of failing silently


- NEW: You can now click 'Make it Rain' as many times as you want.  Each bucket will only take what it needs *per month*



- **FIX:** Fixed bug where 'Duplicate Window' would sometimes throw an error.

- **FIX:** Recurring expense report doesn't report false information for newly-made buckets anymore

- NEW: Added new charts to bucket information pages

- NEW: You can now explicitly mark bucket transactions as transfers


## v0.14.0

- **FIX:** When updating an account balance in a month that isn't the current month, it now does the right thing.

- **FIX:** Removed the mystery of what's going on during update download/install.

- NEW: Added a bucket expense analysis section.


## v0.13.0

- NEW: Added a new 'Analysis' section with helpful month-to-month and year-to-year charts

- NEW: Added *Chat with Matt* navigation item


## v0.12.0

- NEW: Now you can get instant help with the 'Chat...' option in the Help menu.

- NEW: Added *Effective Balance* column to buckets for when there are buckets in debt (so you don't think you have more money than you do).

- NEW: Windows are labeled with the filename now

- NEW: Linux installs will now be notified of updates, too


## v0.11.0

- **FIX:** Style fixes and extra tooltip helps

- **FIX:** Some menu items are disabled/enabled now when the context justifies it.

- **FIX:** Fixed bug where categorizing with math would sometimes make too many rows

- NEW: Categorizing is cleaner now

- NEW: Started changelog.

- NEW: Table rows are now highlighted when you hover over them

- NEW: You can now import OFX/QFX files


