# capstone401-latino-voters
This project serves to understand the current factors contributing to Latino voters' evolving political identity and engagement. Research and data analyses explore the intersection of Latino identity, Americanization, and the U.S.'s evolving political landscape to better understand this critical voting bloc’s role in shaping American democracy. 

Below is my most updated methodology (4/5/25):

Methodology 
This study investigates how the development of party identification has contributed to the increase in Republican vote share among Latino voters in recent years, specifically focusing on the moderating effects of religiosity and political assimilation. I conducted a quantitative analysis using the American National Election Study (ANES) survey data from 2012, 2016, 2020, and 2024 waves.  To address the above research question, this study will examine the associations between party identification, religiosity, political assimilation, and Republican vote choice among Latino respondents. As ANES comprises survey-based data (ANES, 2024), this study follows a non-experimental, correlational design.

Associations & Limitations in Causality

This study aims to determine whether party identification is a significant predictor of republican vote choice and how religiosity and political assimilation moderate this relationship. As ANES comprises survey data, this study cannot establish causality. Party identification and religiosity are self-reported, so external factors may confound the relationship and the republican vote choice. This may include family socialization, media influence, or economic conditions (Collingwood, Barreto, Garcia-Ríos, 2014) (Garcia-Ríos, Barreto, 2016). On the other hand, reverse causality is possible, signifying that vote choice also reinforces party identification over time. 

Alternative Research Design

A longitudinal panel study tracking the same Latino voters across multiple election cycles would be ideal to strengthen causal inference. This may help distinguish whether changes in religiosity or political assimilation precede shifts in vote choice. While ANES has panel studies available, I will utilize the time series studies since my analysis will be trend-based, looking at population-level shifts instead of individual changes presented in the available panel.
Despite the limitation in causal inference, this study can identify significant associations between key political variables via statistical analysis. This will allow for trend identification in Latino Republican vote share over time to understand the associated factors of the Latino republican shift in recent years.  

This research design aligns with methodological models from prior studies. Valenzuela (2014) used logistic regression and subgroup analysis with the 2006 Latino National Survey to examine how religious commitment influences political preferences. His use of interaction terms to capture differences within religious groups influenced this study’s approach to modeling the effects of religiosity. Similarly, Cardenas et al. (2023) utilized logistic models to explore how racialized Latino identity shapes political engagement. Cardenas et al. (2023) also highlight generational status and political discussion in its study. Valenzuela’s (2014) and Cardenas et al.'s (2023) research designs and models support the analytical framework used in this study and reinforce the importance of subgroup and interaction-based modeling.

Data Source

The ANES is a nationally representative survey that collects data on American registered voters’ political attitudes, voting behavior, and socioeconomic demographics. Every ANES for the years I have selected is a two-wave panel design with pre-election and post-election interviews. The ANES includes a substantial sample of Latino respondents across multiple election cycles. Using harmonized datasets from 2012, 2016, 2020, and pre-election 2024, I filtered for Latino respondents using the year-specific Hispanic identity variables (dem_hisp, V161309, V201549x, V241501x). Sample sizes range from 450 to over 5,900 Latino respondents per wave. 

I chose these years because previous studies had associated Latinos as strong supporters of democratic policies and candidates before 2020 (Huddy, Mason, Horowitz, 2016). The 2020 presidential election marked noticeable shifts in Latino political partisanship from Democratic to Republican (Dominguez-Villegas, Rios, 2022). 

Dependent Variable Standardization

The dependent variable is a binary variable of Republican Vote Choice, recoded as 1= voted Republican (eg., Trump) , 0= voted otherwise (e.g, Democrat or Third Pary). Coding varies by years but consistently derived from the ANES presidential vote item (postvote_presvtwho, V162034a, V202073, V241039). 

Independent Variable Standardization

My independent variables are partisan identification, religiosity, and political assimilation. 
Partisan identification is represented as a five-level categorical variable: strong Republican, lean Republican, Independent, lean Democrat, and strong Democrat. 
Religiosity is operationalized using frequency of religious service attendance. This variable is available in ANES across all selected years.
Political assimilation is measured through a composite index of four indicators: 
English proficiency: recoded on a scale so higher values represent greater assimilation (e.g “Only English” = most assimilated), 
Political discussion frequency: recoded and standardized across all waves,
Voter participation history: binary (voted or not in the last presidential election), standardized for the index composite,
 Generational status (1= both parents born in U.S, 2= one parent, 3= neither). 
Each indicator of the political assimilation index is standardized using a z-score, and the final assimilation index is calculated by averaging the four standardized components.

Control Variables

The control variables for this study include demographics: age, gender, social class, and education level. Social class was self-identified by respondents, except in the 2024 wave. For 2024, I recoded and standardized the respondents’ income to be consistent with the prior waves.  Education was recoded into an 8-level ordinal scale for consistency across waves and is treated as a categorical variable in the model. 
Logistic regression
I use logistic regression models to estimate the likelihood of voting Republican. Republican vote choice is the binary outcome. Predictor variables include party ID, religiosity, political assimilation, and all control variables.  

Interaction Terms

To better capture how the relationship between variables changes depending on the level of another variable, I introduced interaction terms in the logistic regression model. It allowed for deeper insight into the dynamics of Latino republican voter shifts and identification of more nuanced relationships between the key variables. 
I added (party id x religiosity) to reveal if partisan identification affects the respondent’s level of religiosity. Political assimilation was also tested to see if it amplified the effect of party identification. This choice was made to help analyze how such a relationship varied across Latino generation subgroups in party identification and vote choice. Previous studies have concluded that first-generation Latinos rely more on ethnic group identity, while later-generation Latinos vote more strictly among party lines (Angel, Garcia-Ríos, 2024).

Comparative Analysis of Generational Status 

I stratified the sample by generational status to compare patterns in political assimilation and voter behavior among immigrant, first, second, and third-generation Latino respondents. 

Assumption Checking: Multicollinearity

I tested for multicollinearity among predictor variables through a variance inflation factor analysis. (PennState STAT 462: Applied Regression Analysis, 2018). 

