# spark-demo
The same Python job , how to run on Spark standalone environment.  Python package and submit a job source code and main function to Spark. 
<pre>
How to package Python source code for Spark
1.python -m venv pyspark_venv
./pyspark_venv/Scripts/activate
pip freeze > requirements.txt
pip install -r requirements.txt
zip whole project to app.zip
create a app.py main function

How to submit a Python Job on Spark standalone environment
2.submit python src and app.py main function file to master node on standalone mode
(pyspark_venv) PS C:\Users\liuji\PycharmProjects\pythonProject\spark-demo> Spark-submit --master spark://192.168.1.105:7077 --py-files app.zip app.py
Hello world! running python on spark standalone
</pre>
