## Project 2: Ames Housing Data and Kaggle Challenge
## Problem Statement
To create a sales home price prediction model for property agent so as to maximize their profit and efficiency in acquiring listing within Ames. And to give a true valuation for home owners as well. 
## Executive Summary
Through our research on the Ames Housing Data, we noticed that there are 3 neighborhood in Ames that are consistently selling at higher price compared to other neighborhood. The 3 neighborhoods are Stone Brook, Northridge, and Northridge Heights. And we also notice these neighborhoods tend to be residential property and are newly built in the year 2000. Therefore, agent can concentrate on these neighborhoods to maximize their commissions and efficiently source for listings within that vicinity. 
## Data Dictionary
|Feature      |Type      |Dataset  |Description|
|---------    |------    |---------|-----------|
|**id**        |int    |train/test  |ID|
|**pid**        |int    |train/test  |Postal Identification |
|**ms_subclass** |int    |train/test  |Building class|
|**ms_zoning**    |object    |train/test  |General zoning classification|
|**lot_frontage**        |float    |train/test  |Linear feet of street connected to property|
|**lot_area**        |int    |train/test  |Lot size in square feet|
|**street**        |object    |train/test  |Type of road access to property|
|**alley**        |object    |train/test  |Type of alley access to property|
|**lot_shape**        |object   |train/test  |General shape of property|
|**land_contour**        |object    |train/test  |Flatness of the property|
|**utilities**        |object   |train/test  |Type of utilities available|
|**lot_config**        |object    |train/test  |Lot configuration|
|**land_slope**        |object    |train/test  |Slope of property|
|**neighborhood**        |object    |train/test  |Physical locations within Ames city limits|
|**condition_1**        |object    |train/test  | Proximity to main road or railroad|
|**condition_2**        |object    |train/test  |Proximity to main road or railroad (if a second is present)|
|**bldg_type**        |object    |train/test  |Type of dwelling|
|**house_style**        |object    |train/test  |Style of dwelling|
|**overall_qual**        |int    |train/test  |Overall material and finish quality|
|**overall_cond**        |int    |train/test  |Overall condition rating|
|**year_built**        |int    |train/test  | Original construction date|
|**year_remod/add**        |int    |train/test  |Remodel date|
|**roof_style**        |object    |train/test  |Type of roof|
|**roof_matl**        |object    |train/test  |Roof material|
|**exterior_1st**        |object    |train/test  |Exterior covering on house|
|**exterior_2nd**        |object    |train/test  |Exterior covering on house|
|**mas_vnr_type**        |object    |train/test  |Masonry veneer type|
|**mas_vnr_area**        |float    |train/test  |Masonry veneer area in square feet|
|**exter_qual**        |object    |train/test  |Exterior material quality|
|**exter_cond**        |object    |train/test  |Present condition of the material on the exterior|
|**foundation**        |object    |train/test  |Type of foundation|
|**bsmt_qual**        |object    |train/test  |Height of the basement|
|**bsmt_cond**        |object    |train/test  |General condition of the basement|
|**bsmt_exposure**        |object    |train/test  |Walkout or garden level basement walls|
|**bsmtfin_type_1**        |object    |train/test  |Quality of basement finished area|
|**bsmtfin_sf_1**        |float    |train/test  |Type 1 finished square feet|
|**bsmtfin_type_2**        |object    |train/test  |Quality of second finished area|
|**bsmtfin_sf_2**        |float    |train/test  |Type 2 finished square feet|
|**bsmt_unf_sf**        |float    |train/test  |Unfinished square feet of basement area|
|**total_bsmt_sf**        |float    |train/test  |Total square feet of basement area|
|**heating**        |object    |train/test  |Type of heating|
|**heating_qc**        |object    |train/test  |Heating quality and condition|
|**central_air**        |object    |train/test  |Central air conditioning|
|**electrical**        |object    |train/test  |Electrical system|
|**1st_flr_sf**        |int    |train/test  |First Floor square feet|
|**2nd_flr_sf**        |int    |train/test  |Second floor square feet|
|**low_qual_fin_sf**        |int    |train/test  |Low quality finished square feet |
|**gr_liv_area**        |int    |train/test  |Above grade (ground) living area square feet|
|**bsmt_full_bath**        |float    |train/test  |Basement full bathrooms|
|**bsmt_half_bath**        |float    |train/test  |Basement half bathrooms|
|**full_bath**        |int    |train/test  |Full bathrooms above grade|
|**half_bath**        |int    |train/test  |Half baths above grade|
|**bedroom_abvgr**        |int    |train/test  |Number of bedrooms above basement level|
|**kitchen_abvgr**        |int    |train/test  |Number of kitchens|
|**kitchen_qual**        |object    |train/test  |Kitchen quality|
|**totrms_abvgrd**        |int    |train/test  |Total rooms above grade|
|**functional**        |object    |train/test  |Home functionality rating|
|**fireplaces**        |int    |train/test  |Number of fireplaces|
|**fireplace_qu**        |object    |train/test  |Fireplace quality|
|**garage_type**        |object   |train/test  |Garage location|
|**garage_yr_blt**        |object    |train/test  |Year garage was built|
|**garage_finish**        |object    |train/test  |Interior finish of the garage|
|**garage_cars**        |float    |train/test  |Size of garage in car capacity|
|**garage_area**        |float    |train/test  |Size of garage in square feet|
|**garage_qual**        |object   |train/test  |Garage quality|
|**garage_cond**        |object    |train/test  |Garage condition|
|**paved_drive**        |object    |train/test  |Paved driveway|
|**wood_deck_sf**        |int    |train/test  |Wood deck area in square feet|
|**open_porch_sf**        |int    |train/test  |Open porch area in square feet|
|**3ssn_porch**        |int    |train/test  |Three season porch area in square feet|
|**screen_porch**        |int    |train/test  |Screen porch area in square feet|
|**pool_area**        |int    |train/test  |Pool area in square feet|
|**pool_qc**        |object    |train/test  |Pool quality|
|**fence**        |object    |train/test  |Fence quality|
|**misc_feature**        |object    |train/test  |Miscellaneous feature not covered in other categories|
|**misc_val**        |int    |train/test  |Value of miscellaneous feature|
|**mo_sold**        |int    |train/test  |Month Sold|
|**yr_sold**        |int    |train/test  |Year Sold|
|**saleprice**        |int    |train/test  |property's sale price in dollars|
## Conclusions and Recommendations

**Property Agent:**
Agent can utilize this model to target the top 3 neighborhood in Ames and give a true valuation to home owners. And from the above violinplot it also shows that most property sold in Ames belong to the residential category. Thus, agent can focus their sales on residential property as compared to other categories. And the top 3 neighborhood that are built 1990s onwards will enable them to fetch the highest sale price and therefore, maximum profit.

**Recommendation:**
More economic data could be given such as the unemployment rate, inflation rate and interest rate. 
More informations on property buyers such as the type of property buyers, age, size of family and nationality. 
The overall population demographics in Ames to get a better understanding of the property buyers pattern. 
