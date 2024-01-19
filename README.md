# codsoft_taskno_4
<h1>Author : VEDANT GHADGE</h1>

<h1>Title : Sales Prediction Using Python</h1>



<h2>Introduction :</h2>
<p>The main goal of this project is to forecast sales by looking at how much money is spent on advertising across different platforms like TV, Radio, and Newspaper. The dataset we have includes details about how much is spent on advertising on these platforms, and alongside that, it shows the actual sales that resulted from those advertising efforts. The idea is to analyze this information to create a prediction model for future sales based on advertising expenses.</p>

<h2>Dataset</h2>
<p>In this project, the primary dataset used is the "advertising.csv" file, which serves as the cornerstone of our analysis. This dataset encapsulates information related to advertising expenditures across three distinct platforms: TV, radio, and newspaper. Each entry in the dataset is characterized by four columns—namely, 'TV', 'radio', 'newspaper', and 'sales'. The 'TV', 'radio', and 'newspaper' columns denote the corresponding advertising expenditures on these channels, while the 'sales' column represents the resultant sales figures. This structured dataset forms the basis of our exploration, allowing us to delve into the relationships between advertising investments and subsequent sales outcomes across different mediums.</p>

<h2>Library Used</h2>
<p>Following Libraries were used in the project :</p>
<ul><li>pandas</li>
    <li>numpy</li>
    <li>matplotlib</li>
    <li>sklearn.model_selection.train_test_split</li>
    <li>sklearn.model_selection.LinearRegression</li>
</ul>

<h2>Data Exploration and Preprocessing</h2>
<ul>
    <li>The structure and summary statistics of the dataset were unveiled through the implementation of `df.shape` to ascertain its dimensions and `df.describe()` to present a comprehensive overview of its key statistical measures.</li>
    <li>Missing values in the dataset were checked using df.isna().sum().</li>
    <li>If any missing values are found they were droped by df.dropna() function.</li>
</ul>


<h2>Data Visualization</h2>
<ul>
    <li>A scatter graph was created to visualize the relationship between advertising expenditure on TV, Radio, Newspaper, and sales using plt.scatter to identify correct correlation between them.</li>
    <li>According, to given scatter graphs
        <ol><li>TV vs Sales ----> High degree +ve correlation</li>
            <li>Radio vs Sales ----> No Correlation</li>
            <li>Newspaper vs Sales ----> No Correlation</li></li>
        </ol>
</ul>


<h2>Model Training</h2>
<ul>
    <li>The dataset was divided into training and testing sets using `train_test_split`.</li>
    <li>A linear regression model was trained on the training data using `sklearn.linear_model.LinearRegression`.</li>
    <li>2d Scatter Graphs are created for Regression (Test Set) and Regression (Train Set) between TV advertising and Sales</li>
</ul>

<h2>Model Results</h2>
<ul>
    <li>The model predicted sales for the test set based on TV advertising expenses using `linear_model.predict(x_test)` and the corresponding TV advertising expenditures in the test set.</li>
    <li>R2 Score was calculated which was 81% using 'r2_score(y_test,y_predict)'</li>
    <li>Mean Squared Error was calculated which was 5.405 using 'mean_squared_error(y_test,y_predict)'</li>
</ul>

<h2>Testing Model</h2>
<ul>
    <li>The model coefficients and intercept were extracted using `linear_model.coef_` and `linear_model.intercept_`.</li>
    <li>x_test value was accepted and printed the prediction sales</li>
</ul>
