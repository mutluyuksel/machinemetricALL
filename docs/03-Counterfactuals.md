
# Counterfactual:

Imagine a college student,Alex, who occasionally gets sick after eating but doesn't know which specific food is the culprit. In a community increasingly concerned about food allergies, this young individual grappled with recurring allergic reactions. Driven by a pressing need to pinpoint the root cause, he embarked on a personal mission. Eager to understand the extent of his susceptibility, Alex meticulously documented every instance in which he consumed food, noting all the ingredients, leading to a comprehensive data collection effort.

In his quest to uncover the reason for his sporadic sickness after eating, Alex adopted an approach that resembled common quantitative research methods: collecting data, utilizing descriptive statistics, visualizing the data, finding correlations, and ultimately using methods to determine the causation of the allergy.

As Alex continues to gather more data about his dietary intake and subsequent health reactions, he starts by creating a simple table for each day. After visualizing the data, he begins to spot correlations between certain foods and his well-being.

**Data Visualization**:

Based on this recorded data, Alex can employ various visualization methods to better understand and identify patterns:

a) For the Histogram of Reaction Intensity, this chart allows Alex to see the frequency of days with varying intensities of reactions. The X-axis represents the Reaction Intensity ranging from 1 to 10, while the Y-axis shows the Number of Days. An observation he might make is if he notices a high number of days with intensities around 8-10 after consuming garlic, providing an initial clue.

b) In the Bar Chart of Reactions by Food, he can visually compare the average reaction intensities for various foods. The X-axis displays different foods or ingredients such as garlic, dairy, and wheat. The Y-axis represents the Average Reaction Intensity. If the bar for garlic consistently stands out in comparison to other foods, it further signals a potential issue.

c) The Time Series Line Graph enables Alex to track the evolution of reactions over time. With the X-axis indicating the Date and the Y-axis highlighting the Reaction Intensity, a line tracing the intensity of reactions over time can help him pinpoint if certain clusters of high-intensity days align with the consumption of specific food.

Recognizing correlations visually with these tools means Alex can discern if there's a pronounced spike in the histogram every time garlic is consumed. The bar chart might indicate that garlic has a noticeably higher average reaction intensity than other foods. Similarly, the time series graph can demonstrate peaks in reaction intensities on specific dates, which Alex can then cross-reference with the food he consumed on those days.

By visually plotting the data, Alex can more effectively recognize patterns and correlations, offering a foundational understanding before venturing into more intricate statistical analyses.

**Investigating Correlations**:

Observing Correlations: Alex began to rank his reactions on a scale from 1 to 10, with 10 marking the most severe reaction. As days turned to weeks, he noticed that every time he consumed garlic, the intensity of his reaction consistently hovered between 8 to 10. Contrastingly, other foods such as dairy or wheat might occasionally result in a reaction intensity of 3 or 4, but not always.

Potential Confounding Factors: On a particular day, Alex felt unwell after a meal without garlic, but recalled having a milkshake. Wondering if dairy might be another trigger, he started noting down dairy consumption alongside garlic. However, after several dairy-heavy days without any reaction, it becomes clear that the milkshake incident might have been a coincidence or caused by another factor.

Strength of Correlation: As weeks go by, the association between garlic ingestion and feeling under the weather becomes more evident. The consistency and strength of this correlation are much higher than with any other food. In statistical terms, one might say that garlic have a strong positive correlation with Alex's adverse reactions.

Spurious Correlations: A pattern Alex took note of was his increased tendency to fall ill on weekends. However, after some contemplation, he discerned that weekends were when he often dined out, inadvertently upping the odds of ingesting garlic. his is an example of a spurious correlation: the actual problem wasn't the weekend itself, but rather the increased exposure to the allergen.

Drawing Conclusions: While correlation does not imply causation, the consistent and strong correlation between garlic consumption and adverse reactions, gives Alex confidence in the hypothesis that he is allergic to garlic.

In this example, Alex's observations and data tracking are analogous to the process of determining correlation in statistical or machine learning contexts. Correlations can highlight patterns, yet it's crucial to ensure that confounding factors or spurious correlations aren't misleading the conclusions.

**The Mystery of Mia’s Illness:**

On certain weekends, Mia, Alex's girlfriend, also started feeling unwell. As she began to correlate her illness to the days she spent with Alex, she grew concerned. Was she allergic to something at Alex’s place? Or, even more alarmingly, was she developing an allergy to garlic, having shared many garlic-laden dishes with him?

Mia decided to chart her symptoms alongside Alex’s diary of garlic consumption. To her surprise, she found that she felt sick on several occasions when Alex had garlic in his meals, even if she hadn’t consumed any garlic herself.

Spurious Correlation Revealed:Further probing revealed an interesting detail. Whenever Alex prepared dishes with garlic at his place, he'd also light up a particular brand of aromatic candle to mask the strong garlic smell. Mia wasn't reacting to the garlic, but to the scent of that specific candle. Her sickness wasn’t directly linked to the days Alex consumed garlic, but rather to the days the candle was lit. The correlation between her sickness and Alex's garlic consumption was spurious, with the actual causative agent being the candle’s aroma.

In this example, Mia’s conclusion, based on initial observations, would lead her down the wrong path, emphasizing the importance of not mistaking correlation for causation. It serves as a cautionary tale on the pitfalls of spurious correlations in both real-life and statistical contexts.

**Alex's exploration of the effect of his garlic consumption on his allergy severity:**

After discovering a strong correlation between his garlic consumption and allergic reactions, Alex decided to take his investigation a step further. While the correlation was evident, he wanted to quantitatively understand the exact impact of garlic consumption on his reactions. He suspected that while garlic was the primary association with his reactions, other variables might exacerbate or alleviate his symptoms. Beyond just the amount of garlic he consumed, could factors like his weight, the weather temperature, and even eating outside influence the severity of his reactions?

Gathering Data: For several weeks, Alex meticulously documented the amount of garlic in his meals, his weight each day, the day's peak weather temperature, whether he dined inside or outside.

To understand the relationship better, Alex used an Ordinary Least Squares (OLS) regression. This approach would allow him to understand how each variable, when considered together, might predict the severity of his allergic reaction. He find that the coefficient for garlic quantity was positive, reaffirming that the more garlic he consumed, the stronger the allergic reaction. Interestingly, on days when he weighed more, the severity of his allergic reaction was slightly less, all else being equal. Perhaps his body was better equipped to handle allergens when he was at a slightly higher weight. On warmer days, Alex's allergic reactions were milder than on colder days. Dining outside frequently correlated with more intense reactions. This puzzled Alex until he realized that eating outside often meant dining at restaurants or cafes where he had less control over ingredients, and the chance of consuming hidden garlic was higher.

Alex remembered that his girlfriend once mentioned he seemed to react more during weekends. Reflecting on it, he saw that weekends were indeed when they often dined out, leading to more exposure to garlic-rich dishes. It wasn't the fact that it was a weekend causing the reactions but the increased likelihood of eating garlic-containing food outside. This was a classic case of spurious correlation; the real culprit was the garlic, not the weekend!

Equipped with these insights, Alex made some lifestyle changes. He became cautious about eating out, especially on weekends. He also kept an eye on the day's temperature, preparing for potential reactions on colder days. Knowing that his weight had a buffering effect was an added insight, but he decided that a balanced diet and regular exercise were more crucial for his overall health.

**Investigating Causation**

Building on the previously identified correlation between garlic and adverse reactions, Alex feels the pressing need to ascertain whether garlic truly triggers his allergic responses. Although correlation had provided some preliminary insights, he recognized the limitations of correlation evidence in proving causation. He turned to Ordinary Least Squares (OLS) regression analysis, aiming to isolate the impact of garlic relative to other potential variables, like his weight, weather temperature, and the environment where he eats.

He remembered a recent news article discussing certain foods that were structurally and chemically similar to garlic. The article suggested that these foods could also trigger allergic reactions in individuals sensitive to garlic. This revelation complicated his inquiry, as neither correlation nor regression methods could offer him a definitive answer. Could there be other foods amplifying his reactions? Or was garlic the sole offender?

Determined to get to the bottom of this mystery, Alex decided to undertake a more rigorous approach: the experimental method. Often hailed as the gold standard for establishing causality, this method would allow Alex to control specific variables and thereby isolate the effects of garlic and other similar foods on his system. By methodically introducing and removing these foods from his diet in a controlled setting, he aimed to definitively ascertain the root cause of his adverse reactions.

