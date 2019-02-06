I am using data that New York city has published on SAT scores and have combined the following datasets into a single, clean, Pandas Dataframe:

    SAT scores by school -- SAT scores for each high school in New York City.
    School attendance -- attendance information on every school in NYC.
    Class size -- class size information for each school in NYC.
    AP test results -- Advanced Placement exam results for each high school. Passing AP exams can get you college credit in the US.
    Graduation outcomes -- percentage of students who graduated, and other outcome information.
    Demographics -- demographic information for each school.
    School survey -- surveys of parents, teachers, and students at each school.

New York City has a significant immigrant population, and is very diverse, so comparing demographic factors such as race, income, and gender with SAT scores is a good way to figure out if the SAT is a fair test. If certain racial groups consistently performed better on the SAT, we would have some evidence that the SAT is unfair, for example.

Since we're interested in exploring the fairness of the SAT, finding that demographic factors like race and gender are strongly positively or negatively correlated with SAT scores would be an interesting result that merited investigation. For example, if men tended to score more highly on the SAT, it would indicate that the SAT is potentially unfair to women.

We can use the Pandas corr method to find correlations between columns in a Dataframe. The result of the method is a Dataframe where each column and row index is the name of a column in the original dataset.
