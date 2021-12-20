# School-District-Analysis-in-Jupyter-Labs
School District Analysis on Test Scores and Funding in Jupyter Labs with Pandas

## Overview of Project

Create a high-level snapshot of the district's key metrics and key metrics for each school, presented in a table format. Additionally repeat the analysis with Thomas High School 9th grader testing scores removed. 

## Results

### How is the district summary affected?
Since the total student count was 39169 and the Thomas High School 9th grade count was 461 (~1.12% of the total count) the average scores and the overall passing percentage largely remained unchanged. There was one exemption, the reading passing percentage was decreased by 11 points (from 97.0 to 86.0).

![This is an image](/Resources/district_summary.png)

With Thomas High School ninth graders’ scores removed.

![This is an image](/Resources/district_summary_mod.png)

### How is the school summary affected?
- This is where we see the sharpest differences in passing percentages with about 26 point drop in passing percentages once the 9th graders’ score are removed. 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
The large drop in passing percentages dropped Thomas High School from being one of the leading charter schools in the district to being the charter school with the worst test scores.

![This is an image](/Resources/per_school_ranked.png)

With Thomas High School ninth graders’ scores removed.

![This is an image](/Resources/per_school_ranked_mod.png)

### How does replacing the ninth-grade scores affect the following:

#### Math and reading scores by grade: 
The way we formatted the DataFrames to show math and reading scores to show by grade, allows us to see that the Thomas 9th graders scores are well within the range of scores from other 9th graders from other schools.

![This is an image](/Resources/by_grade.png)

The format also limits seeing the overall averages by grade.

#### Scores by school spending
An interesting overall trend is the schools that spend less per capita tend to have higher overall scores and passing percentages. Thomas High School fell in the $630-644 range, which saw no change in test averages but about a 7 point drop in passing percentages.

![This is an image](/Resources/by_spending.png)

With Thomas High School ninth graders’ scores removed.

![This is an image](/Resources/by_spending_mod.png)

#### Scores by school size
- Smaller school size tended to have higher overall test scores.

![This is an image](/Resources/by_size.png)

With Thomas High School ninth graders’ scores removed, we saw a similar drop in passing percentage, and very little effect on averages.

![This is an image](/Resources/by_size_mod.png)

#### Scores by school type
- Charter schools, who also tending to be smaller in size and spend less per capita, showed higher overall test scores and passing percentages.

![This is an image](/Resources/by_type.png)

With Thomas High School ninth graders’ scores removed, we saw a similar drop in passing percentage, and again a very little effect on averages.

![This is an image](/Resources/by_type_mod.png)

## Summary

Four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs:
Passing percentages were decreased 4-7% regardless of groupby category
The largest changes occurred when analyzing the passing percentages of Thomas High School itself. Reasonably due to the fact that the 9th graders make up a larger portion of the total count.
Score Averages largely stayed the same due to the small percentage the Thomas High School 9th graders were compared with the total student count of the district.
The charter school ranking was greatly effected once the 9th graders scores were removed. Thomas High School dropped to be charter school with the worst overall passing percentage.
