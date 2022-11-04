# Analysis of ACT 2017 - 2022


### Background
In October 2022, ACT reported that the 2022 average ACT score has declined to the lowest level in more than 30 years. The report indicated that high school students are not meeting college-readiness benchmarks, signaling systemic failures in the American education that were exacerbated by the pandemic. ([*source*](https://leadershipblog.act.org/2022/10/GradClassRelease2022.html))

The ACT is one of the standardized tests for colleges admissions the United States. This score is used along with other materials such as grade point average (GPA) and essay responses to determine whether or not students are accepted into a university. 

Presently 16 out of 50 states and the District of Columbia (DC) require all students to take the ACT as part of statewide testing programs - meaning the tests are offered for free in these states. Seven additional states also fund these tests on optional basis, allowing their students to take the tests for free. Meanwhile, 20 states including DC have started working with the College Board to administer SAT for free. ([*source*](https://blog.prepscholar.com/which-states-require-the-sat))

There are 4 sections in the ACT: English, Mathematics, Reading, and Science, with an additional optional writing section ([*source*](https://www.act.org/content/act/en/products-and-services/the-act/scores/understanding-your-scores.html)). Meanwhile in the other standardized tests, SAT, only has two sections in the test: Evidence-Based Reading & Writing and Math ([*source*](https://www.princetonreview.com/college/sat-sections)). While both tests have different formats and score ranges, the ACT is generally considered more content, particularly the Science section.

However, standardized tests continues to be a controversial topic for students, administrators, and legislators. Supporters of these tests argue that these scores are an objective measure to determine college admittance and provides a push to students to perform academically. Opponents of these tests claim that these tests are not accurate measures of students potential or ability and serve as an inequitable barrier to entry. Lately, more and more schools around the US have opted to drop the SAT/ACT requirement. ([*source*](https://www.virginiamercury.com/2022/10/31/more-virginia-colleges-make-sat-act-exams-optional/))

Before we hold the American education system and parents (or anyone else) accountable for the declining test scores, the first thing we need to figure out is - are test scores really on a decline, per the reports by ACT? 


### Problem Statements
1. Does the participation rate influence ACT scores?
2. Are there overlaps in the ACT subjects, and are the scores related to each other? If yes, do we need to review the format of the ACT?

**Target Audience**: State education departments


### Data Source
This research will cover ACT scores from 2017 to 2022, to ensure a fair analysis that also includes the pre-pandemic period. The datasets used for this research are:

- [`act_2017.csv`](./datasets/act_2017.csv): 2017 ACT Scores by State, provided as part of this project package
- [`act_2018.csv`](./datasets/act_2018_v2.csv): 2018 ACT Scores by State, taken from the U.S. Department of Education, National Center for Education Statistics ([*source*](https://nces.ed.gov/programs/digest/d18/tables/dt18_226.60.asp))
- [`act_2019.csv`](./datasets/act_2019_v2.csv): 2019 ACT Scores by State, taken from the U.S. Department of Education, National Center for Education Statistics ([*source*](https://nces.ed.gov/programs/digest/d19/tables/dt19_226.60.asp))
- [`act_2020.csv`](./datasets/act_2020.csv): 2020 ACT Scores by State, taken from the U.S. Department of Education, National Center for Education Statistics ([*source*](https://nces.ed.gov/programs/digest/d20/tables/dt20_226.60.asp))
- [`act_2021.csv`](./datasets/act_2021.csv): 2021 ACT Scores by State, taken from the U.S. Department of Education, National Center for Education Statistics ([*source*](https://nces.ed.gov/programs/digest/d21/tables/dt21_226.60.asp))
- [`act_2022.csv`](./datasets/act_2022.csv): 2022 ACT Scores by State, taken from ACT ([*source*](https://www.act.org/content/dam/act/unsecured/documents/2022/2022-Average-ACT-Scores-by-State.pdf))


### Data Dictionary

| Feature                        	| Type     	| Dataset         	| Description                                                        	|
|--------------------------------	|----------	|-----------------	|--------------------------------------------------------------------	|
| **state**                      	| _object_ 	| ACT 2017        	| All state names in the US                                          	|
| **part_17**                    	| _float_  	| ACT 2017        	| The 2017 average participation rate in the ACT                     	|
| **eng_17**                     	| _float_  	| ACT 2017        	| The 2017 average ACT English scores                                	|
| **math_17**                    	| _float_  	| ACT 2017        	| The 2017 average ACT Math scores                                   	|
| **read_17**                    	| _float_  	| ACT 2017        	| The 2017 average ACT Reading scores                                	|
| **sci_17**                     	| _float_  	| ACT 2017        	| The 2017 average ACT Science scores                                	|
| **comp_17**                    	| _float_  	| ACT 2017        	| The 2017 average Composite scores                                  	|
| **part_18**                    	| _float_  	| ACT 2018        	| The 2018 average participation rate in the ACT                     	|
| **eng_18**                     	| _float_  	| ACT 2018        	| The 2018 average ACT English scores                                	|
| **math_18**                    	| _float_  	| ACT 2018        	| The 2018 average ACT Math scores                                   	|
| **read_18**                    	| _float_  	| ACT 2018        	| The 2018 average ACT Reading scores                                	|
| **sci_18**                     	| _float_  	| ACT 2018        	| The 2018 average ACT Science scores                                	|
| **comp_18**                    	| _float_  	| ACT 2018        	| The 2018 average Composite scores                                  	|
| **part_19**                    	| _float_  	| ACT 2019        	| The 2019 average participation rate in the ACT                     	|
| **eng_19**                     	| _float_  	| ACT 2019        	| The 2019 average ACT English scores                                	|
| **math_19**                    	| _float_  	| ACT 2019        	| The 2019 average ACT Math scores                                   	|
| **read_19**                    	| _float_  	| ACT 2019        	| The 2019 average ACT Reading scores                                	|
| **sci_19**                     	| _float_  	| ACT 2019        	| The 2018 average ACT Science scores                                	|
| **comp_19**                    	| _float_  	| ACT 2019        	| The 2018 average Composite scores                                  	|
| **part_20**                    	| _float_  	| ACT 2020        	| The 2020 average participation rate in the ACT                     	|
| **eng_20**                     	| _float_  	| ACT 2020        	| The 2020 average ACT English scores                                	|
| **math_20**                    	| _float_  	| ACT 2020        	| The 2020 average ACT Math scores                                   	|
| **read_20**                    	| _float_  	| ACT 2020        	| The 2020 average ACT Reading scores                                	|
| **sci_20**                     	| _float_  	| ACT 2020        	| The 2020 average ACT Science scores                                	|
| **comp_20**                    	| _float_  	| ACT 2020        	| The 2020 average Composite scores                                  	|
| **part_21**                    	| _float_  	| ACT 2021        	| The 2021 average participation rate in the ACT                     	|
| **eng_21**                     	| _float_  	| ACT 2021        	| The 2021 average ACT English scores                                	|
| **math_21**                    	| _float_  	| ACT 2021        	| The 2021 average ACT Math scores                                   	|
| **read_21**                    	| _float_  	| ACT 2021        	| The 2021 average ACT Reading scores                                	|
| **sci_21**                     	| _float_  	| ACT 2021        	| The 2021 average ACT Science scores                                	|
| **comp_21**                    	| _float_  	| ACT 2021        	| The 2021 average Composite scores                                  	|
| **part_22**                    	| _float_  	| ACT 2022        	| The 2022 average participation rate in the ACT                     	|
| **eng_22**                     	| _float_  	| ACT 2022        	| The 2022 average ACT English scores                                	|
| **math_22**                    	| _float_  	| ACT 2022        	| The 2022 average ACT Math scores                                   	|
| **read_22**                    	| _float_  	| ACT 2022        	| The 2022 average ACT Reading scores                                	|
| **sci_22**                     	| _float_  	| ACT 2022        	| The 2022 average ACT Science scores                                	|
| **comp_22**                    	| _float_  	| ACT 2022        	| The 2022 average Composite scores                                  	|
| **national_avg_participation** 	| _float_  	| ACT 2017 - 2022 	| The national average participation rates for ACT from 2017 to 2021 	|
| **national_avg_english**       	| _float_  	| ACT 2017 - 2022 	| The national average English scores for ACT from 2017 to 2021      	|
| **national_avg_math**          	| _float_  	| ACT 2017 - 2022 	| The national average Math scores for ACT from 2017 to 2021         	|
| **national_avg_reading**       	| _float_  	| ACT 2017 - 2022 	| The national average Reading scores for ACT from 2017 to 2021      	|
| **national_avg_science**       	| _float_  	| ACT 2017 - 2022 	| The national average Science scores for ACT from 2017 to 2021      	|
| **national_avg_composite**     	| _float_  	| ACT 2017 - 2022 	| The national average Composite scores for ACT from 2017 to 2021    	|


### Additional Research 

These additional articles and datapoints were used throughout the analysis and to better understand the current state of standardized testing in the US.

- 2022 ACT National Profile Report ([*source*](https://www.act.org/content/dam/act/unsecured/documents/2022/2022-National-ACT-Profile-Report.pdf))
- 2022 ACT average score press release ([*source*](https://leadershipblog.act.org/2022/10/GradClassRelease2022.html))
- ABC article on lowest ACT score ([*source*](https://abcnews.go.com/US/high-school-class-2022-lowest-act-scores-30/story?id=91497084))
- Fortune article on worst test score ([*source*](https://fortune.com/2022/10/12/act-college-admissions-scores-high-school-graduates-worst-30-years/))
- Bloomberg opinion editorial on standardized testing ([*source*](https://www.bloomberg.com/opinion/articles/2022-10-26/us-colleges-should-bring-back-sat-and-act-test-requirements?srnd=opinion))
- Bloomberg article on the rate of test submissions in college applications ([*source*](https://www.bloomberg.com/news/articles/2022-01-24/wealthy-teens-tout-test-results-colleges-no-longer-require))
- More than 1,700 US colleges enforcing test-optional for Fall 2023 ([*source*](https://www.highereddive.com/news/over-1700-colleges-wont-require-sat-act-for-fall-2023-up-from-same-poin/628267/))
- More Virginia colleges enforcing test-optional policy ([*source*](https://www.virginiamercury.com/2022/10/31/more-virginia-colleges-make-sat-act-exams-optional/))
- Maine revamping standardized tests ([*source*](https://www.mainepublic.org/maine/2021-02-02/maine-schools-plan-to-administer-revamped-standardized-tests-after-shelving-them-during-pandemic))
- List of standardized tests by state ([*source*](https://educationadvanced.com/resources/blog/list-of-standardized-tests-by-state/))
- About the ACT Science Section ([*source*](https://www.usnews.com/education/blogs/college-admissions-playbook/articles/what-to-know-about-the-act-science-section))
- US map of ACT 2022 participation rate from ACT 2022 Data Visualization: ([*source*](https://tableauprototypes.act.org/t/ACTExternal/views/ACTProfileReport2022/PercentTestedbyState?%3Aembed=y&%3Adisplay_count=n&%3AshowVizHome=n&%3Aorigin=viz_share_link))


### Summary Findings

1. ACT Participation Rates

- In 2022, 
 - States with higher ACT testing rates for the ACT are in the west, midwest and southern regions, e.g. Nevada, Montana, Oklahoma, Mississippi. 
 - States outside of the US mainland, Alaska and Hawaii also saw high testing rates for the ACT.
 - States with lowest ACT testing rates in the East Coast and West Coast areas, e.g. Maine, New York, California, Oregon, Washington, etc.([*source*](https://tableauprototypes.act.org/t/ACTExternal/views/ACTProfileReport2022/PercentTestedbyState?%3Aembed=y&%3Adisplay_count=n&%3AshowVizHome=n&%3Aorigin=viz_share_link))

- Alabama, Mississippi, Nevada, and Tennessee were able to achieve 100% participation rate for six consecutive years. These states are located in the southern region and have implemented mandatory ACT tests for all high school students. ([*source*](https://blog.prepscholar.com/which-states-require-the-act-full-list-and-advice))

- An increasing number of the states' participation rate dropped in 2021 and 2022 from a perfect 100% in the previous years. These states are Arkansas, Kentucky, Louisiana, Montana, Nebraska, North Carolina, Ohio, Oklahoma, Utah, Wisconsin and Wyoming - standardized tests are also mandated in most of these states.

- Meanwhile, despite a perfect participation in 2017, Colorado saw noticeable and more significant dip in its participation rate from 2018 onwards. During that time period, Colorado started transitioning away from standardized exams to design the state's English and math tests. ([*source*](https://www.coloradoindependent.com/2017/07/06/from-csap-to-parcc-heres-how-colorados-standardized-tests-have-changed-and-whats-next/)) In more recent news, the state of Colorado removed standardized tests as an admission criteria to higher insitutions. ([*source*](https://leg.colorado.gov/bills/hb21-1067)) We can expect the participation rate in Colorado to decline or plateau in the coming years. It's likely that students who continue to take the ACT to fulfill scholarship criteria and also apply for out-of-state colleges that require standardized tests for admission. 

- Maine had the lowest ACT participation rates for six consecutive years. Reason being, Maine has their own standardized test which they've revamped after changes in how students received their eduation during the pandemic ([*source*](https://www.mainepublic.org/maine/2021-02-02/maine-schools-plan-to-administer-revamped-standardized-tests-after-shelving-them-during-pandemic)) and they require all students to take the SAT. ([*source*](https://educationadvanced.com/resources/blog/list-of-standardized-tests-by-state/))

- New Hampshire, Delaware, Rhode Island and Pennsylvania also had relatively low ACT participation rates compared to other states, and continue to decline. These states require students to take the SAT, which likely influenced the declining ACT testing. ([*source*](https://educationadvanced.com/resources/blog/list-of-standardized-tests-by-state/))

2. ACT Subject and Composite Scores

- States with lowest subject and composite scores are Nevada, Mississippi, South Carolina, Hawaii, and North Carolina. While Nevada and Mississippi saw perfect participation rates, these appear to be independent with how the students are performing in the ACT. 

- States with highest subject and composite scores are New Hampshire, Massachusettes, Connecticut, Maine, and New York. These states also show improvement in average scores over the years, but most of them saw a small decline from 2021 to 2022. 

- Subject scores from one year to another are positively correlated, which means that states' performance in certain subjects will be about the same or change slightly in the following years. The impact of any new academic policies and teaching styles will take time, so it's unlikely to see huge leaps in scores within a short timeframe.


### Conclusion 

Overall, the analysis of ACT scores from 2017 to 2022 has shown that:

1. The participation rate are negatively related to ACT scores, and they are nearly independent. The influence of participation rate on performance is minimal, and improving participation rate will not necessarily improve scores because,
 - States that enforce mandatory testing will have a more diverse group of students taking the tests - hence lowering the average scores. 
 - Students in test-optional states who choose to take the ACT are likely to be strong in academic tests, and they may be doing it for scholarship or to boost their college application.
 - Many states have their own statewide tests that students are required to take; it’s not efficient to study for multiple standardized tests.
 - With more colleges enforcing test-optional policy, students may choose to skip the tests so they can focus on their ongoing education and other admission criteria.

2. English and Reading subjects appear to overlap in terms of average scores and trends - indicating that the ACT board could consider reviewing the format of the test and condense further. This may help incentivize more students to take the ACT.

3. While Math and Science scores appear to overlap, however it is not feasible to combine the tests as the subject matters vary greatly. Students looking to specialise in Math- or Science-related majors will likely need the separate scores for their college admission or scholarship application. 


### Recommendations

1. To review the need for mandatory statewide standardized tests and assess how to best help students of different abilities/potential learn.

2. If the mandatory testing policies are meant to drive interest in higher education, schools can encourage students to leverage the colleges’ test-optional policies and apply to more colleges.

3. However if the tests are meant to boost academic standards, state education departments and schools need to recognize different ways to do that and instill an interest in learning, for example, through projects, laboratory time, assignments, etc.

4. Take a more holistic approach to measuring students’ readiness for college, e.g. GPA scores, essays, interviews, advanced-level classes credits, extracurricular activities, passion projects/ hobbies.

