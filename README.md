# Tech Challenge

## Setup

- Run `npm install`
- Run `npm start`

`neutrinojs` will set up a React environment on `http://localhost:5000` for you

## Task 1 - Display Trades in a list

Build a view that displays trade data in a list form.

You'll need to fetch the trade data from the end point `http://localhost:3000/trades`, then render each of the "trade objects" in a list.

Here are the fields we want to be displayed from each "trade object":

- `book_name`
- `cancelled`
- `end_date`
- `matched`
- `product_name`
- `side`
- `start_date`
- `time_created`
- `trade_date`
- `trade_display_volume` (rounded to the nearest integer)
- `trade_price` (rounded to 2 decimal places)

These fields are just alphabetised - you can display the information in any order or way that you wish; as long as all the information is visible and is organised in a way that makes sense.

## Task 2 - Display extra information for each Trade

Each Trade in the list has `child_trade_set` data.

The traders want to be able to toggle the visibility of each individual `child_trade_set` data within the list. Extend the current functionality of the list to allow this information to be conditionally displayed.

Here are the fields we want to be displayed from each "trade object"'s `child_trade_set`'s "child trade object":

- `end_date`
- `price` (rounded to 2 decimal places)
- `side`
- `start_date`
- `trade_display_volume` (rounded to the nearest integer)
- `product_name` (inherited from parent object)

## Task 3 - Display total and average for all trades

In a fixed section above the list, display the total and average of all "trade object"s `trade_price` fields. These values should be rounded to 3 decimal places after the calculations have been performed.
