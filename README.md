# Generate Analytics Report
To generate the analytics report follow the steps.

## Setup
You'll want to clone the repo.

```
If you have any trouble doing this, 
- you can download the zip folder of this repo and then extract the files to a local file. 
- Once you have all the files cloned locally, you should make sure you have all the necessary libraries installed.
```
$ pip install fpdf
$ pip install pandas numpy matplotlib
$ pip install plotly
$ pip install -U kaleido
```
$ pip install numpy==1.19.3 is the best if you have any problem in the current version
```
To test if everything is set up properly now
- Try running `python generate_report.py`. You should get a fresh report file. 
- You'll have to change `helper.py` to read from the online version of the data if you want to access the previous day (uncomment the BASE_PATH URL and comment BASE_PATH='./data'). 
- You will also have to comment out the hard coded date at the bottom of `generate_report.py` file. I saved it this way so not too many unneccesary requests to the GitHub server were made while testing.
- Delete the `report.pdf` before you run the code.
