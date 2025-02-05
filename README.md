# UGC(University Grant Commission)
A Machine Learning model to identify colleges that deserve grant and that do not, where grant level 0 indicates no grant and grant level 6 indicates maximum grant . This means grant ranges from 0 to 6.
There was no real time data available which showed if a college deserved grant or not. 
So I made a synthetic data for colleges in which there are two sheets in one excel file ,one is City_Locality having three columns state, city, locality_category and other is Colleges having 14 columns 'Unnamed: 0', 'College_ID', 'College_Name', 'State', 'City', 'Locality_Category', 'Economic_Location', 'Locality_Score', 'Tuition_Fees', 'Facilities_Score', 'Academic_Excellence', 'Sports_Excellence', 'Number_of_Students', 'College_Type'.
 This are the factor that show how much grant should a college get'Locality_Category', 'Economic_Location', 'Locality_Score', 'Tuition_Fees', 'Facilities_Score', 'Academic_Excellence', 'Sports_Excellence', 'Number_of_Students', 'College_Type'.
Colleges in rich locality or rich economic area will not get 4 5 6 level grant . 
Colleges having high academic or high sports will have 3 4 5 6 level of grant and colleges with both will have 4 5 6 level of grant , irrespective of other factors . 
Colleges with 250 to 500 students will get 0 1 2 level of grant considering their locality , economical area , sports , academic and tuition. 
Also colleges with 500 to 1000 or 1000+ students will have 3 4 5 6 level of grant considering different factors. 
Engineering and Medical colleges will never have 0 or 1 as their grant unless engineering colleges tuition per year is more than 2 lakhs per year and medical colleges has tuition 5 lakh per year.
A Random Forest CLassifier is used to find how accurate our model is.
A bar graph showing colleges which have received grant which have not is also made with a feature importance graph showing which feature affects the grant level the most.
