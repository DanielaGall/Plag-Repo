# Plag-Repo
The basic premise for this plagiarism detection is to accept resources in a few different formats (URL being the most popular, but also text files and Office-type documents). The resources can then be periodically scanned (via custom management commands triggered via a crontab), and a few fairly unique phrases are pulled out of them. These phrases are then searched online (using Bing's search engine API), and the results are the 'plagiarism-detected' candidates. Finally these candidates are scanned to rule out any false positives, and discover an approximate duplication score.
