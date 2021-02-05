# pyPcapAnalysis
This is a quick guide to getting started with exploratory pcap analysis using python. There's no one right to do exploratory analysis -- this just summarizes my personal approach / workflow. 

## Usage

1. install the prerequisites python libs and either nteract or Jupyter. (see below)
2. look at the pcapAnalysis.ipynb notebook for a simple example of parsing, aggregating, and plotting some simple statistics on the packet traces. 

## Prerequisites

- Python 3.X 

**Python libraries**

If you are on ubuntu/linux, you can install these libraries through apt and or pip. If you are on windows or osx, it may be easier to install the anaconda package manager, then install the libraries through that https://www.anaconda.com. Anaconda is a good option on linux too. 

- dpkt (for parsing packets) https://dpkt.readthedocs.io/en/latest/index.html

- pandas (for storing parsed analysis data) https://pandas.pydata.org

- seaborn (for plotting data stored in pandas frames) https://seaborn.pydata.org

- [optional] scipy (for advanced statistical functions) https://www.scipy.org

- [optional] scikit-learn (for ML tools) https://scikit-learn.org/stable/

**Interactive notebooks**
I use python notebooks for exploratory analysis. The alternative, doing the analysis from regular python scripts, breaks my concentration and gets tedious, e.g., because you have to switch between a text editor (for changing analysis), command prompt (for running scripts), and images / windows (for viewing results). 

- For running notebooks locally (on your laptop), I like nteract https://nteract.io

- For running notebooks remotely, use Jupyter. You will need to install a local copy of jupyter on the remote server you want to work on, then start a jupyter server process. Then, you will be able to access your notebooks over http. (I will add more information about how to do this in a bit.) https://jupyter.org


## Datasets

This uses example.pcap, which is 100K packets from "bigFlows.pcap" at https://tcpreplay.appneta.com/wiki/captures.html
