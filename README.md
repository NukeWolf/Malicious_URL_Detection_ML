# Dataset
[Dataset to install](https://www.kaggle.com/datasets/sid321axn/malicious-urls-dataset/code)
# How to run

## Main Analysis 1
For our primary analysis, ensure that `malicious_phish.csv` dataset is downloaded. It should be included in this repository.

 Open the `dataset_analysis.ipynb` file. Ensure that `file_path` points correctly to the dataset. Run all blocks of code and read results. The code is split up into 3 sections.

 - The first half of the cells are feature extraction cells.
 - We then drop unecessary headers, split the data and prepare to run our classification models.
 - After running our classifiers, we plot and analyze feature correlations and perform an adversial attack.

## HTTP Request Analysis 2

The secondary HTTP Request analysis follows a similar format, but gathering HTTP Request data is performed in a different notebook. If you'd like to skip the scraping step, partially scraped data is already stored in `malicious_html_enhanced.csv`.

1. To web scrape data, open the `HTML_Scraper.ipynb` file. Set the `original_dataset_path` to the csv of the original downloaded dataset. 
2. Set `new_dataset_path` to the name for your new dataset csv with HTTP Request data. 
3. HTML files will be downloaded in the `html_file_folder_path`, ensure that the folder exists.
4. Run the bottom code block. This will take multiple hours.

To run the analysis, open the `HTTP_analysis.ipynb`file and follow the same instructions above except insure that file_path points to our `new_dataset_path`. By default, the file included is `malicious_html_enhanced.csv` in this repo.