To unravel this mystery, Alex approached his friend Mia, who didn't have any known food allergies, to participate in a controlled experiment. By having Mia as a control group, Alex could compare reactions between them, potentially teasing out the specific effects of garlic.

They both embarked on a week-long experiment, where their diets were standardized, with the only variance being the consumption of garlic and its similar foods. Mia's consistent lack of adverse reactions when consuming the same meals as Alex, especially those containing garlic, reinforced its role in Alex's allergic symptoms. Meanwhile, Alex's symptoms persisted, lending more weight to the hypothesis about garlic's culpability.

When Mia remained symptom-free even after consuming the foods similar to garlic that the news had warned about, it provided Alex with further clarity. It became evident that while those foods might be problematic for some, they weren't the culprits in Alex's case. By incorporating Mia into the experiment as a control group, Alex was not only able to more confidently ascertain the role of garlic in his reactions but also to rule out other potential allergens. 

Causation Established: With consistent results across multiple trials, combined with the knowledge that other potential causes have been ruled out, Alex concludes that garlic is not just correlated with, but is the actual cause of his allergic reactions. In scientific terms, Alex has moved from observing a correlation (a relationship between garlic consumption and allergic reactions) to establishing causation (determining that garlic directly causes the allergic reactions).

This journey mirrors the scientific process where controlled experiments, repeated trials, and the isolation of variables are crucial for determining the true cause of an observed effect.


## Qualitative and Quantitative research methods:

In the realm of research, there are two primary methodologies: qualitative and quantitative. Qualitative research methods often involve focus groups, unstructured or in-depth interviews, and the review of documents to discern specific themes. For instance, in social sciences, a qualitative study might explore the lived experiences of individuals living in poverty, capturing their stories and challenges through in-depth interviews. In economics, qualitative research might delve into understanding the socio-economic factors influencing a community's resistance to adopting digital currencies.

On the other hand, quantitative research typically employs surveys, structured interviews, and measurements. It also involves reviewing records or documents to gather numeric or quantifiable data. Quantitative methods emphasize objective measurements and the statistical, mathematical, or numerical analysis of data collected through polls, questionnaires, and surveys. An example from economics might be a study analyzing the correlation between unemployment rates and economic recessions using historical data. Another economic example could be a quantitative analysis of the impact of interest rate changes on consumer spending patterns over a decade.

Additionally, quantitative research can involve manipulating pre-existing statistical data using computational techniques. For instance, in economics, researchers might use computational models to predict the future growth rate of an economy based on various indicators. Quantitative research is not just a method but a way to learn about a specific group of people, known as a sample population. In the health sector, a quantitative study might examine the efficacy of a new drug on a sample population, measuring specific health outcomes and side effects. In economics, a study might evaluate the spending habits of millennials compared to baby boomers using structured surveys. Through scientific inquiry, it relies on data that are observed or measured to examine questions about this sample population. There are various designs under quantitative research, including Descriptive non-experimental, Quasi-experimental, and Experimental.

The processes that underpin these two research types differ significantly. Qualitative research is characterized by its inductive approach, which aids in the formulation of theories or hypotheses. In contrast, quantitative research follows a deductive approach, aiming to test predefined concepts, constructs, and hypotheses that together form a theory.

When considering the nature of the data, qualitative research is inherently subjective. It seeks to describe issues or conditions from the vantage point of those experiencing them. For example, in economics, a qualitative study might investigate the perceptions of small business owners towards global trade agreements. Quantitative research, however, is more objective. It focuses on observing the effects of a program on an issue or condition, with these observations subsequently interpreted by researchers.

The type of data these methodologies yield is also distinct. Qualitative research is text-based, delving deep to provide rich information on a limited number of cases. Quantitative research, meanwhile, is number-based, offering a broader scope of information but spread across a larger number of cases, often sacrificing depth for breadth.

In terms of response options, qualitative research tends to use unstructured or semi-structured options, allowing for more open-ended answers. Quantitative research, in contrast, relies on fixed response options, measurements, or observations. Furthermore, while qualitative research does not typically employ statistical tests in its analysis, quantitative research does, ensuring a more structured and numerical interpretation of data.

Lastly, when it comes to generalizability, qualitative research findings are often less generalizable due to their in-depth focus on specific cases. Quantitative research, with its broader scope, tends to be more generalizable to larger populations.

In summary, while both qualitative and quantitative research methodologies offer valuable insights, they differ in their methods, processes, nature of data, and generalizability, each serving unique purposes in the research landscape, as evidenced by their applications in fields like economics, social sciences, and health. In this book, we cover quantitative methods. 

https://libguides.usc.edu/writingguide/quantitative

## Quantitative - Research methods :

General perspective about research methods in health, economics, and social sciences:

A researcher asks a good answerable question. It does not mean we can always find the answer right away with available data and methods.  Yet we know that we can find an answer which will expand our knowledge of how the world works. A good answerable research question can be defined as a hypothesis which can be a phenomenon what we observe in the world. Also, hypothesis, that we want to prove, comes from theory as well.  If the theory explains or predicts this is the specific hypothesis how the world works, then we should observe it with the data. 

To answer these questions, we collect or obtain data, then explore data.  After making certain assumptions, we analyze the data. Then, we reach conclusions which can be associations, correlations, or causal relations. We use results to explain, extrapolate or predict! our hypothesis.	 We covered these concepts in detail in the introduction of this book.

Different fields have dominant methods within their field to answer research questions. 
[The main source for health section is C. Manski, Patient Care under Uncertainty, Princeton University Press, 2019.]
Health research use “Evidence Based Research!” 	
Manski told in his seminal book “Research on treatment response and personalized risk assessment shares a common objective: Probabilistic prediction of some patient outcome conditional on specified patient attributes...Econometricians and Statisticians refer to conditional prediction as regression, a term in use since the nineteenth century. Some psychologists use the term actuarial prediction and statistical prediction. Computer scientists may refer to machine learning and artificial intelligence. Researchers in business school may speak of predictive analytics.”
In most general way, after collecting and analyzing data, they present descriptive analysis seeks to understand associations. By various medical research methods, especially “Gold standard methods!”, when(if) they determine X causes Y. They propose treatment and surveillance. By using clinical trials, they want to determine treatment/surveillance and find its efficacy and effectiveness. Using Prescriptive analyses, they attempt to improve the performance of actual decision making. They try to find optimal solution between surveillance and aggressive treatment. Mainly, they use clinical judgment and evidence-based research.
In general, statistical imprecision and identification problems affect empirical (evidence-based) research that uses sample data to predict population outcomes. There is a tension between the strength of assumptions and their credibility. The credibility of the inference decreases with the strength of the assumptions maintained.

The most credible and acceptable method is The Gold Standard! In health.  The "Gold Standard" Method for Health researchers is obtaining the effect of tested treatment comparing the results from trials and experiments which has treatment and control groups, and. In machine learning this is known as A/B testing, in economics it is random and field experiments. 

Even though this method is the most credible method in empirical research, it has problems like any other empirical methods. First, study/trial sample and actual patient population can be very different. Second, Due to small sample sizes, estimates and identification of treatment effects are imprecise. Third, it is wishful extrapolation to assume that treatment response in trials performed on volunteers is the same as what would occur in actual patient populations. Thus, predictions are fragile as they have limited data and do not handle uncertainty sufficiently.

Most of health researcher give more value for the results obtained by a randomized trial with 200 observations than results from observational studies with 200,000 observations. Why do most of the medical and health researchers have this perspective?	 To justify trials performed on study populations that may differ substantially from patient populations, researchers in public health and the social sciences often cite Donald Campbell, who made a distinction between the internal and external validity of studies of the treatment response (Campbell and Stanley, 1963). A study has internal validity if it has credible findings for the study population (in-sample data in Machine Learning). It has external validity if an invariance assumption permits credible extrapolation (out-sample in ML). The appeal of randomized trials is their internal validity. Campbell argued that studies should be judged primarily by their internal validity and secondarily by their external validity. Since 1960s, this perspective has been used to argue for the primacy of experimental research over observational studies, whatever the study population may be.

In contrast, observational studies which uses the representative sample of the population have more credibility in economics than randomized control trials with a small sample.  The Campbell perspective has also been used to argue that the best observational studies are those that most closely approximate randomized experiments if they are done with representative samples. 

We should keep in mind that statistics and economics have the following perspective which is weird in other fields. For instance, "All models are wrong, but some are useful" (Box, 1976), and "Economists should not worry if their assumptions are wrong, as long as their conclusions are relatively accurate." (Friedman, 1953)

## Data and visualization

