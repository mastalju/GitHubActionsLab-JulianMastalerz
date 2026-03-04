# Purpose of dependent-jobs workflow
this workflow demonstrates how to control the order of job execution using needs key. The jobs have been written to run in the order build -> test -> deploy

# Key Concepts
needs: makes sure that the jobs run in correct order. For example if test needs build  then it will never be able to run first. Build will have to run first.
runs-on: specifies envrionment that job will run on. In this workflow it was ubuntu-latest

# Challenges Faced
I was having trouble when I pushed the file to github but then i changed a permission setting on github and it worked properly

# Purpose of multi-platform workflow
This workflow demonstrates running 3 jobs at the same time on different OS

# Key Concepts:
runs-on: specifies envrionment that job will run on. Each job here was on a different environment (ubuntu, windows, mac)
env: makes it so you can use environment variables in workflow jobs.

# Challenges Faced:
I was a bit confused with the sytax but I resolved this by reffering to what we did in the lecture and the starter workflow that github gave.
