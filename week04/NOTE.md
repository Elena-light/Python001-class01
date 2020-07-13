学习笔记

import pandas as pd 
from sklearn import datasets

iris = datasets.load_iris()
X, y = iris.data, iris.target

import os
pwd = os.path.dirname(os.path.realpath(__file__))
book = os.path.join(pwd, 'data.csv')
df = pd.read_csv(book)