Researchers in fields such as health, economics, business, and social sciences primarily utilize various datasets to deepen their understanding of dynamic and static phenomena. These datasets are primarily categorized into three types: cross-sectional data, time series data, and panel data, which is also referred to as longitudinal data.

Cross-sectional data is collected at a single point in time or within a short period, and is sourced from a variety of subjects, including individuals, companies, or countries. This type of dataset is instrumental in capturing a snapshot of various characteristics or attributes of a population at a given moment, providing insights into the current state of affairs without the changes over time.

In contrast, time series data, collected over an extended period at regular intervals, tracks changes in a particular variable over time. This data is useful for identifying trends and patterns over time and forecasting future occurrences based on historical data.

Panel data combines elements of both cross-sectional and time series datasets by tracking the same sample of subjects over time. This type of data is valuable for studying the relationship between different variables, identifying trends and patterns over time. Panel data enables researchers to analyze the impact of various factors on outcomes while controlling for individual-fixed effects.

The process of working with these datasets involves several critical steps to ensure the reliability and validity of the findings. Initially, researchers must examine the raw data to grasp its structure and content thoroughly. Following this, the data must be cleaned and prepared, which involves checking for errors, addressing missing values, and removing outliers to ensure the dataset is in a usable state. Finally, understanding the data through meticulous statistical analysis, creating visualizations, and employing various analytical techniques is essential to uncover underlying patterns and relationships within the data. This methodical approach enables researchers to derive meaningful conclusions that can significantly impact their respective fields.

Effective visualization is crucial for revealing features in data that are essential for further analysis. It serves as a foundational element in the analytical process across various disciplines, helping clarify complex information. Utilizing a range of visualization techniques, such as histograms, barplots, boxplots, scatterplots, and heatmaps, researchers can uncover subtle patterns and trends that may not be evident from raw data alone. These visual representations provide a comprehensive overview of the data, enabling researchers to identify relationships, correlations, and outliers that can inform subsequent analyses and decision-making processes.

Histograms graphically represent the frequency or distribution of data, whether continuous or discrete. This visualization comprises bins, each representing a range of values, with the height of each bin showing the frequency of data points within that range. For example, a histogram illustrating animal weights might have bins for different weight intervals, such as 20-29 kg and 30-39 kg, with each bin's height indicating the number of animals within those ranges.

Barplots graphically display data's mean or median, providing a visual comparison of central tendencies across different groups or categories. Each bar's height represents the mean or median for that group. For instance, a barplot could compare the average fuel efficiency of various car models or median home prices across different neighborhoods.

Boxplots show a dataset's distribution and are particularly valuable for visualizing data spread, skewness, and potential outliers. They include a box representing the interquartile range (middle 50% of the data), a median line, and whiskers that extend to the data's minimum and maximum values. This makes boxplots ideal for comparing distributions from different groups, such as student exam scores across various classes.

Scatterplots are used to illustrate the relationship between two variables, helping to visualize correlations and trends. In a scatterplot, each point represents the values of two variables for a data point. This type of plot might show how advertising spend correlates with sales revenue or the link between study hours and test scores.

Heatmaps provide a visual representation of the relationship between two or more variables by using color-coded cells, where each color intensity reflects the value of the variables for that cell. Heatmaps are particularly effective for data organized in grids or matrices, such as correlating stock prices or mapping crime frequency across different times and locations.

In addition to these commonly used techniques, there are other advanced visualization tools that can enhance the exploratory data analysis process. Line graphs, for instance, are particularly useful in time series data analysis, enabling the tracking of changes over time with clarity and precision. Area charts can also be employed to illustrate quantitative data graphically, showing how different components contribute to the whole over a given interval. Network diagrams are invaluable for visualizing relationships and interactions within datasets, especially in social sciences and biology, where understanding the connections between entities is crucial.

Moreover, interactive visualizations have become increasingly popular due to their ability to allow users to manipulate the parameters and directly see the effects of different variables on the data. Tools like dashboards and interactive maps provide dynamic insights that can adapt to varying user inputs, offering a more hands-on approach to data exploration.

By integrating these advanced and interactive techniques, researchers can gain a more nuanced understanding of their data. This comprehensive approach not only aids in identifying the underlying trends and patterns but also supports robust decision-making by providing a more detailed and interactive view of the data landscape. Building on these visualization techniques, the next subsection will focus on the concept of correlation, examining how it quantifies the strength and direction of relationships between variables, further enriching our understanding of data interactions.

##  Correlation

The phrase "correlation does not imply causation" is often invoked in discussions of statistical relationships to emphasize a critical caution in data interpretation. To fully grasp what this means, we must first understand the concept of correlation and its role in evaluating the connections between two variables.

Correlation is a statistical measure that quantifies the degree of association between two variables, typically describing how closely the variables follow a linear relationship. The term "association" is broader than "correlation," encompassing any type of relationship between two variables, whether linear or not. In various sectors, including finance, healthcare, and marketing, correlation measurements are crucial for analyzing data and guiding decision-making processes. The etymology of the word "correlation" combines "co-" (meaning together) with "relation," highlighting its function in identifying connections between quantities.

There are three types of correlations: positive, negative, and zero. A positive correlation indicates that both variables move in the same direction; for example, an increase in advertising expenditure might correspond to a rise in sales revenue, suggesting a positive correlation. In contrast, a negative correlation means the variables move in opposite directions, such as the relationship between the number of hours spent watching television and academic performance, where more TV time is associated with lower grades. Variables are considered uncorrelated if changes in one do not affect the other, indicating no discernible relationship.

Correlation analysis is a statistical method used to study the association or absence of a relationship between two variables. By examining the correlation between variables, researchers can measure the strength and nature of their association, allowing them to quantify how variables move together or apart. This analysis is integral in determining a numerical value that reflects the relationship between two variables, whether the change in one variable accompanies a change in another directly or indirectly.

The Pearson correlation coefficient is one of the most commonly used measures in correlation analysis. It quantifies the strength and direction of a linear relationship between two numerical variables. This coefficient ranges from -1 to 1, where -1 indicates a strong negative relationship, 0 signifies no relationship, and 1 indicates a strong positive relationship. For example, a Pearson correlation of 0.8 between two variables denotes a strong positive relationship, suggesting that an increase in one variable generally leads to an increase in the other.

The Pearson correlation coefficient, denoted as \( r \), can be calculated using two equivalent formulas. The first formula is:
\[
r = \frac{\sum (x_i - \overline{x})(y_i - \overline{y})}{\sqrt{\sum (x_i - \overline{x})^2 \sum (y_i - \overline{y})^2}}
\]
This formula directly computes \( r \) as the ratio of the sum of the product of deviations of \( x \) and \( y \) from their means to the geometric mean of the sums of squared deviations of \( x \) and \( y \) from their respective means.

The second method involves the covariance and the standard deviations of \( x \) and \( y \):
\[
r = \frac{\text{cov}(x, y)}{s_x s_y}
\]
where covariance, \( \text{cov}(x, y) \), is defined as:
\[
\text{cov}(x, y) = \frac{1}{n-1} \sum (x_i - \overline{x})(y_i - \overline{y})
\]
and the standard deviations, \( s_x \) and \( s_y \), are given by:
\[
s_x = \sqrt{\frac{1}{n-1} \sum (x_i - \overline{x})^2}
\]
\[
s_y = \sqrt{\frac{1}{n-1} \sum (y_i - \overline{y})^2}
\]

Here, \( x_i \) and \( y_i \) represent the values of the two variables, \( \overline{x} \) and \( \overline{y} \) are the means of the variables \( x \) and \( y \) respectively, and the sums are taken over all \( n \) pairs of data. These formulas showcase how \( r \) quantifies the linear relationship between \( x \) and \( y \), normalizing the covariance of the variables by the product of their standard deviations, thus measuring the degree to which \( x \) and \( y \) co-vary relative to their individual variability.


Covariance provides an indication of the direction of the linear relationship between two variables, 
\( X \) and \( Y \). However, it does not effectively convey the strength of the relationship because it is affected by the scale of the variables involved. To mitigate this limitation of covariance, we use the correlation coefficient.

Correlation is essentially the covariance between two variables standardized by the product of their standard deviation, or the ratio of the covariance to the product of the standard deviations of the two variables. This process of standardization transforms covariance into a dimensionless measure, which ranges from -1 to 1. This range allows for meaningful comparisons across different datasets and variables regardless of their original scales.

