# School_District_Analysis
Module 4
## Overview of PyCity Schools Analysis
The client wanted a comprehensive analysis on the school district's reading and math scores for each high school. Due to scpeculation of academic dishonesty in the 9th grade class at Thomas High School (THS) for reading and math, the client wanted an analysis without those scores. The analysis on the school district's data for reading, math, and overall scores were reconfigured without the potential dishonest scores. Data is organized into top and bottom five schools based on overall passing percentage, average math and reading scores from each school, and scores by spending per student, school size, and school type.

## Results: Using bulleted lists and images of DataFrames as support, address the following questions.
### How is the district summary affected?
  * The data show a 0.1% decrease in the average math score, bringing the score down to 78.9%. The average reading score reamains the same. The percentage for passing math decreases by 0.2% bringing it to 74.8%. The percentage for passing reading is brought down to 85.7%, which is a 0.3% decrease. The overall passing percentage decreases by 0.1%, dropping from 65% to 64.9%.
  * **All District Summary DataFrame**  <br />
  ![all_district_summary_df](https://user-images.githubusercontent.com/98570777/165002360-74f263c8-436f-4212-9f6e-eab704cc878a.png)

  * **District Summary DataFrame - omitted THS 9th grade data**  <br />
  ![district_summary_df_no_9_THS](https://user-images.githubusercontent.com/98570777/165002373-b09781e5-eb59-4dff-92f8-15d75e0aa7df.png)
  
### How is the school summary affected?
  * The data show an overall decrease in rates of students passing math, reading, and math and reading combined when THS 9th graders' scores were taken out of the analysis. Percentage passing math decreases by 26.4%, percentage passing reading decreases by 27.6%, and percentage passing overall decreases by 25.8%.
  * **All School Summary DataFrame**  <br />
  ![all_school_summary_df](https://user-images.githubusercontent.com/98570777/165003255-f72452f9-394d-4f94-b52f-49ec8bc5d5a9.png)

  * **School Summary DataFrame - omitted THS 9th grade data** <br />
  ![school_summary_no_9_THS](https://user-images.githubusercontent.com/98570777/165003273-35dcb59f-721f-4b7d-a4a0-441d387a3da7.png)
  
### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
  * The performance of THS compared to the other four top schools is quite similar. At first glance, you would not be able to tell the numbers are different. The only slight difference is the approximately 0.3% decrease in % passing math, % passing reading and % overall passing after the THS 9th grader data is omitted.
  * **Original Top Five Schools**<br />![top_schools_original](https://user-images.githubusercontent.com/98570777/165020982-c84bb270-eb38-4a68-89c1-57b06238157c.png)

  * **Top Five Schools with Omitted THS 9th Grade Data**<br />![top_schools_no_9_THS](https://user-images.githubusercontent.com/98570777/165021285-1492ea22-ab3b-437f-be77-7c5461229bfd.png)


### How does replacing the ninth-grade scores affect the following:
   * ### Math and Reading Scores by Grade
     *  The only change in both math and reading scores by grade is the absensce of the 9th grade value for THS.
     * **Math Scores by Grade** followed by **Math Scores by Grade, no THS 9th Grade Data** <br />
    ![all_math_score_by_grade](https://user-images.githubusercontent.com/98570777/165005488-0a51bbf3-3ddc-4d9c-9af6-567b68d2571d.png)![math_score_by_grade_no_9_THS](https://user-images.githubusercontent.com/98570777/165005721-a34941d6-a1ee-423c-9bb1-bb9f2b5ecc12.png)

     * **Reading Scores by Grade** followed by **Reading Scores by Grade, no THS 9th Grade Data** <br />
    ![all_reading_score_by_grade](https://user-images.githubusercontent.com/98570777/165005500-43e9d10f-2eae-4769-9714-f237109b94ce.png)![reading_score_by_grade_no_9_THS](https://user-images.githubusercontent.com/98570777/165006301-5919e3d7-7260-4b04-90a3-d4a06b98ddde.png)


   * ### Scores by school spending
     * There were three changes to the Spending Range (Per Student) row "$631-645" The percentage passing math dropped from 73.5% to 66.2%; the percentage passing   reading dropped from 84.4% to 77.5%; and the percentage overall passing dropped from 62.9% to 56.4%. The lowest percentage passing overall is 53.5% which is in the highest spending range in both data sets, $646-675 and $646-655.
     * **Original** <br /> ![all_scores_by_school_spending](https://user-images.githubusercontent.com/98570777/165018358-99aa7146-3a5b-45ae-a8da-3cca91d1e050.png)
     * **Omitted THS 9th Grade Data** <br />![scores_by_school_spending_no_9_THS ](https://user-images.githubusercontent.com/98570777/165008726-b1bc582d-439d-47a6-8ef5-af8100ff21a3.png)


   * ### Scores by school size
     * When 9th grade THS data is omitted, the percentages in passing math, reading and overall passing scores in the "Medium (1000-1999)" school size row drop by 5%. 
     * **Original** <br />![all_scores_by_school_size_new](https://user-images.githubusercontent.com/98570777/165018910-0ce83eb8-07f9-488d-99d2-b2e446905550.png)
     * **Omitted THS 9th Grade Data** <br />![scores_by_school_size_no_9_THS](https://user-images.githubusercontent.com/98570777/165008780-2602bf82-05f1-484a-99e5-7f089b4757c5.png)

   * ### Scores by school type
     * When 9th grade THS data is omitted, the percentages in passing math, reading and overall passing scores in the "Charter" row drop by 3%.
     * **Original** <br />![all_score_by_school_type](https://user-images.githubusercontent.com/98570777/165008809-a1172033-5a2c-4b6e-95c6-3ef6f3541d04.png)

     * **Omitted THS 9th Grade Data** <br />![score_by_school_type_no_9_THS](https://user-images.githubusercontent.com/98570777/165008826-48864030-f4e6-4942-87f5-cb969299ec02.png)


## Summary: 
### Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
* District data summary: This data show there was a slight decrease in the average math score while the average reading score reamains the same. The percentage for passing math, reading and overall passing decreases only slightly as well. 
* Scores by school spending: There were three changes to the Spending Range (Per Student) row "$631-645" The percentage passing math dropped from 73.5% to 66.2%; the percentage passing reading dropped from 84.4% to 77.5%; and the percentage overall passing dropped from 62.9% to 56.4%. The lowest percentage passing overall is 53.5% which is in the highest spending range in both data sets, $646-675 and $646-655.
* Scores by school size: With the omitted data, the percentages in passing math, reading and overall passing scores in the "Medium (1000-1999)" school size row drop by 5%.
  * The small changes to the results could be due to the large sample size that was being worked with. The small amount of data taken out was not enough to affect the whole.
* Thomas High School data summary: These results show a much more substantial decrease in rates of the two datasets. About a 25% decrease for overall percentage passing, percentage passing math and percentage passing reading. 
  * The large rate of decrease could be due to the absence of 9th grade data. With a smaller sample size, the smallest changes can affect the whole at a much larger scale. 
