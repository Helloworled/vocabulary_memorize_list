This project is a text constructor based on parsed csv data

description:

the project will be hosted on a github page. the csv will also exist in the repo and loaded alongside the page.

data:

csv file contains 14 colums, every row (except the first row) have a serial number, every colum (including the serial number colum) have a alphabetical id (A-N).

csv file loaded from a remote address alongside with the page

sample data:

| A  | B         | C       | D  | E  | F  | G  | H  | I  | J  | K | L | M | N |
| -- | --------- | ------- | -- | -- | -- | -- | -- | -- | -- | - | - | - | - |
| 1  | 2026/9/1  | String  | 1  | 1  | 1  | 0  | 0  | 0  | 0  | 0 | 0 | 0 | 0 |
| 2  | 2026/9/2  | String  | 2  | 2  | 2  | 1  | 0  | 0  | 0  | 0 | 0 | 0 | 0 |
| 3  | 2026/9/3  | String  | 3  | 3  | 3  | 2  | 1  | 0  | 0  | 0 | 0 | 0 | 0 |
| 4  | 2026/9/4  | String  | 4  | 4  | 4  | 3  | 2  | 0  | 0  | 0 | 0 | 0 | 0 |
| 5  | 2026/9/5  | String  | 5  | 5  | 5  | 4  | 3  | 1  | 0  | 0 | 0 | 0 | 0 |
| 6  | 2026/9/6  | String  | 6  | 6  | 6  | 5  | 4  | 2  | 0  | 0 | 0 | 0 | 0 |
| 7  | 2026/9/7  | String  | 7  | 7  | 7  | 6  | 5  | 3  | 0  | 0 | 0 | 0 | 0 |
| 8  | 2026/9/8  | String  | 8  | 8  | 8  | 7  | 6  | 4  | 1  | 0 | 0 | 0 | 0 |
| 9  | 2026/9/9  | String  | 9  | 9  | 9  | 8  | 7  | 5  | 2  | 0 | 0 | 0 | 0 |
| 10 | 2026/9/10 | String  | 10 | 10 | 10 | 9  | 8  | 6  | 3  | 0 | 0 | 0 | 0 |
| 11 | 2026/9/11 | String  | 11 | 11 | 11 | 10 | 9  | 7  | 4  | 0 | 0 | 0 | 0 |
| 12 | 2026/9/12 |  String | 12 | 12 | 12 | 11 | 10 | 8  | 5  | 0 | 0 | 0 | 0 |
| 13 | 2026/9/13 |  String | 13 | 13 | 13 | 12 | 11 | 9  | 6  | 0 | 0 | 0 | 0 |
| 14 | 2026/9/14 |  String | 14 | 14 | 14 | 13 | 12 | 10 | 7  | 0 | 0 | 0 | 0 |
| 15 | 2026/9/15 |  String | 15 | 15 | 15 | 14 | 13 | 11 | 8  | 0 | 0 | 0 | 0 |
| 16 | 2026/9/16 |  String | 16 | 16 | 16 | 15 | 14 | 12 | 9  | 1 | 0 | 0 | 0 |
| 17 | 2026/9/17 |  String | 17 | 17 | 17 | 16 | 15 | 13 | 10 | 2 | 0 | 0 | 0 |
| 18 | 2026/9/18 |  String | 18 | 18 | 18 | 17 | 16 | 14 | 11 | 3 | 0 | 0 | 0 |
| 19 | 2026/9/19 |  String | 19 | 19 | 19 | 18 | 17 | 15 | 12 | 4 | 0 | 0 | 0 |
| 20 | 2026/9/20 |  String | 20 | 20 | 20 | 19 | 18 | 16 | 13 | 5 | 0 | 0 | 0 |

index.html:

html page displays: a button (to copy content in textbox to clipboard), a textbox, a table area that renders the content of the csv data.

minimum css needed

logic:

init an array for storing numbers.

on page load: get the current date (YYYY/MM/DD, UTC+8), query colum B where the same data (string of date), save number in colum A to array. get number in colum G, H, J, K, L, M, N and save them to array.

query string data in colum C for all colum A equals saved numbers, display the strings in the textbox.