In the following simulation, we demonstrate the influence of scaling on covariance and the invariance of the correlation coefficient to such changes. We begin by generating two variables, each with 20 observations, and subsequently scale these variables by multiplying each by 1000. This process significantly alters the covariance values, showcasing how covariance is affected by the scale of the data. However, when we calculate the correlation coefficients using two different equations above —both before and after scaling—we observe that correlation remain sama regardless of the scale, unlike covariance.


```r
# Set seed for reproducibility
set.seed(0)

# Generate two variables each with 20 observations, all less than 10
x <- runif(20, min = 0, max = 10)
y <- runif(20, min = 0, max = 10)

# Scaling the data by multiplying each element by 1000
x_scaled <- x * 1000
y_scaled <- y * 1000

# Print the original and scaled variables
#print(x)
#print(y)
#print(x_scaled)
#print(y_scaled)

# Calculate the covariance between x and y
covariance_original <- cov(x, y)
print(paste("Original covariance:", covariance_original))
```

```
## [1] "Original covariance: -1.26490786248817"
```

```r
# Calculate the covariance between x_scaled and y_scaled
covariance_scaled <- cov(x_scaled, y_scaled)
print(paste("Covariance after scaling:", covariance_scaled))
```

```
## [1] "Covariance after scaling: -1264907.86248817"
```

```r
# Compute standard deviations for both datasets
sd_x <- sd(x)
sd_y <- sd(y)
#print(paste("Standard deviation of x:", sd_x))
#print(paste("Standard deviation of y:", sd_y))

# Standardize the variables
x_standardized <- (x - mean(x)) / sd_x
y_standardized <- (y - mean(y)) / sd_y
#print(paste("Standardized variable x:", x_standardized))
#print(paste("Standardized variable y:", y_standardized))

# Calculate the covariance between the standardized x and y which give us the correlation coefficient:
correlation_original <- cov(x_standardized, y_standardized)
print(paste("Correlation after standardizing:", correlation_original))
```

```
## [1] "Correlation after standardizing: -0.152795399233766"
```

```r
# Equivalent formula to calculate the correlation between the original x and y
correlation_original2 <- cov(x, y) / (sd_x * sd_y)
print(paste("Correlation after standardizing2:", correlation_original2))
```

```
## [1] "Correlation after standardizing2: -0.152795399233766"
```

```r
# Compute standard deviations for both scaled datasets
sd_x_scaled <- sd(x_scaled)
sd_y_scaled <- sd(y_scaled)
# Standardize the variables
x_scaled_standardized <- (x_scaled - mean(x_scaled)) / sd_x_scaled
y_scaled_standardized <- (y_scaled - mean(y_scaled)) / sd_y_scaled

# Calculate the correlation between the scaled x and y
correlation_scaled <- cov(x_scaled, y_scaled)/(sd_x_scaled * sd_y_scaled)
print(paste("Correlation after scaling:", correlation_scaled))
```

```
## [1] "Correlation after scaling: -0.152795399233766"
```

```r
# Equivalent formula to calculate the correlation between the scaled x and y
correlation_scaled2 <- cov(x_scaled_standardized, y_scaled_standardized)
print(paste("Correlation after scaling:", correlation_scaled2))
```

```
## [1] "Correlation after scaling: -0.152795399233766"
```

Having seen how correlation remains consistent across different scales, highlighting the robustness of this statistical measure against changes in data magnitude, we want to remind to the critical role of data visualization that we discussed in the previous subsection. A compelling illustration of why visual analysis is essential is provided by the Anscombe Quartet. This example underscores the limitations of relying solely on statistical summaries and demonstrates the importance of visualizing data to capture the true nature of relationships between variables.

A classic example that highlights the importance of visualizing data before drawing conclusions is the Anscombe Quartet (1973). This dataset consists of four sets of data that have nearly identical statistical properties, including the same mean, variance, and correlation. Moreover, each group's linear regression line has identical parameters, yet the underlying data distributions vary significantly. Thus, when plotted, the datasets reveal distinct patterns, emphasizing the need to visualize data to understand relationships accurately.  Group I displays a typical linear relationship, while Group II reveals a nonlinear pattern, illustrating poor fit despite identical regression lines. Group III's outlier drastically affects the regression influence, misleading interpretations if not visually inspected. Group IV, dominated by a cluster at one x-value with a single influential point, also misrepresents the actual data characteristics through its fitting. These visual discrepancies underscore the crucial role of plotting raw data to correctly interpret statistical results and avoid misleading conclusions based solely on numerical summaries.



```r
# Create Anscombe's quartet dataset
anscombe <- data.frame(
  x1 = c(10, 8, 13, 9, 11, 14, 6, 4, 12, 7, 5),
  y1 = c(8.04, 6.95, 7.58, 8.81, 8.33, 9.96, 7.24, 4.26, 10.84, 4.82, 5.68),
  x2 = c(10, 8, 13, 9, 11, 14, 6, 4, 12, 7, 5),
  y2 = c(9.14, 8.14, 8.74, 8.77, 9.26, 8.10, 6.13, 3.10, 9.13, 7.26, 4.74),
  x3 = c(10, 8, 13, 9, 11, 14, 6, 4, 12, 7, 5),
  y3 = c(7.46, 6.77, 12.74, 7.11, 7.81, 8.84, 6.08, 5.39, 8.15, 6.42, 5.73),
  x4 = c(8, 8, 8, 8, 8, 8, 8, 19, 8, 8, 8),
  y4 = c(6.58, 5.76, 7.71, 8.84, 8.47, 7.04, 5.25, 12.50, 5.56, 7.91, 6.89)
)

# Set up the plotting area with consistent axes and include fitted lines
par(mfrow = c(2, 2)) # Arrange plots in a 2x2 grid

# Define consistent x and y axis limits
xlim <- c(3, 20)
ylim <- c(2, 14)

# Function to calculate and print stats for each group
calculate_stats <- function(x, y) {
  c(mean_x = formatC(mean(x), format = "f", digits = 3), 
    mean_y = formatC(mean(y), format = "f", digits = 3), 
    variance_x = formatC(var(x), format = "f", digits = 3), 
    variance_y = formatC(var(y), format = "f", digits = 3), 
    covariance = formatC(cov(x, y), format = "f", digits = 3),  # Calculating covariance
    correlation = formatC(cor(x, y), format = "f", digits = 3), 
    intercept = formatC(coef(lm(y ~ x))[1], format = "f", digits = 3), 
    slope = formatC(coef(lm(y ~ x))[2], format = "f", digits = 3))
}

# Calculate stats for each group
stats1 <- calculate_stats(anscombe$x1, anscombe$y1)
stats2 <- calculate_stats(anscombe$x2, anscombe$y2)
stats3 <- calculate_stats(anscombe$x3, anscombe$y3)
stats4 <- calculate_stats(anscombe$x4, anscombe$y4)

# Create a matrix for the statistics
stats_matrix <- cbind("Statistics" = c("Mean X", "Mean Y", "Variance X", "Variance Y", 
                                      "Covariance", "Correlation", "Intercept", "Slope"), 
                     "Group I" = stats1, 
                     "Group II" = stats2, 
                     "Group III" = stats3, 
                     "Group IV" = stats4)

# Convert matrix to data frame for nicer printing
stats_df <- as.data.frame(stats_matrix)

# Print the data frame without row names
print(stats_df, row.names = FALSE)
```

```
##   Statistics Group I Group II Group III Group IV
##       Mean X   9.000    9.000     9.000    9.000
##       Mean Y   7.501    7.501     7.500    7.501
##   Variance X  11.000   11.000    11.000   11.000
##   Variance Y   4.127    4.128     4.123    4.123
##   Covariance   5.501    5.500     5.497    5.499
##  Correlation   0.816    0.816     0.816    0.817
##    Intercept   3.000    3.001     3.002    3.002
##        Slope   0.500    0.500     0.500    0.500
```

```r
# Print the data frame without row names
print(stats_df, row.names = FALSE)
```

```
##   Statistics Group I Group II Group III Group IV
##       Mean X   9.000    9.000     9.000    9.000
##       Mean Y   7.501    7.501     7.500    7.501
##   Variance X  11.000   11.000    11.000   11.000
##   Variance Y   4.127    4.128     4.123    4.123
##   Covariance   5.501    5.500     5.497    5.499
##  Correlation   0.816    0.816     0.816    0.817
##    Intercept   3.000    3.001     3.002    3.002
##        Slope   0.500    0.500     0.500    0.500
```

