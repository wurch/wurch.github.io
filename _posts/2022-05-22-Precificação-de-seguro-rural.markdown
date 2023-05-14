---
layout: post
title: "Impacts of the Climatic Risk Agricultural Zoning (ZARC) in the precification of agricultural insurance"
date: 2022-05-22 12:30:00 -0000
---
> This text is an adaptation of the script used to present my final theses as a Bachelor of Actuarial Sciences. You can find the original version in this [link](https://www.anspnet.org.br/wp-content/uploads/2022/12/E-book_2022_compressed.pdf) at page 136 (the original text was written in Portuguese). This work received maximum grade and was published by the National Academy of Insurance and Welfare ([ANSP](https://www.anspnet.org.br/)) in December of 2022.

### Introduction

Given the efforts of the insurance market and the government's concern to understand how the climate impacts insurance modeling, this article evaluates the relationship between the rates practiced in agricultural insurance policies issued in Brazil and the risk indicator of the Climatic Risk Agricultural Zoning (ZARC), in order to comprehend if these elements are coherent between each other. Therefore, it is necessary to understand the concept of risk, the agricultural insurance product, and its operationalization difficulties, as well as the role of ZARC and its purpose of reducing the asymmetry of information and scarcity of data in this market and, finally, the comparison between rates, claims, and risk of policies issued from the Rural Insurance Premium Subsidy Program (PSR). 

### Market Challenges
![image tooltip here](/assets/images/banner.jpg)

Agricultural insurance pricing is a major challenge for insurers around the world, and this article aims to answer the following question: Are agricultural insurance premiums in Brazil consistent with the risk levels indicated by the Climatic Risk Agricultural Zoning (ZARC)? This study evaluates the relationship between the risk levels obtained from ZARC, both in the rates practiced by insurers and in the loss ratios of these insurance contracts.

In particular, it analyzes the policies issued under the Rural Insurance Premium Subsidy Program between the years 2017 and 2021

### Risks and Agricultural Insurance

![image tooltip here](/assets/images/risk_insurance.png)

When it comes to risk, it is the central element of insurance. In everyday life, we understand risk as the danger that something unwanted may happen to someone. In actuarial terms, this qualitative judgment of risk is suppressed, and it becomes a way of dealing with the financial consequences of a particular event. In the context of insurance, for a risk to be insurable, it must possess three main characteristics:
- It must be calculable;
- It must be collective;
- And it must represent a capital amount.

Insurance can be formally defined as a mutual agreement to compensate for the random consequences of events governed by the laws of statistics. It is considered an element of social balance because it proportionally mitigates the loss that would otherwise fall on only one individual across society as a whole. Insurance makes the community more stable by reducing the impact of unexpected events on the financial planning of economic agents.

Agricultural insurance, then, is specific financial protection against events resulting from meteorological phenomena. The coverage of this insurance protects the insured against losses caused by weather-related phenomena such as droughts, excessive rainfall, hailstorms, frosts, etc. A striking characteristic of this type of insurance is its high actuarial complexity. Even in a country as agrarian as ours, it still has a very low penetration rate. One of the reasons for the difficulty in marketing is that it breaks some insurability assumptions, which hampers the pricing by insurers. Therefore, it is rarely offered exclusively by the market. Even in countries where this product is already widely disseminated, such as the United States and Spain, the high percentage of insured area was only achieved because public agencies developed policies to encourage its commercialization.

### Agricultural Insurance in Brazil and Public Policies
![image tooltip here](/assets/images/seguro_brasil.png)

In Brazil, agriculture contributed 26% to the GDP and generated 9 million direct jobs. This highlights the importance of insurance in rural policy. Currently, the Rural Insurance Premium Subsidy Program (PSR) is in effect. It was introduced in 2002 and became law in December 2003. It provides support to farmers who want to protect their crops against climatic risks. The subsidy percentage varies according to the priorities of agricultural policy in a given year and represents around 30% to 35% of the premium.

In conjunction with the PSR and other public policies such as PROAGRO, there is also the Agroclimatic Risk Zoning. It is an agrometeorological study carried out by a team of agricultural engineers, statisticians, and meteorologists. Its objective is to define what, where, and when to plant. By cross-referencing location data, planting start dates, soil texture, and crop information, it classifies the risk level of the undertaking into a range of 20%, 30%, or 40%. These percentages represent the risk of production loss throughout the crop cycle due to the occurrence of climatic phenomena. In addition to the PSR, PROAGRO and PROAGRO Mais also rely on this risk indicator as a requirement for accessing credit.


### Analysis of Brazilian Insurance Data
All the data in this study were collected from public sources, and the cross-referencing between them allowed for this analysis to be conducted. The insurance policy data was collected from the database disclosed by SISSER, which is the system that manages PSR subsidies, and the soil texture data was obtained from the Soil Map of Brazil, a report produced by EMBRAPA. This allowed us to determine the risk level of the policies based on ZARC.

![image tooltip here](/assets/images/fonte_dados.png)

After all the data cross-referencing and cleaning, we ended up with a sample of 64,000 policies for the crops of soybean, second-season corn, and wheat. The total population of these three crops is around 328,000 policies in the original database, so the obtained sample greatly exceeds the minimum sample size required for an analysis with a 99% confidence level and a 1% margin of error. Additionally, a subset of this sample was extracted, containing only second-season corn policies located in Paraná. The purpose of this subset, referred to as 'Group 2' throughout the graphs, is to isolate variables that could bias the pricing, such as crop type, planting location, and soil type. In this case, the determining factor for the risk level is primarily the date.

![image tooltip here](/assets/images/localizacao_apolices.png)

Regarding the loss ratio of these groups, when evaluating the closed policies until June 2020 and grouping them by risk level, we can observe that in Group 1, the loss ratio reflects the respective expected risk level of the contracts. Despite the magnitude of the loss ratio varying from year to year, the consistency of the indicator is maintained. However, for the subset, which is Group 2, the data does not maintain consistency throughout all the years. Although the policies issued in 2019 are ordered by risk as expected, the erratic behavior of the loss ratio in the policies from 2018 and 2017 may indicate the occurrence of some acute climatic event that affected these contracts.

![image tooltip here](/assets/images/sinistralidade_risco_ano_milho_pr.png)

According to a news article published by Gazeta do Povo in 2018, there was indeed a crop failure that year due to drought, and in 2017, the crop yield for this particular crop exceeded expectations.

It is also important to note how the magnitude of the loss ratios varies collectively from year to year in both groups. Group 1, which has high diversification, experiences increases and decreases in the loss ratio in the same years as Group 2, which is the highly concentrated group. This behavior exemplifies the systemic nature of agricultural risks.

Now, focusing directly on the object of this study, which is the rates by risk level, the graphs demonstrate that for Group 1, although the medians of each group are staggered, the interquartile range and the minimum and maximum values are in the reverse order.

![image tooltip here](/assets/images/boxplot_taxas_grupos.png)

For Group 2, there are some more abrupt distortions worth noting: in addition to the median of the 40% risk group being lower than that of the 20% group, the maximum and minimum values are also respectively lower.

Given this apparent greater divergence between the rates of 20% and 40% in Group 2, a hypothesis test was conducted to validate the statistical significance of the observed behavior. The formulated hypotheses were:"

- $$H_0$$: On average, the ZARC risk classification does not affect the policy rates;
- $$H_1$$: Distribution X (20% risk) is higher than distribution Y (40% risk).

The obtained result is a $$\textit{p-value}<0.001$$, therefore we reject the null hypothesis and can assume that, on average, the rates of Group 2 for policies with a 40% risk level are lower than the rates of policies with a 20% risk level. This demonstrates a mismatch between the pricing of insurance companies and the risk level indicated by the Agricultural Zoning of Climatic Risks.

### Conclusions
Therefore, the findings obtained from the data analysis lead us to the conclusion that, despite the significant efforts made in implementing the ZARC and its demonstrated ability to discriminate between levels of loss, the indicated risk level does not correlate with the rates practiced in agricultural insurance policies. Over the three years analyzed, the indicator showed consistency with the observed loss experience, where higher assessed risk corresponded to higher loss ratios across the contract portfolio. However, this same trend did not hold when comparing the rates charged by the contracts, leading us to the conclusion that the Brazilian insurance market does not utilize the technological inputs of the Agricultural Zoning of Climatic Risks to price policies more accurately and with more customization. 

Furthermore, the subsidy percentage could be linked to the indicated risk level for a specific crop, encouraging safer agricultural ventures and making the agricultural insurance market more sustainable in the long term.

For years, the Brazilian government and state governments have been trying to establish insurance as the main instrument for rural policy protection. However, as we have seen from the adoption rate of this product, the desired success has not yet been achieved. Nevertheless, the two initiatives addressed in this study have proven to be successful in their intended purposes and hold promise:
- The **PSR** (Program for Subsidizing Agricultural Insurance Premiums), which is in effect nationwide and also applies to state-level counterparts, has been expanding its coverage area, reaching more and more producers.
- And also the **ZARC** (Agricultural Zoning for Climatic Risk), which, as demonstrated earlier, fulfills its intended purpose and determines the most suitable planting periods. 

Countries like the United States and Spain took years to develop their agricultural insurance models, and there is no reason for Brazil to be any different.
