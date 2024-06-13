# v0.74.1 - 2024-06-13

- **FIX:** When there's already a problem, errors localizing the menu won't cause extra errors ([#956](https://github.com/buckets/application/issues/956))
- **FIX:** Sharing folders now include a creation timestamp so you can distinguish and old and new version in the case where a device gets new keys ([#970](https://github.com/buckets/application/issues/970))
- **FIX:** Misc group buckets that disappeared in the last few versions will return and be visible ([#990](https://github.com/buckets/application/issues/990))
- **FIX:** When keys used for encrypting shared folders are broken, there is now a way to regenerate the keys in the Sharing preference pane ([#969](https://github.com/buckets/application/issues/969))
- **FIX:** Merging errors are now diplayed consistently between desktop and mobile

# v0.74.0 - 2024-03-06

- **NEW:** You can now skip updating to certain versions on Linux ([#980](https://github.com/buckets/application/issues/980))
- **NEW:** Added a 'Show Budget File' menu option to quickly locate the current budget file in Finder/Explorer ([#977](https://github.com/buckets/application/issues/977))
- **NEW:** There is now a total at the top of the Recurring Expenses report ([#954](https://github.com/buckets/application/issues/954))
- **FIX:** The Recurring Expense report now computes expenses the same way the buckets page does. ([#565](https://github.com/buckets/application/issues/565), [#854](https://github.com/buckets/application/issues/854))
- **FIX:** Updated translations for several languages
- **FIX:** When merging, schema difference detection now ignores whitespace ([#978](https://github.com/buckets/application/issues/978))
- **FIX:** Clarify that SimpleFIN is likely not free ([#827](https://github.com/buckets/application/issues/827))

# v0.73.4 - 2024-02-28

- **FIX:** When merging budgets, equivalent categorizations are no longer shown as conflicts ([#973](https://github.com/buckets/application/issues/973))

# v0.73.3 - 2024-01-30

- **FIX:** Fixed a crash that sometimes happened with the Find on page feature ([#963](https://github.com/buckets/application/issues/963))
- **FIX:** Verified fix for white screen issue on Linux ([#946](https://github.com/buckets/application/issues/946))
- **FIX:** Upgrade Electron to 26.6.7
- **FIX:** Fixed a crash caused by trying to access windows that are already closed ([#966](https://github.com/buckets/application/issues/966))
- **FIX:** Fixed an error that caused no windows to show up on Linux when trying to open last saved windows. ([#965](https://github.com/buckets/application/issues/965))

# v0.73.2 - 2024-01-16

- **FIX:** Fixed minor logging typo with shared folders ([#955](https://github.com/buckets/application/issues/955))
- **FIX:** Fixed slowness introduced in latest version ([#957](https://github.com/buckets/application/issues/957))

# v0.73.1 - 2024-01-15

- **FIX:** Fixed a bug that prevented deleting existing sharing avenues when upgrading to v0.73.0 ([#949](https://github.com/buckets/application/issues/949))
- **FIX:** On Linux, GPU rendering is now disabled by default to fix a rendering bug on many Linux machines. To reenable it set `BUCKETS_ENABLE_HARDWARE_ACCELERATION=1` when running Buckets. ([#946](https://github.com/buckets/application/issues/946))
- **FIX:** Fixed a crash that happened when a shared folder becomes unavailable ([#953](https://github.com/buckets/application/issues/953))
- **FIX:** Errors during merging are now shown as specific error messages ([#950](https://github.com/buckets/application/issues/950))
- **FIX:** Catch more errors during update instead of crashing ([#934](https://github.com/buckets/application/issues/934), [#939](https://github.com/buckets/application/issues/939), [#941](https://github.com/buckets/application/issues/941))
- **FIX:** Fixed rare crash from translation misconfiguration ([#938](https://github.com/buckets/application/issues/938))

# v0.73.0 - 2024-01-04

- **BREAKING CHANGE:** **If you open a budget with this version, you will likely not be able to open it with a prior version.** This version changes all sequential database IDs to non-sequential GUIDs to prepare for device-to-device syncing.
- **NEW:** Budget files can now be merged! Go to *Tools* > *Merge Budgets* to try it out. ([#134](https://github.com/buckets/application/issues/134))
- **NEW:** Upgraded SQLite to 3.44.0
- **NEW:** Account starting balance is now stored explicitly (rather than being computed from the recorded balance and all balance-affecting transactions)
- **NEW:** Budgets can be shared between devices using a shared folder, such as is offered by Dropbox, Google Drive, iCloud and others. ([#276](https://github.com/buckets/application/issues/276), [#548](https://github.com/buckets/application/issues/548), [#633](https://github.com/buckets/application/issues/633), [#712](https://github.com/buckets/application/issues/712), [#891](https://github.com/buckets/application/issues/891))
- **FIX:** Generic linux builds use `linux-latest` rather than `ubuntu-22.04` in their filename. ([#937](https://github.com/buckets/application/issues/937))
- **FIX:** Fixed translations for Estonian, Spanish, Turkish, Romanian and Portuguese. Thank you, translators!
- **FIX:** Add Беларуская translations -- thank you Yahor!

# v0.72.2 - 2024-01-30

- **FIX:** Verified fix for white screen issue on Linux ([#946](https://github.com/buckets/application/issues/946))
- **FIX:** Upgrade Electron to 26.6.7

# v0.72.1 - 2023-10-06

- **FIX:** On Windows and Linux, Buckets will do better at reopening the last set of windows you had opened when you closed it. ([#406](https://github.com/buckets/application/issues/406), [#751](https://github.com/buckets/application/issues/751))
- **FIX:** Fix error when accounts used in syncing were deleted but not fully cleaned up ([#931](https://github.com/buckets/application/issues/931))
- **FIX:** When Buckets fails to get a valid SimpleFIN Access URL, it no longer stores it as if it's a good one ([#930](https://github.com/buckets/application/issues/930))
- **FIX:** When a new update is available for Buckets Beta on Linux, it will send you to the Beta download page rather than the Stable download page. ([#933](https://github.com/buckets/application/issues/933))
- **FIX:** The calendar popup no longer hangs around when you focus on the next field ([#924](https://github.com/buckets/application/issues/924))

# v0.72.0 - 2023-09-28

- **NEW:** You can now print (to paper or PDF) various pages! Some screens will look better than others. This is mostly to make the new Income and Expense report printable. ([#285](https://github.com/buckets/application/issues/285))
- **NEW:** Added a first draft of a simple Income and Expense report under Analysis ([#927](https://github.com/buckets/application/issues/927))
- **NEW:** Buckets is now built for Apple Silicon (M1/M2/ARM64) machines in addition to Intel macOS machines ([#688](https://github.com/buckets/application/issues/688), [#906](https://github.com/buckets/application/issues/906))
- **NEW:** Buckets is now built for Linux ARM64 devices ([#735](https://github.com/buckets/application/issues/735), [#763](https://github.com/buckets/application/issues/763))
- **FIX:** Export date range inputs now work again. Also, the list of available date range presets has expanded and exported transaction filenames now include the date range ([#922](https://github.com/buckets/application/issues/922))
- **FIX:** Fixed a startup failure on various Linux distributions that required passing `--no-sandbox` when launching. You should no longer need to pass that flag. ([#916](https://github.com/buckets/application/issues/916), [#781](https://github.com/buckets/application/issues/781))
- **FIX:** Fixed a common logging error that happened in languages other than English ([#852](https://github.com/buckets/application/issues/852), [#873](https://github.com/buckets/application/issues/873))
- **FIX:** Fixed a crash that would happen when importing from malformed nYNAB files ([#642](https://github.com/buckets/application/issues/642))
- **FIX:** Find on page functionality has been rewritten and should be much less prone to errors ([#465](https://github.com/buckets/application/issues/465))
- **FIX:** The *cents* part of the Expenses number at the top is now affixed to the top like all the other numbers in that area ([#349](https://github.com/buckets/application/issues/349))
- **FIX:** Resizing windows on Windows should no longer result in a black screen ([#791](https://github.com/buckets/application/issues/791))
- **FIX:** Fixed a launch crash that happened on Ubuntu 22.10 ([#829](https://github.com/buckets/application/issues/829), [#724](https://github.com/buckets/application/issues/724))
- **FIX:** Off-budget accounts show up in the dropdowns for creating transactions and transfers again ([#929](https://github.com/buckets/application/issues/929))
- **FIX:** Update license price to $64
- **FIX:** macOS fonts will no longer turn blurry ([#848](https://github.com/buckets/application/issues/848))
- Upgraded to Electron 26 ([#885](https://github.com/buckets/application/issues/885), [#559](https://github.com/buckets/application/issues/559))

# v0.71.1 - 2023-08-10

- **FIX:** Move calendar in new date picker to the front of the input to transaction-entry require one less tab ([#917](https://github.com/buckets/application/issues/917))

# v0.71.0 - 2023-07-06

- **NEW:** Closed accounts no longer show in the Transaction page dropdown. If you need to create a transaction for a closed account, go to the page for closed account. ([#470](https://github.com/buckets/application/issues/470))
- **NEW:** After adding a transaction, focus will go to the date input rather than the memo. This way, you should be able to only ever press `Tab` and not have to press `Shift`-`Tab` to go back to the date. ([#476](https://github.com/buckets/application/issues/476))
- **NEW:** Improved the transaction date picker, including fixing a bug that caused both day and month to change when adjusting with the keyboard ([#728](https://github.com/buckets/application/issues/728), [#240](https://github.com/buckets/application/issues/240), [#258](https://github.com/buckets/application/issues/258), [#721](https://github.com/buckets/application/issues/721))
- **FIX:** Bug reports now include log files formatted correctly.
- **FIX:** While the clickable arrows aren't back, you can use the keyboard to adjust each part of the date now ([#824](https://github.com/buckets/application/issues/824))
- **FIX:** Removed clutter from log for backups ([#912](https://github.com/buckets/application/issues/912))
- **FIX:** Some OFX files lack account information for banks that reuse transaction ids across different accounts. You can now import those transactions and see which transactions are duplicates. ([#894](https://github.com/buckets/application/issues/894))

# v0.70.5 - 2023-06-08

- **FIX:** Fixed an error that prevented pasting a Buckets License in when trying to use the Buckets Relay ([#884](https://github.com/buckets/application/issues/884))
- **FIX:** Show local sharing server as "Running" instead of "Starting" when it's actually running.
- **FIX:** Bug reports work again and failed report submissions are no longer reported as successes in the log ([#909](https://github.com/buckets/application/issues/909))
- **FIX:** When checking for updates fails for network problems outside of Buckets' control, an error is no longer shown to the user ([#898](https://github.com/buckets/application/issues/898))
- **FIX:** In sidebar list of accounts, a consistent number of decimal places is now shown, even if the "cents" part is 0 ([#910](https://github.com/buckets/application/issues/910))

# v0.70.4 - 2023-04-11

- **FIX:** Fixed SimpleFIN Bridge certificate errors by using a more forward-compatible method of making HTTP requests ([#895](https://github.com/buckets/application/issues/895))

# v0.70.3 - 2023-03-21

- **FIX:** Update translations for Polski, Español, Português and Română. Thank you, translators!
- **FIX:** A failed backup will no longer crash Buckets ([#879](https://github.com/buckets/application/issues/879))
- **FIX:** Fix bug with a missing function in `libSystem` on macOS High Sierra ([#881](https://github.com/buckets/application/issues/881))

# v0.70.2 - 2023-03-07

- **FIX:** Fix failure to run on Windows 11 due to missing `libwinpthread-1.dll` ([#876](https://github.com/buckets/application/issues/876))

# v0.70.1 - 2023-03-06

- **FIX:** Fix missing symbol on older macOS versions ([#870](https://github.com/buckets/application/issues/870), [#808](https://github.com/buckets/application/issues/808))
- **FIX:** Statically link libsodium on Linux again ([#861](https://github.com/buckets/application/issues/861), [#825](https://github.com/buckets/application/issues/825))
- **FIX:** Include bug report ID in bug report submission body so we can find old bug reports more easily
- **FIX:** Prevent rare error when updating an account balance without a transaction  ([#835](https://github.com/buckets/application/issues/835))
- **FIX:** Fixed a bug that prevented you from entering two transactions in a row for the same account ([#868](https://github.com/buckets/application/issues/868))

# v0.70.0 - 2023-03-01

- **NEW:** Sharing between devices is much more straightforward now. Also, you many now share using the public relay (or your own relay if you'd like to host one). ([#670](https://github.com/buckets/application/issues/670), [#866](https://github.com/buckets/application/issues/866), [#850](https://github.com/buckets/application/issues/850))
- **FIX:** Support sharing on older macOS computers ([#687](https://github.com/buckets/application/issues/687))
- **FIX:** Make various transient errors that sometimes happen during auto updates less annoying and only pop up the update window when there's something a user can do ([#570](https://github.com/buckets/application/issues/570), [#817](https://github.com/buckets/application/issues/817), [#822](https://github.com/buckets/application/issues/822), [#830](https://github.com/buckets/application/issues/830), [#839](https://github.com/buckets/application/issues/839), [#840](https://github.com/buckets/application/issues/840), [#859](https://github.com/buckets/application/issues/859), [#864](https://github.com/buckets/application/issues/864))
- **FIX:** Fix auto update on Windows due to certificate Common Name case mismatch ([#836](https://github.com/buckets/application/issues/836))

# v0.69.0 - 2022-11-30

- **NEW:** Added End User License Agreement and Privacy Policy to Guide. Also, you may choose to accept the EULA through App Settings. In a future version all users will be **required** to accept the EULA to continue using Buckets.
- **NEW:** Made bucket names in the Recurring Expense report link to the individual bucket view ([#314](https://github.com/buckets/application/issues/314))
- **NEW:** Accounts balances in the sidebar now include cents ([#601](https://github.com/buckets/application/issues/601))
- **NEW:** If a budget has only one account, it will be automatically chosen in the transaction-creation form ([#441](https://github.com/buckets/application/issues/441))
- **NEW:** More prominently display "Undo" after deleting and account. ([#813](https://github.com/buckets/application/issues/813))
- **NEW:** Added more default time formats for CSV importing, including single-digit months and days ([#826](https://github.com/buckets/application/issues/826))
- **FIX:** The Recurring Expense report now includes the current month ([#337](https://github.com/buckets/application/issues/337))
- **FIX:** Preferences, Bank macro recorder and bug report windows no longer have a menu on Windows and Linux ([#617](https://github.com/buckets/application/issues/617), [#806](https://github.com/buckets/application/issues/806), [#805](https://github.com/buckets/application/issues/805))
- **FIX:** You can now categorize 0-amount transactions ([#700](https://github.com/buckets/application/issues/700))
- **FIX:** Fixed failure to parse OFX timestamps with a 'GMT' at the end ([#815](https://github.com/buckets/application/issues/815))
- **FIX:** The plus button to add a bucket is aligned correctly on the Misc group ([#501](https://github.com/buckets/application/issues/501))
- **FIX:** The bucket settings and trash can icon is now separated to make it less goofy ([#562](https://github.com/buckets/application/issues/562))
- **FIX:** Upgrade SQLite to 3.39.4
- **FIX:** The bucket settings acceptance button (the checkmark) is now lined up better with the settings box ([#242](https://github.com/buckets/application/issues/242))
- **FIX:** On the account list table, you can now click anywhere in the name cell to go to an account's details (so that it's easier to click on accounts with short names) ([#578](https://github.com/buckets/application/issues/578))
- **FIX:** Changed the Rain/mo tooltip to specifically mention *want* (since it's a sum of all the bucket wants) ([#326](https://github.com/buckets/application/issues/326))

# v0.68.0 - 2022-09-22

- **NEW:** Automatic backups are now created for your budgets. ([#74](https://github.com/buckets/application/issues/74))
- **FIX:** Fixed regression that prevented importing into off-budget accounts ([#284](https://github.com/buckets/application/issues/284))
- **FIX:** Restored some of the readability of the category-choosing dropdown by removing whitespace and allowing the popup menu to expand its width ([#780](https://github.com/buckets/application/issues/780))
- **FIX:** Fixed license entry field so that copying and pasting works on all machines ([#587](https://github.com/buckets/application/issues/587))
- **FIX:** If automatic updates fail, users are prompted to download from the website instead ([#786](https://github.com/buckets/application/issues/786))

# v0.67.2 - 2022-09-05

- **FIX:** Several translation fixes for Türkçe, Español and Eesti. Thank you, contributors!
- **FIX:** Log OS version for debugging help
- **FIX:** Fixed bug in OFX importing where later transactions would get copies of data from earlier transactions ([#778](https://github.com/buckets/application/issues/778))
- **FIX:** If you accidentally give an account a blank name, you can now rename it ([#785](https://github.com/buckets/application/issues/785))
- **FIX:** Restore ability to import CSV files with separate credit/debit columns where both are positive ([#790](https://github.com/buckets/application/issues/790))

# v0.67.1 - 2022-07-25

- **FIX:** A bucket's *Activity* and *In* amounts are now correctly updated when you undo a prior deposit or withdrawal ([#591](https://github.com/buckets/application/issues/591))
- **FIX:** Document that Rain only makes sense when transactions have all been categorized ([#508](https://github.com/buckets/application/issues/508))
- **FIX:** CSV imports will treat parentheses-enclosed numbers as negative ([#740](https://github.com/buckets/application/issues/740))
- **FIX:** Syncing from SimpleFIN will no longer overwrite the memo unless it's blank ([#746](https://github.com/buckets/application/issues/746))
- **FIX:** In the case where 0-amount transactions are created (typically via import/sync) you can now categorize them so they no longer show as uncategorized ([#700](https://github.com/buckets/application/issues/700))
- **FIX:** When importing from YNAB4, Buckets now looks for `Budget.ymeta` and `Budget.yfull` files in more places ([#429](https://github.com/buckets/application/issues/429), [#493](https://github.com/buckets/application/issues/493))
- **FIX:** Fuzzy searching when categorizing will now highlight the best option consistently ([#773](https://github.com/buckets/application/issues/773))
- **FIX:** Prior to this change, if you kicked the Buckets License bucket it would reappear next time you opened the budget. This was confusing. Now, you can no longer kick it at all with the Trial Version. ([#609](https://github.com/buckets/application/issues/609))
- **FIX:** Removed up/down buttons on all date inputs because they are buggy and the keyboard up/down keys can achieve the same effect. ([#764](https://github.com/buckets/application/issues/764))

# v0.67.0 - 2022-07-18

- **BREAKING CHANGE:** When entering transaction amounts, typing `-` before the number will no longer flip the sign. Sorry, we know this is going to ruin your muscle memory! Instead, type `+` for positive numbers and use no prefix (or type `-`) to use negative numbers. You can also click on the big `-` before the amount to toggle between positive and negative numbers ([#725](https://github.com/buckets/application/issues/725), [#496](https://github.com/buckets/application/issues/496))
- **NEW:** Added 8 new colorblind-friendly default bucket colors *and* added a color picker so you can choose whatever hue hue want! ([#690](https://github.com/buckets/application/issues/690))
- **NEW:** Buckets with the same name will now also include their group name in the categorizing dropdown list. ([#594](https://github.com/buckets/application/issues/594))
- **NEW:** Handle new SimpleFIN `pending` transaction attribute. At this point, the attribute is used to ignore pending transactions but will be used in the future to add the transactions once pending transactions are added to Buckets.
- **NEW:** You can now do fuzzy searching when categorizing transactions. That is, you can type "Insurance" and it will match both "Car Insurance" and "Dog insurance" buckets. ([#153](https://github.com/buckets/application/issues/153))
- **FIX:** Silence Dbus-related errors on Linux when keychain access fails ([#755](https://github.com/buckets/application/issues/755))

# v0.66.5 - 2022-06-20

- **FIX:** Fix startup error on Windows ([#762](https://github.com/buckets/application/issues/762))
- **FIX:** Updates to various translations. Thank you, all!

# v0.66.4 - 2022-06-13

- **FIX:** Changed how *Activity* is computed so that it *only* includes real life income/expenses for a bucket. Also changed *In* to only include money directly deposited into or withdrawn from a bucket via the In/Out input. ([#362](https://github.com/buckets/application/issues/362))
- **FIX:** When categorizing, you can now enter a number higher than the total amount so you can do math with it. ([#118](https://github.com/buckets/application/issues/118))
- **FIX:** CSV date format chooser now explicitly mentions that you can type a custom format ([#752](https://github.com/buckets/application/issues/752))
- **FIX:** Remove the "running balance does not match the last synced balance" warning, as it was almost always unhelpful ([#706](https://github.com/buckets/application/issues/706))
- **FIX:** Removed notice about Amazon tool not working, because it still works ([#528](https://github.com/buckets/application/issues/528))
- **FIX:** Removed closed accounts from the transfer to/from dropdown ([#543](https://github.com/buckets/application/issues/543))
- **FIX:** Fix race condition error on application startup ([#580](https://github.com/buckets/application/issues/580))
- **FIX:** Bug reports now include version number in the subject line  (internal change).

# v0.66.3 - 2022-04-19

- **FIX:** Exporting tool now honors the date range you pick ([#563](https://github.com/buckets/application/issues/563))
- **FIX:** Activity no longer shows up in the wrong month ([#744](https://github.com/buckets/application/issues/744))

# v0.66.2 - 2022-04-14

- **FIX:** Restore proper ordering to transactions ([#739](https://github.com/buckets/application/issues/739))

# v0.66.1 - 2022-04-13

- **FIX:** Improved logging when importing transaction data.
- **FIX:** Fixed regression preventing imports in budgets with a mix of manually-entered and imported transactions ([#739](https://github.com/buckets/application/issues/739))

# v0.66.0 - 2022-04-05

- **NEW:** When importing OFX/QFX files, you may now swap the `<NAME>` and `<MEMO>` fields ([#366](https://github.com/buckets/application/issues/366))
- **FIX:** When importing CSV or OFX files, you can now invert the sign of transaction amounts *per account.* ([#574](https://github.com/buckets/application/issues/574))
- **FIX:** When importing from CSV/OFX, duplicates aren't created anymore and existing data is left intact. ([#338](https://github.com/buckets/application/issues/338))
- **FIX:** When creating a new budget file, it no longer hangs sometimes before  opening the budget ([#611](https://github.com/buckets/application/issues/611))
- **FIX:** When importing CSV files, you can use patterns with periods in them now, like `dd.MM.yyyy` ([#723](https://github.com/buckets/application/issues/723))

# v0.65.0 - 2022-02-17

- **NEW:** CSV files delimited by semicolons and tabs can now be imported ([#530](https://github.com/buckets/application/issues/530))
- **NEW:** Buckets now supports currencies with 3 (or more) decimal places and any thousands or decimal separator ([#597](https://github.com/buckets/application/issues/597))
- **NEW:** You can now search for numbers on the search page. ([#422](https://github.com/buckets/application/issues/422))
- **NEW:** You can choose the number format when importing OFX files ([#583](https://github.com/buckets/application/issues/583))
- **NEW:** Added a keyboard shortcut and menu item to quickly get to the search page (`Command /` or `Control /`)
- **NEW:** Exports now include transaction notes ([#717](https://github.com/buckets/application/issues/717))
- **FIX:** Fixed link to purchase license and ability to paste license for some macOS users ([#587](https://github.com/buckets/application/issues/587))
- **FIX:** When importing, you can now ignore unknown/unlinked accounts ([#408](https://github.com/buckets/application/issues/408))
- **FIX:** Fixed crash when importing from nYNAB without a delimiter ([#716](https://github.com/buckets/application/issues/716))
- **FIX:** When importing CSV files, selecting multiple columns for 'Memo' will now concatenate the chosen fields ([#331](https://github.com/buckets/application/issues/331))
- **FIX:** When importing CSV files, dates are no longer incorrectly flagged as invalid ([#581](https://github.com/buckets/application/issues/581),[#573](https://github.com/buckets/application/issues/573),[#533](https://github.com/buckets/application/issues/533))
- **FIX:** You can now cancel CSV imports ([#324](https://github.com/buckets/application/issues/324))
- **FIX:** CSV import can now handle dates of the format 01 JAN 2020 ([#702](https://github.com/buckets/application/issues/702))
- **FIX:** Fixed various errors encountered while importing transactions from OFX and CSV files ([#340](https://github.com/buckets/application/issues/340), [#463](https://github.com/buckets/application/issues/463), [#545](https://github.com/buckets/application/issues/545), [#536](https://github.com/buckets/application/issues/536), [#502](https://github.com/buckets/application/issues/502))
- **FIX:** OFX files with mismatched `<CCSTMTRS>` and `</STMTRS>` tags can now be imported ([#378](https://github.com/buckets/application/issues/378))
- **FIX:** CSV importing can handle much bigger files now ([#459](https://github.com/buckets/application/issues/459))
- **FIX:** Fixed a bug that discarded pending bucket name changes when you updated a bucket groups name. ([#231](https://github.com/buckets/application/issues/231), [#661](https://github.com/buckets/application/issues/661))
- **FIX:** When importing CSV files, you can now exclude rows from the top and bottom of the CSV file ([#300](https://github.com/buckets/application/issues/300))
- **FIX:** Fixed error on search page ([#644](https://github.com/buckets/application/issues/644))
- **FIX:** When importing CSV files, fixed a bug where columns were duplicated if they had the same header ([#460](https://github.com/buckets/application/issues/460))
- **FIX:** When importing CSV files, removed *Unique ID* column in favor of computing it automatically ([#556](https://github.com/buckets/application/issues/556))
- **FIX:** More French translations!
- **FIX:** OFX files with lone `&` characters are now supported ([#627](https://github.com/buckets/application/issues/627))
- **FIX:** When importing from CSV, you may reverse the order transactions are imported if the CSV list transactions from most to least recent ([#329](https://github.com/buckets/application/issues/329))
- **FIX:** New translations for Română, Español, Deutsch and Русский!

# v0.64.0 - 2021-12-14

- **NEW:** Added documentation for sharing tool, describing how to get budget files from the Desktop app to the mobile app. ([#655](https://github.com/buckets/application/issues/655))
- **NEW:** Updated sharing tool to match most recent mobile app version.
- **FIX:** Updated German translations
- **FIX:** Fixed month names for Swedish ([#616](https://github.com/buckets/application/issues/616))

# v0.63.2 - 2021-11-10

- **FIX:** More Turkish translations.
- **FIX:** During nYNAB import, decimal and thousands separators are now honored. ([#641](https://github.com/buckets/application/issues/641))
- **FIX:** When importing from nNYAB, Buckets attempts to guess the date format if it doesn't match what was given ([#634](https://github.com/buckets/application/issues/634))
- **FIX:** More Norwegian translations.
- **FIX:** More Hungarian translations.
- **FIX:** More Spanish translations. Thanks, osanchez!

# v0.63.1 - 2021-11-06

- **FIX:** In nYNAB import, don't stop if there's an unknown category ([#614](https://github.com/buckets/application/issues/614))

# v0.63.0 - 2021-11-05

- **NEW:** Buckets is now partially translated into Magyar. Thanks Peter!
- **NEW:** Buckets is now translated into Svenska. Tack, Therese!
- **NEW:** Buckets is now partially translated into Eesti. Thanks, Indrek!
- **FIX:** When importing from nYNAB, there's now an indication that something is actually happening :) ([#598](https://github.com/buckets/application/issues/598))
- **FIX:** When importing from nYNAB, Buckets does better at keeping activity in past months instead of all in the current month ([#603](https://github.com/buckets/application/issues/603))
- **FIX:** When importing from nYNAB, reconciled transactions are now marked as cleared. ([#610](https://github.com/buckets/application/issues/610))
- Rename Bokmål to Norsk

# v0.62.0 - 2021-11-03

- **NEW:** Buckets is now available in Bokmål. Takk, Viggo!
- **FIX:** When importing from web YNAB, dates with periods `.` are now parsed correctly.
- **FIX:** Kubuntu users can now import YNAB4 files ([#582](https://github.com/buckets/application/issues/582))
- **FIX:** Fix on Windows to let users select the YNAB .zip file instead of just directories ([#595](https://github.com/buckets/application/issues/595))
- **FIX:** When importing from Web YNAB, buckets retain more category history than before ([#596](https://github.com/buckets/application/issues/596))

# v0.61.0 - 2021-11-03

- **NEW:** Added the ability to import from nYNAB's exported zip files. ([#110](https://github.com/buckets/application/issues/110))
- **NEW:** Faint cents are now disabled by default. You can re-enable them in preferences if you like squinting :) ([#344](https://github.com/buckets/application/issues/344))

# v0.60.1 - 2021-10-05

- **FIX:** Allow Kubuntu users to navigate filesystem when looking for YNAB4 files to import ([#582](https://github.com/buckets/application/issues/582))
- **FIX:** Buckets no longer crashes on startup on Windows ([#584](https://github.com/buckets/application/issues/584))

# v0.60.0 - 2021-09-13

- **NEW:** Builds are more automated now.
- **FIX:** When submitting bugs, redirects are followed now.
- Updated bug-reporting server URL.

# v0.59.0 - 2021-07-14

- **NEW:** Updated computer-to-computer sync protocol to be forward compatible
- **NEW:** Upgrade SQLite to v3.35.0
- **FIX:** Fixed a crash caused by goal buckets with very large goals ([#547](https://github.com/buckets/application/issues/547))
- **FIX:** Fix a few errors that happened when choosing months in the month pickers ([#546](https://github.com/buckets/application/issues/546), [#568](https://github.com/buckets/application/issues/568))
- **FIX:** Fixed a bug that made it seem like undo/redo wasn't working when in fact it was just not updating the screen in some cases ([#564](https://github.com/buckets/application/issues/564), [#552](https://github.com/buckets/application/issues/552))

# v0.58.0 - 2020-11-19

- **FIX:** Accounts are now sorted alphabetically ([#148](https://github.com/buckets/application/issues/148))
- **FIX:** Fixed bug that prevented entering some years in a goal bucket target date ([#539](https://github.com/buckets/application/issues/539))
- **FIX:** Fixed crash caused by invalid transaction dates ([#537](https://github.com/buckets/application/issues/537))
- **FIX:** Windows 10 may auto-update again (on the next version, though) ([#538](https://github.com/buckets/application/issues/538))

# v0.57.5 - 2020-11-12

- **NEW:** Added a debugging tool for those extra tricky bugs
- **FIX:** Tooltip flickering on calculator has been fixed ([#498](https://github.com/buckets/application/issues/498))
- **FIX:** Now you can't accidentally make duplicate transactions by pressing enter really quickly ([#487](https://github.com/buckets/application/issues/487))
- **FIX:** Application no longer crashes when trying to open a non-existent file ([#488](https://github.com/buckets/application/issues/488))
- **FIX:** Fix goal date picker going to wrong year ([#527](https://github.com/buckets/application/issues/527))
- **FIX:** Newly created "Save X by Y date" buckets now immediately show the required deposit after you enter a goal ([#526](https://github.com/buckets/application/issues/526))
- **FIX:** Fixed bug where a invalid timestamp caused an error when attempting to turn it into a date ([#529](https://github.com/buckets/application/issues/529))
- **FIX:** The *Make it so* button again clears out all the current values in In/Out ([#531](https://github.com/buckets/application/issues/531))
- Reduced error logging for missing locales ([#489](https://github.com/buckets/application/issues/489))
- Deprecated Amazon Reconciliation tool, *sniff*

# v0.57.4 - 2020-10-14

- **NEW:** Make SimpleFIN sync faster by requesting whole time period at once ([#511](https://github.com/buckets/application/issues/511))
- **FIX:** Fixed several date/time and timezone bugs, especially for our friends down under. ([#515](https://github.com/buckets/application/issues/515), [#516](https://github.com/buckets/application/issues/516), [#518](https://github.com/buckets/application/issues/518), [#519](https://github.com/buckets/application/issues/519))
- **FIX:** Fixed error that caused too many requests to SimpleFIN server ([#522](https://github.com/buckets/application/issues/522))
- Made null-checking more strict to prevent TypeErrors ([#517](https://github.com/buckets/application/issues/517))

# v0.57.3 - 2020-10-05

- **NEW:** Remove need to select timezone ([#180](https://github.com/buckets/application/issues/180))
- **FIX:** Fix goal bucket being off by one month ([#407](https://github.com/buckets/application/issues/407))
- **FIX:** Fixed end-of-month, disappearing transactions bug ([#514](https://github.com/buckets/application/issues/514), [#510](https://github.com/buckets/application/issues/510), [#170](https://github.com/buckets/application/issues/170))

# v0.57.2 - 2020-08-21

- **FIX:** Show on the import page that Buckets can import OFX, QFX and CSV files ([#445](https://github.com/buckets/application/issues/445))
- **FIX:** Fix undo/redo bug that would sometimes break budget files ([#484](https://github.com/buckets/application/issues/484))
- Changing between months is faster now.

# v0.57.1 - 2020-08-12

- **FIX:** Fix bug where opening multiple budgets caused interference between them. It was never reported from users, so it may never have been a problem other than in development.
- **FIX:** Fixed bug that prevented transaction data from being updated ([#479](https://github.com/buckets/application/issues/479))

# v0.57.0 - 2020-07-31

- **FIX:** Fix excessive use of file descriptors crash ([#474](https://github.com/buckets/application/issues/474))
- **FIX:** Fix macOS notarization for Catalina ([#478](https://github.com/buckets/application/issues/478))
- Refactored the computation of most budget values to make it consistent with mobile app.
- Better explanation of how to categorize debt transactions.

# v0.56.2 - 2020-06-12

- **FIX:** Turned a silent crash into a reported crash ([#464](https://github.com/buckets/application/issues/464))
- **FIX:** Fix date-formatting bug that caused crash ([#468](https://github.com/buckets/application/issues/468))
- **FIX:** CSV importing with separate "sign" column works again ([#442](https://github.com/buckets/application/issues/442))
- **FIX:** Fix issue where currency symbol would get corrupted when changing it ([#469](https://github.com/buckets/application/issues/469))
- **FIX:** Attempted fix for macOS 10.10 failure to run after update. ([#472](https://github.com/buckets/application/issues/472))
- Removed the part on the export page asking why you're exporting data.

# v0.56.1 - 2020-05-21

- **FIX:** Fix random, discrepency between uncategorized transaction count and the transaction badge.  ([#453](https://github.com/buckets/application/issues/453), [#454](https://github.com/buckets/application/issues/454))
- **FIX:** No more security error on macOS Catalina ([#428](https://github.com/buckets/application/issues/428))
- **FIX:** Fixed OFX import error when accounts have no name ([#386](https://github.com/buckets/application/issues/386))
- **FIX:** Fixed various TypeErrors ([#458](https://github.com/buckets/application/issues/458), [#414](https://github.com/buckets/application/issues/414), [#413](https://github.com/buckets/application/issues/413), [#461](https://github.com/buckets/application/issues/461))
- **FIX:** Fixed error when reopening the same budget file without quitting ([#451](https://github.com/buckets/application/issues/451))
- **FIX:** Undoing of large actions now works ([#450](https://github.com/buckets/application/issues/450))

# v0.56.0 - 2020-04-20

- **NEW:** Buckets is now available in Italiano!  Grazie!
- **NEW:** Various translation additions/changes for Polski, Deutsch and Français.
- **FIX:** Guide navigation in Windows fixed ([#452](https://github.com/buckets/application/issues/452))

# v0.55.4 - 2019-06-11

- **NEW:** Added keyboard shortcuts for going forward and back a year.
- **FIX:** Year-to-Year and Month-to-Month analysis charts now clearly indicate the period being averaged and totaled. ([#343](https://github.com/buckets/application/issues/343))
- **FIX:** Analysis chart dots are finally lined up ([#158](https://github.com/buckets/application/issues/158))
- **FIX:** Clicking on a bucket's *Want* column will no longer try to remove money from a bucket that has been overfilled.  ([#396](https://github.com/buckets/application/issues/396))
- **FIX:** Daylight savings time no longer confuses the goal date calculations. ([#288](https://github.com/buckets/application/issues/288))
- **FIX:** When searching on the page for something, the find next/find prev buttons now work ([#353](https://github.com/buckets/application/issues/353))
- **FIX:** Guide is reachable again on Windows/Linux ([#402](https://github.com/buckets/application/issues/402))
- **FIX:** You can now access invalid years (e.g. 200 AD) to fix mistakenly added transactions. ([#400](https://github.com/buckets/application/issues/400))
- **FIX:** The month selector will now show even if the content below it is very wide.  ([#257](https://github.com/buckets/application/issues/257))
- **FIX:** Off-budget transactions no longer show up in analysis charts ([#397](https://github.com/buckets/application/issues/397), [#296](https://github.com/buckets/application/issues/296))
- **FIX:** When entering transfers, the same date is now used for both transactions.  ([#391](https://github.com/buckets/application/issues/391))

# v0.55.3 - 2019-05-27

- **FIX:** Fixed bug that was labelling Income as Debt when entering transactions.  ([#390](https://github.com/buckets/application/issues/390))
- **FIX:** Sidebar calculator now correctly honors chosen number format. ([#398](https://github.com/buckets/application/issues/398))
- **FIX:** Fixed it so that clicking on the want bubble doesn't fill in the in/out amount so as to prevent the tooltip from staying open annoyingly.  ([#395](https://github.com/buckets/application/issues/395))
- **FIX:** Fixed it so that when entering a transfer, the +/- toggle will correctly toggle between Transfer From/To.  ([#348](https://github.com/buckets/application/issues/348))
- **FIX:** Importing from YNAB4 no longer appears to hang (though it is still a little choppy).  ([#399](https://github.com/buckets/application/issues/399))
- **FIX:** Fixed bug where YNAB4 import multiplied numbers by 100 ([#387](https://github.com/buckets/application/issues/387))

# v0.55.2 - 2019-05-15

- **NEW:** Upgraded font to better support Cyrillic characters ([#381](https://github.com/buckets/application/issues/381))
- **FIX:** Search box now appears on top of everything, including faint cents ([#356](https://github.com/buckets/application/issues/356))
- **FIX:** Fixed bug where Linux Beta version would offer to update to latest non-Beta version ([#383](https://github.com/buckets/application/issues/383))
- **FIX:** Long numbers no longer split across lines.  ([#389](https://github.com/buckets/application/issues/389))
- **FIX:** When you have many accounts showing in the left navigation bar, you can now scroll down to see all nagivation items.  ([#380](https://github.com/buckets/application/issues/380))
- **FIX:** Added more logging for unhandled errors
- **FIX:** Fixed a bug in the *Want* for *Save X by Y date* buckets where the amount would change incorrectly after depositing an amount during a month.  ([#346](https://github.com/buckets/application/issues/346))
- **FIX:** Fixed error during some YNAB4 imports. ([#392](https://github.com/buckets/application/issues/392))

# v0.55.1 - 2019-03-26

- **FIX:** Fixed bug with want values not showing up ([#377](https://github.com/buckets/application/issues/377))

# v0.55.0 - 2019-03-16

- **NEW:** Made internal changes to allow for portable Windows versions of Buckets to work ([#292](https://github.com/buckets/application/issues/292))
- **FIX:** Debt account payment buckets now correctly show up in the transaction categorization dropdown ([#368](https://github.com/buckets/application/issues/368))
- **FIX:** Fix Uncaught TypeError for old debt payment buckets ([#367](https://github.com/buckets/application/issues/367))
- **FIX:** Fixed bug that prevented importing GnuCash OFX files ([#332](https://github.com/buckets/application/issues/332))
- **FIX:** You no longer have to switch between importing CSV files or QFX/OFX ([#342](https://github.com/buckets/application/issues/342))
- **FIX:** OFX files which lack unique transaction ids can now be imported ([#336](https://github.com/buckets/application/issues/336))

# v0.54.1 - 2019-03-09

- **FIX:** Fix Windows 64-bit installation

# v0.54.0 - 2019-02-28

- **NEW:** Removed Beta preference (since there's now a separate Buckets Beta application)
- **NEW:** Your email address is remembered when you report a bug (so you don't have to enter each time you report a bug).

# v0.53.1 - 2018-12-13

- **FIX:** Fix erroneous SignMismatch error ([#323](https://github.com/buckets/application/issues/323))

# v0.53.0 - 2018-12-12

- **NEW:** Accounts and balances can now optionally be shown in the side bar if you want.  Use the per-budget settings page to toggle.  ([#99](https://github.com/buckets/application/issues/99))
- **NEW:** Total Want is now shown for each bucket group.  ([#274](https://github.com/buckets/application/issues/274))
- **NEW:** This change might annoy you at first, but once you get used to it, you'll like it :)  When entering transactions, the amount now defaults to a **negative** amount since most transactions are expenses.  You can enter positive amounts by clicking the big *minus* button or by entering a negative number.  ([#307](https://github.com/buckets/application/issues/307))
- **NEW:** Money inputs now stay the same width even when doing math inside of them.  Computed values are displayed in a floating tag above the input rather than to the side.
- **FIX:** Fix CSV import error when CSV contains blank header cells.  ([#316](https://github.com/buckets/application/issues/316))
- **FIX:** Top bar expenses are no longer red so that red is reserved for problem-like situations.  ([#291](https://github.com/buckets/application/issues/291))
- **FIX:** Clicking account names now opens up the account details rather than editing the account name.  You can still edit account names by clicking on the name in the details pane.  ([#244](https://github.com/buckets/application/issues/244))
- **FIX:** When importing from YNAB4, you can choose the YNAB4 file or as a convenience to users, any file inside it ([#318](https://github.com/buckets/application/issues/318))

# v0.52.1 - 2018-11-26

- **FIX:** Fixed a bug where calculator wouldn't work if you had whitespace ([#313](https://github.com/buckets/application/issues/313))
- **FIX:** Dutch translation corrections
- **FIX:** French translation corrections

# v0.52.0 - 2018-09-17

- **FIX:** Attempted fix at unreproducible account deletion error. ([#301](https://github.com/buckets/application/issues/301))
- **FIX:** Attempted fix of goal date inconsistency ([#288](https://github.com/buckets/application/issues/288))
- **FIX:** Errors related to entering licenses are better logged now.  ([#229](https://github.com/buckets/application/issues/229))
- **FIX:** OFX files with multiple accounts inside can now be imported. ([#302](https://github.com/buckets/application/issues/302))
- **FIX:** Make sure newly-created budget files end with the correct extension. ([#304](https://github.com/buckets/application/issues/304))
- **FIX:** Fixed bug where tooltip would flicker at the edge of the screenstatus ([#299](https://github.com/buckets/application/issues/299))
- More internal refactoring for mobile apps.

# v0.51.1 - 2018-08-08

- **FIX:** Pressing Enter while editing bucket details will close the details. ([#235](https://github.com/buckets/application/issues/235))
- **FIX:** Fix false warning about using an older version of buckets on a newer budget file. ([#280](https://github.com/buckets/application/issues/280))
- **FIX:** You can now import transactions for off-budget accounts. ([#284](https://github.com/buckets/application/issues/284))

# v0.51.0 - 2018-08-06

- **NEW:** Added some Net Wealth charts ([#171](https://github.com/buckets/application/issues/171))
- **NEW:** When transactions are created for a month other than the one you're looking at, a notification will pop up to let you know that it was successfully created.  ([#283](https://github.com/buckets/application/issues/283))
- **NEW:** Added shortcut keys for going to next and previous month.  Also included them in the Budget, Go To... menu. ([#266](https://github.com/buckets/application/issues/266))
- **NEW:** Using an old version of Buckets to open a newer budget file displays a warning now.  ([#280](https://github.com/buckets/application/issues/280))
- **FIX:** Restored Buckets License bucket for the trial version.  It accidentally got removed a few versions back.
- **FIX:** Fixed a bug so that now, when you change a transaction's date to another month, the transaction will disappear from the current month as it should.  ([#275](https://github.com/buckets/application/issues/275))
- **FIX:** Fixed bug where Linux Beta installations would offer to downgrade to latest non-beta version.  ([#279](https://github.com/buckets/application/issues/279))
- **FIX:** Fewer characters are swallowed when searching on the page. ([#270](https://github.com/buckets/application/issues/270))

# v0.50.0 - 2018-07-30

- **NEW:** Paying off credit cards and some other debt is now easier with the addition of Debt accounts.  ([#277](https://github.com/buckets/application/issues/277))
- More internal refactoring to prepare for mobile apps

# v0.49.0 - 2018-07-16

- **FIX:** Added DD/MMM/YY as date format for CSV importing.  Also made it so you can type in whatever format you want. ([#263](https://github.com/buckets/application/issues/263))
- **FIX:** Fixed a bug that would clear a transaction's income/transfer designation if you changed the amount. ([#265](https://github.com/buckets/application/issues/265))

# v0.48.0 - 2018-07-09

- **NEW:** You can now kick buckets right from the buckets list view. ([#225](https://github.com/buckets/application/issues/225))
- **FIX:** Possible duplicate transaction detection is now limited to transactions that have nearby dates and is expanded to look for transactions in adjacent months.  ([#261](https://github.com/buckets/application/issues/261))

# v0.47.0 - 2018-07-02

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

# v0.46.2 - 2018-06-27

- **FIX:** Fix missing locale bug ([#252](https://github.com/buckets/application/issues/252))

# v0.46.1 - 2018-06-26

- **FIX:** Renamed bucket transaction "Misc" column to "Account" ([#245](https://github.com/buckets/application/issues/245))
- **FIX:** Fixed bug that prevented removing categories while editing a transaction ([#239](https://github.com/buckets/application/issues/239))

# v0.46.0 - 2018-06-25

- **NEW:** Now available in Deutsch!
- **FIX:** Added more verbose logging for Linux file read/write issues, including a message to instruct the user about how to possibly fix the problem. ([#224](https://github.com/buckets/application/issues/224))
- **FIX:** Override number format set in Preferences is now honored ([#237](https://github.com/buckets/application/issues/237))
- Massive code refactoring to get ready for the mobile app.
- Added a little more context for translators.  ([#234](https://github.com/buckets/application/issues/234))

# v0.45.0 - 2018-06-18

- **NEW:** Added a preference for getting Beta releases of Buckets.
- **FIX:** You can now negate values when importing from CSV files.  This allows you to handle banks that list both debits and credits as positive values.  ([#222](https://github.com/buckets/application/issues/222))

# v0.44.2 - 2018-06-04

- **NEW:** When you create a new account, the account's details are shown ([#176](https://github.com/buckets/application/issues/176))
- **FIX:** Fix the bug where a category is removed when editing a transaction in the account view.  ([#217](https://github.com/buckets/application/issues/217))
- **FIX:** Exclude off-budget accounts from analysis ending balance field.  Don't worry, there will be more reports later that include off-budget accounts :) ([#220](https://github.com/buckets/application/issues/220))
- **FIX:** [afcu.com-209 4cf27da] Fixed bank macro bug where a bank's short HTTP-only domain did not properly redirect to the full HTTPS domain.  ([#209](https://github.com/buckets/application/issues/209))
 1 file changed, 1 insertion(+), 1 deletion(-)
- **FIX:** You can now transfer to/from off-budget accounts when making transactions.  ([#213](https://github.com/buckets/application/issues/213))
- **FIX:** Prevent accidentally opening the same file twice (as with a double click) from the starting file-chooser pane ([#211](https://github.com/buckets/application/issues/211))
- **FIX:** You can now unlink accounts from import files so that the next time you import a file for that account, you will be prompted to choose which account the file belongs to.  ([#210](https://github.com/buckets/application/issues/210))
- Internal refactorings to get ready for mobile app

# v0.44.1 - 2018-05-25

- **FIX:** Fix analysis reports so that they no longer include off-budget accounts.  There will be other reports for off-budget accounts.  ([#206](https://github.com/buckets/application/issues/206))
- **FIX:** Handle non-unicode CSV files.  ([#202](https://github.com/buckets/application/issues/202))
- **FIX:** Potential fix for update error on start on Ubuntu ([#207](https://github.com/buckets/application/issues/207))

# v0.44.0 - 2018-05-10

- **NEW:** Buckets is now signed for macOS and Windows!  This means you shouldn't get as many warnings when trying to install it.  ([#150](https://github.com/buckets/application/issues/150))
- **FIX:** Indicate that you might have to download the new version manually ([#203](https://github.com/buckets/application/issues/203))
- Switched out sqlite for sqlite3-offline ([#183](https://github.com/buckets/application/issues/183))

# v0.43.1 - 2018-05-08

- **FIX:** Fix bug preventing the remapping of CSV files ([#199](https://github.com/buckets/application/issues/199))
- **FIX:** Fix for bug with CSV importing where numbers were multiplied by 100 because the chosen language's default number format was not honored. ([#200](https://github.com/buckets/application/issues/200))

# v0.43.0 - 2018-05-07

- **NEW:** You can now choose a currency symbol to be displayed with the top summary numbers.  Go to the new *Settings* tab (look on the bottom left corner) and type in your favorite symbol. ([#107](https://github.com/buckets/application/issues/107))
- **FIX:** Fixed alignment on Buckets table headings.  ([#193](https://github.com/buckets/application/issues/193))
- **FIX:** Fix CSV import bug ([#190](https://github.com/buckets/application/issues/190))
- **FIX:** Dates are properly formatted according to your chosen locale again.  ([#186](https://github.com/buckets/application/issues/186))
- **FIX:** "Save X by depositing Z/mo" buckets no longer keep wanting after the goal has been reached ([#192](https://github.com/buckets/application/issues/192))
- **FIX:** When launching from the command line, look for custom BUCKETS_LANG environment variable instead of LANG.
- **FIX:** Fix no-internet false positive error ([#195](https://github.com/buckets/application/issues/195))
- **FIX:** The Recurring Expenses month slider is no longer impossible to use ([#188](https://github.com/buckets/application/issues/188))
- **FIX:** Fix Starting over bug when you want to delete everything, including buckets ([#191](https://github.com/buckets/application/issues/191))

# v0.42.0 - 2018-04-30

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

# v0.41.0 - 2018-04-24

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

# v0.40.1 - 2018-03-29

- **FIX:** Let us check for updates again if an update fails to download.  ([#Qtufqzis](https://trello.com/c/Qtufqzis))
- **FIX:** Fix YNAB4 import error for transactions with mixed-sign categorizations ([#KiDm6dZS](https://trello.com/c/KiDm6dZS))

# v0.40.0 - 2018-03-26

- **NEW:** Added a 'Start Over' tool.  ([#gMedmoLD](https://trello.com/c/gMedmoLD))
- **FIX:** Letters are no longer eaten when writing a note on *any* object.  ([#ZQa6alQo](https://trello.com/c/ZQa6alQo))
- **FIX:** You can choose a number format independent of your language. ([#ZaP9MCUO](https://trello.com/c/ZaP9MCUO))

# v0.39.2 - 2018-03-23

- **FIX:** Fix white on white text in transaction dropdown on Windows ([#Cb24GGRR](https://trello.com/c/Cb24GGRR))

# v0.39.1 - 2018-03-22

- **FIX:** Fixed a bug in CSV importing ([#2KYzgBet](https://trello.com/c/2KYzgBet))
- **FIX:** Sync time range alert is not correct.

# v0.39.0 - 2018-03-21

- **NEW:** It's now much easier to record transfers between accounts.  When creating a transaction, simply mark it as a transfer and choose the account the funds are coming from or going to.  ([#W1s6v7WU](https://trello.com/c/W1s6v7WU))
- **NEW:** The Buckets tab is cleaner (less busy) through the following changes.  The balance of each bucket is now the first number.  "Out" and "Transfer" columns have been combined into a single "Activity" column.  When there is an amount in the "In/Out" field, the current and future balance no longer make the table expand horizontally. The heading labels are repeated for each bucket group.  Effective balance is no longer shown when in debt.  ([#VSy1vj99](https://trello.com/c/VSy1vj99), [#6T7u0kWO](https://trello.com/c/6T7u0kWO))
- **NEW:** You can now categorize transactions as you enter them, instead of having to categorize them after adding them.
- **NEW:** The Recurring Expenses analysis chart now remembers the time period you chose. ([#2yalBubk](https://trello.com/c/2yalBubk))
- **NEW:** Names of translation contributors appear in the source file of each language.  ([#1s7TvSdi](https://trello.com/c/1s7TvSdi))
- **FIX:** For labels with a bright yellow background, black text is now used instead of white.  In other words, you can read the words now :)
- **FIX:** Simple categorization is preserved after editing transactions.  ([#L7jULmPb](https://trello.com/c/L7jULmPb))
- **FIX:** Only list recently-opened files that still exist.  ([#OvGiy3pc](https://trello.com/c/OvGiy3pc))
- **FIX:** Refunds/returns now add money to the 'Activity' column rather than the 'Rain' column on the Buckets view.  ([#zmXmsVbp](https://trello.com/c/zmXmsVbp))

# v0.38.2 - 2018-03-15

- **FIX:** Don't overwrite non-null account balances to fix daylight saving problem.

# v0.38.1 - 2018-03-14

- **FIX:** Prevent NULL amounts in transactions. ([#FJHZHCxx](https://trello.com/c/FJHZHCxx))

# v0.38.0 - 2018-03-14

- **FIX:** Handle daylight saving time ([#9MfU7pAj](https://trello.com/c/9MfU7pAj))

# v0.37.0 - 2018-03-12

- **FIX:** Several visual changes.  The Accounts view uses horizontal space better.  The Month-to-Month analysis view no longer includes the year on the first date.  ([#4MgmeJq9](https://trello.com/c/4MgmeJq9), [#5oypmRTm](https://trello.com/c/5oypmRTm), [#Ljy70cM6](https://trello.com/c/Ljy70cM6))
- **FIX:** Rain tooltip no longer has faded cents. ([#TlvT3o2a](https://trello.com/c/TlvT3o2a))
- **FIX:** When downloading an update, release notes stay visible. ([#N6ZbcQvk](https://trello.com/c/N6ZbcQvk))

# v0.36.0 - 2018-03-06

- **NEW:** Numbers are localized according to language now (i.e. in Portuguese and Spanish the decimal separator is now a comma) ([#0iXa6tJR](https://trello.com/c/0iXa6tJR))
- **FIX:** It's more obvious how to close notes. ([#2qffJJW9](https://trello.com/c/2qffJJW9))
- **FIX:** Emoji in Bucket names no longer causes height problems in macOS ([#XTu7f4EW](https://trello.com/c/XTu7f4EW))
- **FIX:** Recurring expense chart labels aren't cut off anymore.  ([#dl6Rupnn](https://trello.com/c/dl6Rupnn))
- **FIX:** Fixed an internal input warning. ([#LaBarRXx](https://trello.com/c/LaBarRXx))
- **FIX:** If there's no internet connection, an error about not being able to update is no longer displayed on start ([#hjnugHpN](https://trello.com/c/hjnugHpN))

# v0.35.1 - 2018-02-28

- **FIX:** Another fix for another kind of YNAB4 import failure.  ([#MpmFZutK](https://trello.com/c/MpmFZutK))

# v0.35.0 - 2018-02-28

- **NEW:** Added *Start with a template* button for getting started with Buckets.  ([#2kWWcMGa](https://trello.com/c/2kWWcMGa))
- **FIX:** Handle CSV files that don't have a consistent number of columns throughout.  ([#TvFClGGM](https://trello.com/c/TvFClGGM))
- **FIX:** Fixed a bug when importing YNAB4 files with transactions that are split, but not split into categories ([#rJgT119e](https://trello.com/c/rJgT119e))

# v0.34.0 - 2018-02-23

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

# v0.33.0 - 2018-02-08

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

# v0.32.0 - 2018-02-02

- **NEW:** You can delete bucket transactions (Issue [#q2PpU2iV](https://trello.com/c/q2PpU2iV))
- **NEW:** Added a 'Quit' option for Windows/Linux users.  ([#XjHhptE6](https://trello.com/c/XjHhptE6))
- **FIX:** Budget always opened to the month before the current month, by default.  Now it opens to the current month.  ([#tE6BlTgh](https://trello.com/c/tE6BlTgh))
- **FIX:** You can now adjust the Buckets License amount so that different currencies can be made to work ([#j8rA12Fu](https://trello.com/c/j8rA12Fu))
- **FIX:** Fixed math being wrong on money inputs ([#wtnk1A92](https://trello.com/c/wtnk1A92))
- **FIX:** When there are no recurring expense buckets, the analysis page no longer looks like a broken page.  ([#6snqIshs](https://trello.com/c/6snqIshs))
- **FIX:** Posted date of newly created transactions will now always be (by default) in the month you are looking at.  ([#LauMJXLI](https://trello.com/c/LauMJXLI))

# v0.31.2 - 2018-01-30

- **FIX:** Fixed *Used in future* to not include kicked buckets.
- **FIX:** Fixed future rain missed update with multiple windows ([#dXwraTOl](https://trello.com/c/dXwraTOl))
- Moved to Trello for issue/bug tracking ([#JeaRIFN9](https://trello.com/c/JeaRIFN9))

# v0.31.1 - 2018-01-29

- **FIX:** Fix error in want-to-buy message

# v0.31.0 - 2018-01-29

- **NEW:** Added a transaction export tool.  (Issue [#28](https://github.com/buckets/application/issues/28))
- **NEW:** Rain in the current month now takes into account any amount spoken for in future months.  This allows for budgeting future months.  (Issue [#38](https://github.com/buckets/application/issues/38))
- **NEW:** When reopening buckets, the last set of opened windows is restored.  (Issue [#59](https://github.com/buckets/application/issues/59))
- **FIX:** Another attempt at the off by one problem.  (Issue [#40](https://github.com/buckets/application/issues/40))

# v0.30.0 - 2018-01-25

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

# v0.29.0 - 2018-01-22

- **NEW:** Added a preference to disable money animations
- **NEW:** CSV importing is now supported.  (Issue [#5](https://github.com/buckets/application/issues/5))

# v0.28.0 - 2018-01-19

- **NEW:** Now there's a way to submit bugs from within Buckets. (Issue [#43](https://github.com/buckets/application/issues/43))

# v0.27.1 - 2018-01-18

- **NEW:** Added some options in the Help menu to allow for more verbose log reports.
- **FIX:** Fix some database schema issues.

# v0.27.0 - 2018-01-17

- **FIX:** Check for updates, and version information is now available for Windows and Linux users.  (Issue [#43](https://github.com/buckets/application/issues/43))
- **FIX:** Fix a bug that prevented adding transactions in the account view.  (Issue [#44](https://github.com/buckets/application/issues/44))
- **FIX:** Make update window not be so small (especially on Windows) (Issue [#45](https://github.com/buckets/application/issues/45))

# v0.26.0 - 2018-01-17

- **NEW:** Added Amazon reconciliation tool.  (Issue [#33](https://github.com/buckets/application/issues/33))
- **FIX:** Database migrations are less flakey now.

# v0.25.1 - 2018-01-15

- **FIX:** Hopefully fix issue [#39](https://github.com/buckets/application/issues/39) so that importing from YNAB4 works.
- **FIX:** Make month selector more resilient to different timezones.  (Issue [#40](https://github.com/buckets/application/issues/40))

# v0.25.0 - 2018-01-15

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

# v0.24.0 - 2018-01-08

- **FIX:** You can no longer make 0-amount bucket transactions (Issue [#22](https://github.com/buckets/application/issues/22))
- **FIX:** Include more information to distinguish between similar accounts when using SimpleFIN Sync
- **FIX:** Clarify that most U.S. banks are supported by SimpleFIN (Issue [#24](https://github.com/buckets/application/issues/24))
- NEW: Accounts can now be closed, and you can shoot yourself in the foot by completely deleting accounts and all linked transactions.  You're welcome.  (Issue [#2](https://github.com/buckets/application/issues/2))

# v0.23.0 - 2018-01-05

- **FIX:** Account balance table aligns balance to the right.
- **FIX:** Report bug feature now works on Windows (Issue [#11](https://github.com/buckets/application/issues/11))
- **FIX:** Fix YNAB importing for budgets that have categories without subcategories. (Issue [#12](https://github.com/buckets/application/issues/12))
- NEW: When updating Buckets, release notes are shown in the notification window, a progress bar shows progress and you can opt to skip a version to prevent more notifications. (Issues [#3](https://github.com/buckets/application/issues/3), [#9](https://github.com/buckets/application/issues/9))
- NEW: Under *Analysis* the *Regular Expenses* section includes helpful number line charts and groups buckets according to whether expenses appear monthly v. yearly (or somewhat yearly) and groups them by relative budgeted amount.  In short, it's prettier :)

# v0.22.1 - 2018-01-02

- **FIX:** Fix [issue #8](https://github.com/buckets/application/issues/8) by allowing users to select directories and files for import

# v0.22.0 - 2017-12-29

- NEW: Added first (experimental) version of creating macros to download transaction data from banks automatically.  (Not yet translated into Spanish).

# v0.21.0 - 2017-11-17

- **FIX:** Improved the explanation of what rain is
- NEW: Switch from bucketsisbetter.com to budgetwithbuckets.com

# v0.20.0 - 2017-11-06

- **FIX:** Light grey on charts is now less light and more visible
- **FIX:** When turning a bucket from a specialized type back into a regular bucket, the rain is now reported correctly (as zero)
- **FIX:** Set default save directory to ~/Documents (or OS equivalent) so that the default is no longer /
- NEW: All budget-related menu options have been moved to a single 'Budget' menu (rather than being dispersed over several other menus)
- NEW: Buckets can now import You Need a Budget (YNAB) v4 budget files.

# v0.19.0 - 2017-11-03

- **FIX:** Translate the preferences page
- NEW: Buckets files format is documented
- NEW: Auto-updating is now supported on Linux for AppImage installs
- NEW: Reduce license price from $40 to $29 (and intro price from $20 to $15)

# v0.18.0

- NEW: Buckets is now available in Spanish!

# v0.17.0 - 2017-09-12

- **FIX:** Fixed a bug that prevented actually linking SimpleFIN accounts
- NEW: Added better logging for times where there are silent errors

# v0.16.0 - 2017-09-01

- **FIX:** Got rid of scary balance-mismatch warnings that weren't actually actionable.  And a better explanation of what mismatches mean is included.
- **FIX:** Now, when you sync transactions, it will only sync the current month
- **FIX:** The update process is even *more* clear.

# v0.15.0

- **FIX:** If you try to open/create a file that's unreadable and error is displayed instead of failing silently

- NEW: You can now click 'Make it Rain' as many times as you want.  Each bucket will only take what it needs *per month*


- **FIX:** Fixed bug where 'Duplicate Window' would sometimes throw an error.
- **FIX:** Recurring expense report doesn't report false information for newly-made buckets anymore
- NEW: Added new charts to bucket information pages
- NEW: You can now explicitly mark bucket transactions as transfers


# v0.14.0

- **FIX:** When updating an account balance in a month that isn't the current month, it now does the right thing.
- **FIX:** Removed the mystery of what's going on during update download/install.
- NEW: Added a bucket expense analysis section.


# v0.13.0

- NEW: Added a new 'Analysis' section with helpful month-to-month and year-to-year charts
- NEW: Added *Chat with Matt* navigation item


# v0.12.0

- NEW: Now you can get instant help with the 'Chat...' option in the Help menu.
- NEW: Added *Effective Balance* column to buckets for when there are buckets in debt (so you don't think you have more money than you do).
- NEW: Windows are labeled with the filename now
- NEW: Linux installs will now be notified of updates, too


# v0.11.0

- **FIX:** Style fixes and extra tooltip helps
- **FIX:** Some menu items are disabled/enabled now when the context justifies it.
- **FIX:** Fixed bug where categorizing with math would sometimes make too many rows
- NEW: Categorizing is cleaner now
- NEW: Started changelog.
- NEW: Table rows are now highlighted when you hover over them
- NEW: You can now import OFX/QFX files


