# PocketSort

PocketSort is a small personal expense tracker that helps answer a familiar question: where did my money go this month?

## Run it

Open `index.html` in a current web browser. No installation, account, server, or physical device is required. Entries and category budgets are stored in that browser's local storage and are not uploaded. Use **Load sample** to explore the dashboard; sample data replaces entries for the selected month, so export any month you want to keep before loading samples.

## Features

- Monthly summary and ranked spending categories
- Add, edit, delete, search, and filter transactions
- Monthly category budgets with 80% warning and over-budget indicators
- Export the selected month's transactions to CSV
- Monthly insights and an in-app explanation of the algorithms
- Responsive layout for phone and desktop browsers

## DSA used

- A hash map groups transactions by category and adds amounts in one pass: O(n), where n is the number of transactions.
- Merge sort orders category totals from largest to smallest: O(k log k), where k is the number of categories.
- Totals and average are calculated from the selected month's transactions.

## Honest portfolio description

After reviewing and understanding the code, the developer can describe this as a browser-based expense tracker with category budgets and spending insights. It uses JavaScript, local storage, hash-map aggregation, and merge sort. Do not claim independent authorship of code that was not personally built or understood; customize it, trace the algorithm, and be ready to explain the implementation.

## Deploy

This is a static, dependency-free site and can be hosted by any static hosting service. Upload the folder contents, with `index.html` at the site root. No backend or paid service is needed for the static app. Live hosting still requires an account or a connected project on a hosting provider.
