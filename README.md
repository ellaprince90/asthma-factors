Results

Tree-based machine learning models substantially outperformed linear baselines in predicting age-adjusted asthma emergency department (ED) visit rates. The tuned XGBoost model achieved strong predictive 
performance (R2: 0.90, RMSE: 21), representing a marked improvement over a mean-based baseline (Baseline RMSE: 65.89) and linear regression models (R2: 0.600 RMSE: 41.67. Visual inspection of predicted 
versus actual values demonstrated close alignment along the line of perfect prediction, indicating that the model captured meaningful structure in the data rather than simple noise.

SHAP (SHapley Additive exPlanations) analysis was used to interpret the fitted XGBoost model and identify the factors most strongly influencing predictions. Global SHAP feature importance revealed that race/ethnicity 
stratification—specifically the African American category—was the single most influential predictor of elevated asthma ED visit rates, exceeding the impact of age group, year, and geographic indicators. Age group 
(particularly the “Under 18” category) and temporal trends also contributed meaningfully, while individual counties exhibited smaller but non-negligible effects.

Discussion

The SHAP results indicate a pronounced disparity in asthma-related ED utilization associated with African American populations. Importantly, this finding reflects predictive association rather than causal inference. 
The dataset does not include information on environmental exposures, housing conditions, access to preventive care, insurance status, socioeconomic factors, or structural determinants of health that could explain 
the observed discrepancy. As a result, the underlying drivers of this elevated risk cannot be determined from the available data alone.

Rather than attributing causality, these findings should be interpreted as highlighting an area of significant inequity that warrants further investigation. The magnitude and consistency of the association suggest 
that unmeasured factors may play an important role in shaping asthma outcomes for African American communities.

Future work should incorporate richer individual- and community-level data, including environmental measures (e.g., air quality), healthcare access indicators, and socioeconomic variables, to better understand the 
mechanisms underlying this disparity. Such analyses are essential for informing targeted public health interventions and reducing preventable asthma-related morbidity.

Overall, this analysis demonstrates the value of interpretable machine learning methods for identifying high-risk populations while underscoring the importance of cautious interpretation and the need for more 
comprehensive data to move from prediction toward explanation and action.
