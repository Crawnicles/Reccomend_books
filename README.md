# Reccomend_books
A program using Goodreads data to suggest books to read

# Steps

## Download book data
* Go to https://sites.google.com/eng.ucsd.edu/ucsdbookgraph/books
* Download book data from https://drive.google.com/uc?id=1LXpK1UfqtP89H1tYy0pBGHjYk8IhigUK

## Download interaction data
* Go to https://sites.google.com/eng.ucsd.edu/ucsdbookgraph/shelves
* Download https://drive.google.com/open?id=1zmylV7XW2dfQVCLeg1LbllfQtHD2KUon
* Download https://drive.google.com/uc?id=1CHTAaNwyzvbi1TR08MJrJ03BxA266Yxr

## Using the Data

1) Search For Books
2) Create Book List
3) Recommend Books

### Search Engine

Creating a Term Frequency Matrix - takes all the unique words across all titles and turns them into a column in the Matrix

Go through each title - if the word exists in the title, add a 1

Rows are the book titles
Columns are the terms

Inverse Document Frequency - make words that appear infrequently more meaningful.
Log(number_of_titles / number_of_titles_word_appears)

Term Frequency matrix * Inverse Document Frequency matrix