```r
# Group I
plot(anscombe$x1, anscombe$y1, main = "Group I", xlab = "X1", ylab = "Y1", 
     pch = 19, col = "blue", xlim = xlim, ylim = ylim)
abline(lm(y1 ~ x1, data = anscombe), col = "blue")

# Group II
plot(anscombe$x2, anscombe$y2, main = "Group II", xlab = "X2", ylab = "Y2", 
     pch = 19, col = "red", xlim = xlim, ylim = ylim)
abline(lm(y2 ~ x2, data = anscombe), col = "red")

# Group III
plot(anscombe$x3, anscombe$y3, main = "Group III", xlab = "X3", ylab = "Y3", 
     pch = 19, col = "green", xlim = xlim, ylim = ylim)
abline(lm(y3 ~ x3, data = anscombe), col = "green")

# Group IV
plot(anscombe$x4, anscombe$y4, main = "Group IV", xlab = "X4", ylab = "Y4", 
     pch = 19, col = "purple", xlim = xlim, ylim = ylim)
abline(lm(y4 ~ x4, data = anscombe), col = "purple")
```

<img src="03-Counterfactuals_files/figure-html/unnamed-chunk-2-1.png" width="672" />


Note that Correlation between x and y is zero doesNOT mean that x and y are not related and independent. It means that there is no linear relationship between x and y. There might be a non-linear relationship between x and y. 


```r
# Set seed for reproducibility
set.seed(0)

# Generate x as a sequence of values
x <- -10:10

# Define y as a non-linear function of x (e.g., y = A+B*x^2)
y <- 9+2*x^2

# Plot x vs y to visualize the non-linear relationship
plot(x, y, main = "Non-linear Relationship: 9+2*x^2", xlab = "x", ylab = "y", pch = 19, col = "blue")
```

<img src="03-Counterfactuals_files/figure-html/unnamed-chunk-3-1.png" width="672" />

```r
# Calculate and print the correlation between x and y
correlation <- cor(x, y)
print(paste("Correlation between x and y:", formatC(correlation, format = "f", digits = 3)))
```

```
## [1] "Correlation between x and y: -0.000"
```

If the relationship between variables is nonlinear, other correlation measures may be more appropriate.

Beyond the Pearson correlation, other correlation measures include partial correlation, conditional correlation, spatial correlation, and dynamic correlation.Partial correlation, for example, is a statistical method that measures the relationship between two variables while controlling for the effects of one or more additional variables. This technique helps isolate the direct relationship between the two primary variables by excluding the influence of other factors. For instance, in examining the relationship between education level and income, partial correlation can be utilized to account for variables like age or work experience, providing a clearer picture of the direct impacts of education on income.

Conditional correlation also measures the relationship between two variables but includes the consideration of one or more categorical variables. This method aims to understand how other variables might modify the relationship between the primary variables of interest.

Spatial correlation is another important technique, especially relevant in geographical studies. It assesses the relationship between variables measured at different locations, helping to determine if and how closely observations near each other are related. For example, researchers might use spatial correlation to analyze how pollution levels correlate with population density across different urban areas.

Lastly, dynamic correlation is used to analyze the relationship between variables that change over time. This measure is particularly useful in fields like finance or economics, where it is important to understand how relationships between variables such as stock prices and economic indicators evolve. Dynamic correlation provides insights into how these relationships fluctuate over time, aiding in the prediction of future trends based on historical data.

Each of these correlation measures offers unique insights and is chosen based on the specific characteristics of the data and the research questions at hand. These tools allow researchers to delve deeper into understanding the complexities of variable interactions, ensuring a more comprehensive analysis of their data.

In summary, correlation analysis is a powerful statistical tool for examining the relationships between variables, allowing researchers to measure the strength and nature of these associations. By employing various correlation measures such as Pearson correlation, partial correlation, conditional correlation, spatial correlation, and dynamic correlation, researchers can gain valuable insights into the complex relationships between variables in numerous fields.

Understanding the nature of correlation between variables allows for the prediction of future trends and clarifies the type of relationship, if any, that exists. However, the critical caveat remains: correlation does not imply causation. The presence of a strong correlation does not necessarily mean that one variable causes changes in another. There could be confounding factors or other underlying causes affecting the observed relationship. This underscores the importance of contextual understanding and conducting further analyses to explore causality beyond mere correlation before drawing definitive conclusions about the effects one variable may have on another.This analytical caution is encapsulated in the phrase "correlation does not imply causation," highlighting the necessity of a deeper investigation beyond correlation to fully understand the dynamics at play.

**Correlation and Regression**

Correlation and regression are two statistical methods used to analyze the relationships between variables. While they share some similarities, their purposes and applications differ significantly.Both correlation and regression are used to explore relationships between variables and typically assume a linear relationship between them. Additionally, both techniques involve the calculation of coefficients that quantify the relationships between variables, helping to illustrate how these variables interrelate.

However, the key differences between the two methods are crucial to understand. Correlation is primarily a descriptive statistical technique that measures the strength and direction of a relationship between two variables. It is used to summarize how closely two variables are related without predicting one from the other. Correlation is quantified using a correlation coefficient, which ranges from -1 to 1. A correlation coefficient of 1 indicates a perfect positive relationship, -1 signifies a perfect negative relationship, and 0 denotes no relationship. Correlation is valuable for identifying associations between variables, such as the relationship between smoking and lung cancer, without implying causation.

On the other hand, regression is a predictive statistical technique that not only assesses the relationship between variables but also models and predicts the value of one variable based on the value of another. This makes regression particularly valuable for forecasting and determining the impact of changes in one variable on another. Regression analysis can handle both continuous variables, such as height and weight, and categorical variables, such as GPA and major. It utilizes various statistics to build its models, including the coefficient of variables, the standard error, and the p-value, which help to understand the accuracy and reliability of the predictions made.

In conclusion, while correlation and regression both analyze relationships between variables, they serve different purposes: correlation describes the relationship without implying causation, while regression goes a step further by modeling and predicting outcomes based on this relationship. Understanding these differences is essential when selecting the appropriate statistical method for data analysis, ensuring that the analysis aligns with the research objectives.


##  Effect of X on Y / Regression

Economists and social scientists predominantly utilize observational survey data to answer research questions or test hypotheses. By analyzing samples, they make inferences about the larger population, which involves addressing three key issues: the effect of other factors on the relationship between x (independent variable) and y (dependent variable), the functional relationship between y and x, and ensuring a ceteris paribus (all other things being equal) condition in their analysis.

The simple linear regression model effectively addresses these concerns. It assumes a linear relationship between x and y, focusing on interpreting this relationship rather than on prediction. This contrasts with machine learning (ML) techniques, which do not assume a specific functional form but instead seek the optimal form for the best predictive model. This difference in focus is highlighted in Victor Chernozhukov's presentation at the 2013 NBER Summer Institute, where he demonstrated that Lasso, a linear ML method, can better approximate the conditional expectation function (CEF) than ordinary least squares (OLS) for certain datasets.

Bruce Hansen, in his recent book, points out that OLS regression yields the best linear approximation of the CEF. This property makes regression particularly valuable to economists and social scientists who are more interested in interpreting an approximation of reality rather than engaging in complex curve fitting.

The predictive power of \(x\) on \(y\) is encapsulated in the Conditional Expectation Function (CEF), \(E(y \mid x_i)\), which represents the expected value of \(y\) when a specific covariate \(x\) is held constant. This function is crucial for understanding how changes in x affect y on average, rather than predicting individual outcomes. The regression CEF theorem further supports this by stating that even if the CEF is nonlinear, regression provides the best linear approximation.

OLS estimates the coefficient \(\beta_1\) using a random sample of data to represent the population and makes assumptions about the relationships between the error term \(u\) and \(x\). These assumptions include the expected value of the error term being zero in the population, mean independence of the error term, and the zero conditional mean assumption.

In summary, while both simple linear regression and machine learning methods offer distinct approaches to exploring the relationship between x and y in observational survey data, they cater to different needs. Regression emphasizes interpretation and provides the best linear approximation to the CEF, useful for understanding distributions and influences in the data. On the other hand, machine learning techniques focus on creating the best functional form for predictive modeling, useful for making accurate predictions. Both methods have their merits and can provide valuable insights for economists and social scientists, depending on their specific research objectives.

### How can we estimate the population parameters, $\beta_{0}$ and $\beta_{1}$?

To estimate the population parameters \(\beta_0, \beta_1, \ldots, \beta_k\) in a linear regression model, we start by selecting a random sample that represents the population. We model the relationship as:
\[ y_i = \beta_0 + \beta_1 x_{i1} + \ldots + \beta_k x_{ik} + \epsilon_i, \]
where \( \epsilon_i \) represents the error terms satisfying the assumptions \( E(\epsilon_i) = 0 \) and \( \operatorname{Cov}(x_{ij}, \epsilon_i) = 0 \) for all \( j \).

