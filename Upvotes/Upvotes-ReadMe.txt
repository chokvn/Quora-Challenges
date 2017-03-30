Quora Challenge - Upvotes

*Description
The upvotes challenge represents the development of a metric to monitor the exposure the website receives. The ability to
count the consecutive segments where the upvotes trend is non-decreasing or non-increasing can translate to determining an
increased or decreased exposure and reaction to the site as related to a catalyst. This catalyst can be attributed to many
factors such as peer to peer recommendation, increase in content, implementation of advertisement, and other changes to the
website itself. This tool can be performed on a singular question or a group of questions(by topic or the whole website
itself) for analyzing specific and broader changes respectively.

*Personal Opinion
My first thoughts when determining the utility of this analysis relate to the use of the result as a metric for A/B testing.
As an example, a layout change to determine which setup caters better to users can be tested to two groups of people over a
period of time and monitored for more non-decreasing segments versus the previous or control layout. It is likely that an
effective layout change will result in longer non-decreasing segments compared to the unchanged layout. However, there are
some shortcomings with this as a metric for any form of testing. While it checks for non-decreasing and non-increasing
consecutive days, it does not take into account the magnitude of upvotes per day and if both the control and variable layouts
have similar patterns, the variable or changed layout could have the same pattern but with a higher amount of net upvotes per
day by comparison. Assuming more upvotes means more exposure or effectiveness of the layout to users, using the results from
this program may not sufficiently reflect the benefits.

*Method
The method employed to create this program was to create the window with size determined by input and analyze the window
as it "slided" through the list of upvotes one by one. The analysis for this window determines whether the first two numbers
are in an increasing or decreasing pattern. This increases the count for non-decreasing or non-increasing respectively.
Afterwards, the next numbers are analyzed by adding the next number to the sequence and checked for the same non-decreasing
or non-increasing nature. When the sequence stops in one of the two manners, the second number of the sequence is pitted
against the third number and the pattern continues until they reach the last two numbers.

*Improvement Ideas
