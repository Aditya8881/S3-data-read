# S3-data-read
How to read S3 data in Pycharm using boto3

import boto3
import pandas as pd
client = boto3.client('s3')
path = "s3://avd1145/bank-full.csv"

df = pd.read_csv(path)
print(df.head(10))