The Ordinary Least Squares (OLS) method estimates the parameters by minimizing the sum of the squared residuals. This involves solving:
\[ \min_{\hat{\beta}_0, \hat{\beta}_1, \ldots, \hat{\beta}_k} \sum_{i=1}^{n} \left( y_i - (\hat{\beta}_0 + \hat{\beta}_1 x_{i1} + \ldots + \hat{\beta}_k x_{ik}) \right)^2. \]

The matrix form of the same model is \( y = X\beta + \epsilon \), where \( X \) is the matrix of regressors and \( \epsilon \) is the vector of error terms with \( \epsilon_i \sim (0, \sigma^2) \). The OLS estimator \(\hat{\beta}\) is given by:
\[ \hat{\beta} = (X'X)^{-1}X'y, \]
where \( X' \) is the transpose of \( X \) and \( y \) is the vector of observed values. This estimator provides the best linear unbiased estimates (BLUE) of the parameters under the Gauss-Markov theorem, assuming linearity, exogeneity, and homoscedasticity of errors among other conditions. Further exploration of error terms and OLS properties will be covered in Chapter 5.

That results from the first order conditions for the minimization problem:
\[ \frac{1}{n} \sum_{i=1}^n x_i (y_i - x_i' \hat{\beta}) = 0. \]

This estimator provides the best linear unbiased estimates (BLUE) of the parameters under the Gauss-Markov theorem, assuming linearity, exogeneity, and homoscedasticity of errors among other conditions. Further exploration of error terms and OLS properties will be covered in Chapter 5.

### Predicting $y$

The next step in regression analysis is predicting the dependent variable \( y \) using a set of predictors. Given estimators \( \hat{\beta}_0 \) and \( \hat{\beta}_1 \), we define the fitted values for each observation \( i \) as:
\[
    \hat{y}_i = \hat{\beta}_0 + \hat{\beta}_1 x_i.
\]
This equation provides us with \( n \) fitted values corresponding to \( n \) observations. The fitted value \( \hat{y}_i \) represents the predicted value of \( y_i \) given the predictor \( x_i \) and the estimated coefficients \( \hat{\beta} \).

The difference between the actual value \( y_i \) and the predicted value \( \hat{y}_i \) is known as the residual, which quantifies the error in our prediction:
\[
    \hat{\epsilon}_i = y_i - \hat{y}_i = y_i - (\hat{\beta}_0 + \hat{\beta}_1 x_i).
\]

In the matrix form, the model can be expressed as:
\[
    Y = X\beta + \epsilon,
\]
where \( Y \) is the vector of observed values, \( X \) is the matrix of predictors including a column of ones for the intercept, \( \beta \) is the vector of coefficients, and \( \epsilon \) is the vector of residuals. The OLS solution to estimating \( \beta \) is:
\[
    \hat{\beta} = (X'X)^{-1}X'Y,
\]
resulting in the vector of fitted values:
\[
    \hat{Y} = X\hat{\beta}.
\]
and residuals:
\[ \hat{\epsilon} = Y - \hat{Y}. \]

This matrix form is particularly beneficial in multiple regression models, clarifying the relationship between multiple predictors and the response variable. Detailed examination of these relationships will continue in Chapter 5.

\textbf{Note:} In econometrics, we often focus not just on forecasting \(y_i\) but also on understanding the relationship between \(y_i\) and elements of \(x_i\), with other factors held constant (ceteris paribus). We estimate coefficients by minimizing the sum of squared residuals in OLS. Different samples yield different estimates \(\hat{\beta}^1\) for the true \(\beta_1\), making \(\beta_1\) a random variable. However, \(\hat{\beta}^1\) acts as an estimator for that causal parameter, derived from a specific sample. The effect of \(x\) on \(y\) is \(\beta_1\) as long as it remains unbiased. Estimates must also be consistent and satisfy asymptotic normality, which we will explore in further chapter 5.

Unbiasedness means that if we could repeatedly take random samples on \(Y\) from the population and compute an estimate each time, the average of these estimates would equal \(\beta_1\). OLS is unbiased under certain assumptions: the model must be linear in parameters, utilize random sampling, include sample variation in the explanatory variable, ensure zero conditional mean, and exhibit homoskedasticity or constant variance (alternatively, handle heteroskedasticity). These conditions guarantee that, on average, our estimates match the population values.

Consistency ensures that using a larger sample size decreases the likelihood of obtaining an estimate \(\hat{\beta}\) that substantially deviates from the true effect \(\beta\). As sample size increases towards the size of the entire population, an estimate \(\hat{\beta}\) increasingly reflects the true \(\beta\), particularly when \(\beta\) is unbiased and its variance decreases with larger samples.

When many samples are drawn randomly, and \(\beta\) is estimated in each, asymptotic normality suggests that the pooled estimate \(\hat{\beta}\) from these samples follows a normal distribution, given very large sample sizes. Having this property makes it possible to approximate the distribution of an estimate across many samples well, even if we have only one sample with a sufficient number of observations rather than many samples. Understanding the distribution of an estimate is crucial in statistical inference.

However, obtaining an unbiased \(\beta\) is often very challenging or even impossible, as the population DGM (Data Generating Mechanism) is unknown. Errors may not be iid (independently and identically distributed). For example, observations between units in a group might be related (clustered), samples might be non-representative, or there could be issues such as the exclusion or inclusion of variables, measurement errors, endogeneity, reverse causality, or missing observations. Therefore, we often find associations or correlations instead of causal relationships. In such cases, we discuss the relationship, association, or correlation between \(y\) and \(x\).

### Maximum Likelihood Estimation (MLE)}

Maximum Likelihood Estimation (MLE) is a statistical method that estimates the parameters of a statistical model based on observed data. Unlike Ordinary Least Squares (OLS), which minimizes the squared differences between observed and predicted values, MLE seeks the parameter values that make the observed data most probable under an assumed probability distribution.

In MLE, the core objective is to estimate unknown parameters by maximizing the likelihood function, \( L(\theta; x) \), which represents the probability of observing the data \( x \) given the parameters \( \theta \):
\[
    \hat{\theta} = \arg\max_{\theta} L(\theta; x).
\]
This approach aims to find the parameter values \( \theta \) that best explain the observed data under the specified model.

Maximum Likelihood Estimation (MLE) offers a range of benefits that can make it a preferred choice over other estimation methods such as Ordinary Least Squares (OLS). MLE is known for its consistency; the estimates it provides converge to the true parameter values as the sample size increases, assuming the model is accurately specified. Additionally, under certain regularity conditions, MLE estimates are asymptotically normally distributed. This property is highly beneficial as it facilitates the construction of confidence intervals and enables hypothesis testing. MLE also stands out for its efficiency, achieving the lowest possible variance among all unbiased estimators, which guarantees highly precise estimates. Another advantage of MLE is its invariance property; the estimates remain unchanged under transformations, meaning that the transformation of the estimates corresponds directly to the estimates of the transformed parameters.

However, despite these significant advantages, MLE comes with certain limitations that must be carefully managed. One major drawback is its dependence on the correct specification of the data's probability distribution. If the assumed probability distribution does not accurately reflect the true distribution, the MLE estimates may become biased or inconsistent. MLE is also sensitive to outliers in the data because it aims to maximize the likelihood of the entire dataset. This sensitivity can result in biased estimates if the dataset contains extreme values. Furthermore, the process of maximizing the likelihood function can be computationally intensive, posing challenges in cases involving large datasets or complex models. This computational demand requires robust computational resources and can complicate the application of MLE in large-scale data analysis.

Keep in mind that Ordinary Least Squares (OLS) and Maximum Likelihood Estimation (MLE) converge under certain conditions, primarily when the model assumptions align particularly well. The most common scenario where OLS and MLE provide identical estimates is in linear regression models with normally distributed error terms. In such cases, the assumptions for OLS—that the errors have a mean of zero (no bias) and constant variance (homoscedasticity)—also satisfy the requirements for MLE under a normal distribution. Specifically, when the error terms are assumed to be normally distributed, the likelihood function for a linear model becomes proportional to the sum of squared residuals, which OLS minimizes. Thus, minimizing these residuals (as OLS does) also maximizes the likelihood of observing the data under the assumed normal error distribution (as MLE seeks to do). This overlapping objective ensures that both estimation methods yield the same parameter estimates when the model errors are normally distributed and other regularity conditions are met. However, in cases where the model assumptions diverge, such as non-normal error terms or heteroscedasticity, OLS and MLE may produce different estimates. Understanding the relationship between OLS and MLE is essential for interpreting regression results and selecting the most appropriate estimation method for a given dataset and research question.


```r
# Set seed for reproducibility
set.seed(123)

# Generate a vector of 10,000 random integers between 9 and 24
x <- sample(9:24, 10000, replace = TRUE)

# View the first few elements of x
# head(x)
intercept <- 3
slope <- 2
epsilon <- rnorm(10000, mean = 0, sd = 1)  # Error term
y <- intercept + slope * x + epsilon  # True linear relationship with some noise

# Perform linear regression using OLS
ols_model <- lm(y ~ x)
summary(ols_model)
```

```
## 
## Call:
## lm(formula = y ~ x)
## 
## Residuals:
##     Min      1Q  Median      3Q     Max 
## -3.8310 -0.6682 -0.0044  0.6948  3.8534 
## 
## Coefficients:
##             Estimate Std. Error t value Pr(>|t|)    
## (Intercept) 2.966117   0.036993   80.18   <2e-16 ***
## x           2.002174   0.002158  927.76   <2e-16 ***
## ---
## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
## 
## Residual standard error: 1.002 on 9998 degrees of freedom
## Multiple R-squared:  0.9885,	Adjusted R-squared:  0.9885 
## F-statistic: 8.607e+05 on 1 and 9998 DF,  p-value: < 2.2e-16
```

```r
# Perform linear regression using MLE
mle_model <- nls(y ~ beta0 + beta1 * x, start = list(beta0 = 0, beta1 = 0))
summary(mle_model)
```

```
## 
## Formula: y ~ beta0 + beta1 * x
## 
## Parameters:
##       Estimate Std. Error t value Pr(>|t|)    
## beta0 2.966117   0.036993   80.18   <2e-16 ***
## beta1 2.002174   0.002158  927.76   <2e-16 ***
## ---
## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
## 
## Residual standard error: 1.002 on 9998 degrees of freedom
## 
## Number of iterations to convergence: 1 
## Achieved convergence tolerance: 1.201e-09
```


In conclusion, Maximum Likelihood Estimation is a robust method for parameter estimation in statistical modeling, offering flexibility and efficiency under specific probability distribution assumptions. However, it is crucial to be mindful of its limitations regarding distributional assumptions and outlier sensitivity when applying MLE to real-world data. We will explore these concepts further in subsequent chapters.

##  Causal Effect

You may have heard the phrase "correlation does not equal causation," emphasizing that the co-occurrence of two events does not automatically imply that one causes the other. A more precise expression would be "correlation is not sufficient for causation." This distinction is crucial in research design, particularly in the initial stages prior to data collection. Unlike most traditional statistical analyses where you work with an existing random sample with no control over its selection, causal inference requires careful planning in the design phase.

In this phase, researchers decide how treatments are assigned to sample units or patients. If direct assignment isn't feasible, it becomes necessary to gather detailed information about covariates which can affect the outcome. This proactive approach in experimental design is fundamental for making valid causal inferences from the data. It's important to recognize that while correlation can indicate a relationship, it does not confirm causality without these rigorously controlled conditions. This perspective is a significant shift from typical statistical tasks, where the primary goal is to interpret and make sense of already collected data, emphasizing the importance of design in causal studies.

Most of the time though, we also want to find out not only the relationship or correlation between observations but also the reason behind it. Using this information, we are able to take action to alter the relationships and causes. Essentially, we want to know what the consequences are of not doing one thing or the other. Our goal is to understand the effects and consequences of specific actions, policies, and decisions.

In order to develop a hypothesis about such causal effects, we rely upon previous observations, personal experiences, and other information. Researchers in economics, health, and social sciences analyze empirical data to evaluate policies, actions, and choices based on quantitative methods.

When we want to say something about why? We work with potential outcomes Potential Outcomes (Neyman, 1923 - Rubin, 1975) framework, especially in applied economics, or directed acyclic graphs (DAG) which you can think presenting a chain of causal effects with a graph. We will review causal analysis as short as possible, and considering the approaches integrating the machine learning with causal analysis. The books we can recommend in this topic are Causal Inference-The Mixtape, The Effect, Mostly Harmless Econometrics,...

At the center of interest is the causal effect of some intervention or treatment on an outcome of interest by inferring what the outcome would be in the presence and in the absence of a specific treatment. Causality is tied to a unit (person, firm, classroom, city) exposed to an action (manipulation, treatment or intervention) at a particular point in time. The Causal Effect is the comparison or difference of potential outcomes,$Y_{i}(1)$ and $Y_{i}(0)$, for the same unit, at the same moment in time post-treatment. where $Y_{i}(1)$ is the outcome when unit $i$ exposed the treatment (active treatment state), and $Y_{i}(0)$ is the outcome when same unit $i$ has not exposed the treatment (control state) (at the same point in time)

Let's say $D$ is the treatment indicator (or intervention, or policy). When $D=1$ , the unit receives the treatment or participates in the intervention, thus these units constitute "treatment group". When $D=0$ , the unit does not receive treatment or does not participate in the intervention, thus these units constitute "control group". 

The causal effect of treatment,$D$, on outcome,$Y$, is the difference between the potential outcomes $Y_{i}(1)- Y_{i}(0)$ for unit $i$. 

However, we can not observe the unit in 2 different state at the same time. We can not observe "The Road Not Taken" (by Robert Frost). "The fundamental problem of causal inference" is therefore the problem that at most one of the potential
outcomes can be realized and thus observed (Holland, 1986). Thus, Holland (1986, 2003) says "No causation without manipulation" 

 Keep in mind that counter-factual state is and never will be observable. We can define counterfactual as what would have happened in the absence of a policy/treatment. Donald Rubin has been known to say that "causal inference is a missing data problem" (Ding and Li, 2018)
Hence, there are several methods used to find causal effect. Experiments (Randomized Control Trials) and Quasi-natural Experiments such as Regression Discontinuity (Sharp, Fuzzy), Instrumental Variable, Difference-in-Difference(-in-Difference), Synthetic Cohort, Propensity Score, and Partial identification. 

We can never know the real! causal effect (of a unit) in social sciences. Using Rubin’s framework, we can only estimate the causal effect under certain assumptions. Overcoming the missing data problem arising from the fact that only one state of nature is realized is very difficult. To do so requires credible assumptions!


Main implicit assumption in Rubin framework for all the aforementioned methods is the Stable Unit Treatment Value Assumption (SUTVA, Rubin 1978). SUTVA implies that potential outcomes of observation $i$ are independent of the treatment assignment of all other units. In another word, the unit's potential outcome are not affected by the spillover or interference effects by the treatment of other units. Thus, SUTVA rules out general equilibrium or indirect effects via spillovers.  Moreover, SUTVA also implies that the treatment, $D$, is identical for all observations and no variation in treatment intensity. Most of the current empirical work assumed this assumption satisfied. However, it may not be always plausible to assume no spillover effect when treated group is very large share of the population. We also need to reassess our policy proposal, which are based on the findings of randomized or natural experiments, for all population as they may violate SUTVA assumption when these studies are designed with small sample. 



### Average Treatment Effect(ATE)


While causal effects cannot be observed and measured at a unit level, under certain statistical assumptions we may identify causal effect of treatment,D, on outcome,Y, at an aggregate level, while using treatment and control groups.  

Even though we cannot observe treatment effect for each individual/unit separately, we know that for a given population these individual causal effects-if exist- will generate a distribution of treatment effects. [footnote: A distribution is simply a collection of data, or scores, on a variable. Usually, these scores are arranged in order from smallest to largest and then they can be presented graphically. — Page 6, Statistics in Plain English, Third Edition, 2010.]Thus, we can estimate the mean, variance and other parameters related to this distribution. 

 Most common parameter we want to estimate is the mean of treatment distribution. We can think the average treatment effect(ATE) is the population average of all individual treatment effects. We can formally write:
$$	
		 \delta^{ATE} = E[\delta_{i}]= E[Y_{i}(1) - Y_{i}(0)] = E[Y_{i}(1)] - E[Y_{i}(0)]
$$

 As known, the expected value of a random variable X is often denoted by E(X). 
 
 
 Assume government implement a policy, an agency act, or a doctor prescribe a pill. All in all, we can think 2 states. Treatment state in which every units in the population exposed a treatment, and control state in which every units in the population has not exposed the treatment . The equation above shows that the average of the outcome for everyone in treatment state and the average of the outcome for everyone in control state is called the average treatment effect for all population.
 
Depends on the question, we may want to estimate different treatment effects as well. Some of them are:
  
 Average Treatment Effect on the Treated (ATT, or ATET): The average treatment effect on the treatment group is equal to the average treatment effect conditional on being a treatment group member (D=1).
 
$$ 
 ATT= E[Y_{i}(1)|D=1] - E[Y_{i}(0) | D=1]
 $$
Average Treatment Effect on the Untreated (ATU): The average treatment effect on the control group is equal to the average treatment effect conditional on being untreated.
$$ 
 ATU= E[Y_{i}(1)|D=0] - E[Y_{i}(0) | D=0]
 $$

However,we want to emphasize ATE (ATT, and ATU) is unknowable because of the fundamental problem of causal inference.i.e. we can only observe individuals either when they receive treatment state or when they do not, thus we cannot calculate the average treatment effect. However, we can estimate it. How?

If we can find a population or split the population such as some of whom receive this treatment or act on it and some of whom has not. Then we can estimate "causal/treatment effect" as the difference between average outcome of the treated group and average outcome of control group.

How does the population split into treatment and control group? Whether units have any choice to be eligible for the treatment or not? Whether splitting process has any direct effect on outcome or not? How large, how many and how similar similar these groups? Whether treatment level is equal or not? Whether everyone who are eligible for treatment receive treatment or not? 
Answers of all these questions require different identification strategies and leads all the different causal methods we use.
 
### Additional Treatment Effects

yesil pdf fileindan
Local Average Treatment Effect (LATE): g = E[dijCompliers]The Local Average Treatment Effect (LATE) is a statistical measure that is used to estimate the effect of a treatment or intervention on a specific subgroup of the population. It is a measure of the average treatment effect for a group of individuals who would not have received the treatment if they had not been eligible for it.

LATE is typically estimated using a technique called instrumental variables (IV) regression, which involves using a variable that is correlated with the treatment but is not directly affected by the outcome of interest. By using this "instrumental" variable, researchers can estimate the effect of the treatment on the subgroup of individuals who are eligible for the treatment based on their values of the instrumental variable.

LATE is a useful measure when the treatment effect is not the same for all individuals in the population. For example, a study might estimate the LATE of a new medication on individuals with a specific type of disease, in order to understand how the medication affects this subgroup compared to the overall population.

It is important to note that LATE is only applicable when the treatment is randomly assigned, meaning that individuals are assigned to receive the treatment or not receive the treatment based on chance rather than their characteristics or other factors. This is necessary in order to ensure that the treatment effect can be accurately estimated and is not confounded by other factors.



Conditional Average Treatment Effect (CATE)
d(x) = E[Yi(1)−Yi(0)jXi = x] = E[dijXi = x]
• Xi exogenous pre-treatment covariates/features
• Xi includes not only confounders but also other covariates which are potentially
responsible for effect heterogeneity
• CATEs are often called individualised or personalised treatment effects
• CATEs can differ from CATET, r(x), and CLATE, g(x)

The Conditional Average Treatment Effect (CATE) is a statistical measure that is used to estimate the effect of a treatment or intervention on a specific subgroup of the population. It is a measure of the average treatment effect for a group of individuals who are similar in some way, such as having the same level of a certain characteristic or risk factor.

CATE is typically estimated using a technique called conditional mean regression, which involves estimating the expected value of the outcome variable for individuals with different values of the conditioning variable. By using this conditioning variable, researchers can estimate the effect of the treatment on the subgroup of individuals who are similar in terms of the conditioning variable, compared to the overall population.

CATE is a useful measure when the treatment effect is not the same for all individuals in the population and when there is a characteristic or factor that may influence the treatment effect. For example, a study might estimate the CATE of a new medication on individuals with a specific type of disease, in order to understand how the medication affects this subgroup compared to individuals with a different type of disease.

It is important to note that CATE is only applicable when the treatment is randomly assigned, meaning that individuals are assigned to receive the treatment or not receive the treatment based on chance rather than their characteristics or other factors. This is necessary in order to ensure that the treatment effect can be accurately estimated and is not confounded by other factors.

Group Average Treatment Effects (GATEs):
d(g) = E[d(x)jGi = g]
where the groups g can be defined based on exogenous or endogenous
variables

Group Average Treatment Effects (GATE) is a statistical measure that is used to estimate the effect of a treatment or intervention on a specific subgroup of the population. It is a measure of the average treatment effect for a group of individuals who are similar in some way, such as having the same level of a certain characteristic or risk factor.

GATE is typically estimated using a technique called group mean regression, which involves estimating the mean of the outcome variable for individuals with different values of the grouping variable. By using this grouping variable, researchers can estimate the effect of the treatment on the subgroup of individuals who are similar in terms of the grouping variable, compared to the overall population.

GATE is a useful measure when the treatment effect is not the same for all individuals in the population and when there is a characteristic or factor that may influence the treatment effect. For example, a study might estimate the GATE of a new medication on individuals with a specific type of disease, in order to understand how the medication affects this subgroup compared to individuals with a different type of disease.

It is important to note that GATE is only applicable when the treatment is randomly assigned, meaning that individuals are assigned to receive the treatment or not receive the treatment based on chance rather than their characteristics or other factors. This is necessary in order to ensure that the treatment effect can be accurately estimated and is not confounded by other factors.
 
### Selection Bias and Heteregeneous Treatment Effect Bias:

 When a group of individuals receive a treatment and a group does not, most inclined to calculate the treatment effect just calculating the simple difference between average outcomes of treated group and control group. However, this is (nearly) always wrong.
 
Can we find average treatment effect by calculating the simple difference between the average outcome for the treatment group and the average outcome for the control group? 

There may be already intrinsic differences between these 2 groups as some already decided to choose treatment, or there may be differences with some other characteristics that will already effect outcome directly or through another path. Hence, all of these will be included in the simple difference between average of outcome of these 2 groups. That "misassigned" effect is called as treatment selection bias. We can think the selection bias as the difference between a treatment group and a control group if there was no treatment at all. We want to emphasize that we may not observe this difference, we may not verify that. However, the main purpose of all causal inference methods is to eliminate as much as possible this bias by imposing different identifying assumptions.

Heteregeneous treatment effect bias always exist if we want to calculate ATE. However, when we assume that treatment effects -dosage effect- are constant then this bias disappears. Even though this is a strong assumption, this is very common and plausible in social sciences and economics as we want to analyze average effects, not individual effect. That average treatment/causal effect is presented either treatment effect for average person or "homogeneous" average treatment effect for everyone. However, heterogeneous treatment effect and dealing its bias is one of the major topic in which machine learning methods are contributing recently.  

Decomposition of difference in means
$$
		\begin{eqnarray*}
			\underbrace{E[Y_{i}(1) | D=1] - E[Y_{i}(0) | D=0]}_{{\text{Simple Difference in Outcomes}}}&=& \underbrace{E[Y_{i}(1)] - E[Y_{i}(0)]}_{{\text{Average Treatment Effect}}} \\
			&&+ \underbrace{E[Y_{i}(0)|D=1] - E[Y_{i}(0) | D=0]}_{{\text{Selection bias}}}  \\
			&& + \underbrace{(1-\pi)(ATT - ATU)}_{{\text{Heterogenous treatment effect bias}}} 
		\end{eqnarray*}
		$$
		where $(1-\pi)$ is the share of the population in the control group.(Detailed derivation of this equation in Mixtape page 131-133)

As we mentioned the simple difference between the average outcome for the treatment group and the average outcome for the control group can be assumed by most as an average treatment effect. It may be true only if we do not have selection and heterogeneous treatment bias. However, most of the time already the difference exist between a treatment group and a control group before treatment implemented. Thus selection bias exists. 

Most of the time the treatment effects individuals as well as groups differentially. Thus, the average effect of treatment for the group consist from treated individuals and for the group consist from untreated individuals differ. The multiplication of that difference and the share of the population in the control group is called as Heterogenous treatment effect bias.

As previously noted, we are unable to directly observe individuals in both treatment and control states, making it impossible to explicitly calculate treatment effects and associated biases. Social scientists have been devising strategies to address these biases and estimate treatment effects, with machine learning methods contributing to these advancements in recent years. The various methodologies can be categorized as follows:

Regression, penalized regression, and fixed effects

Matching and propensity score methods

Randomization inference

Instrumental variables, difference-in-differences, regression discontinuity, and event studies

Synthetic control method

Causal forest method

In the upcoming chapters, we will delve into these approaches and explore the relevant machine learning techniques that complement and enhance these methods in estimating treatment effects.

