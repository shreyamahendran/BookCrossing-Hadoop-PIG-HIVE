# BookCrossing-Hadoop-PIG-HIVE
Analyze BookCrossing Dataset using PIG (and HIVE too)

BookCrossing is a social networking site celebrating literature and a place where books get a new life. 
\n Their MOTTO : “Label. Share. Follow”

BookCrossing is the act of releasing your books "into the wild" for a stranger to find, or via "controlled release" to another BookCrossing member, and tracking where they go via journal entries from around the world.

We have used BX-Books and BX-Book-Ratings for our analysis.
Collected by Cai-Nicolas Ziegler in a 4-week crawl (August / September 2004) from the Book-Crossing community with kind permission from Ron Hornbaker, CTO of Humankind Systems. Contains 278,858 users (anonymized but with demographic information) providing 1,149,780 ratings (explicit / implicit) about 271,379 books.
\n You can find the dataset here : http://www2.informatik.uni-freiburg.de/~cziegler/BX/

BX-Books:
Books are identified by their respective ISBN. Invalid ISBNs have already been removed from the dataset. 
Moreover, some content-based information is given (`Book-Title`, `Book-Author`, `Year-Of-Publication`, `Publisher`), obtained from Amazon Web Services. Note that in case of several authors, only the first is provided. URLs linking to cover images are also given, appearing in three different flavours (`Image-URL-S`, `Image-URL-M`, `Image-URL-L`), i.e., small, medium, large. These URLs point to the Amazon web site. These URL columns have hot been used by us.

BX-Book-Ratings:
Contains the book rating information. Ratings (`Book-Rating`) are either explicit, expressed on a scale from 1-10.
\n higher values denoting higher appreciation), or implicit, expressed by 0.
