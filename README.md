# psycopg2-aws-lambda

This is a custom compiled psycopg2 C library for Python, this covers the problem of: 
AWS Lambda missing the required PostgreSQL libraries in the AMI image. This usualy happens
with the following error message

```No module named 'psycopg2._psycopg': ModuleNotFoundError```

**Details** 

- This package was compiled using AWS EC-2 instance AMI: Amazon Linux AMI 2018.03.0 (HVM), SSD Volume Type.
- Python 3.7
- PostgreSQL: 11.6
- psycopg2: 2.8.5

**Usage**

Just copy the psycopg2 directory and paste it into your AWS Lambda zip package.

## References

Check @jkheler GitHub for more details: https://github.com/jkehler/awslambda-psycopg2
