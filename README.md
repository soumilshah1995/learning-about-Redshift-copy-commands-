# learning-about-Redshift-copy-commands-
learning about Redshift copy commands 

### Tutorial  https://www.youtube.com/watch?v=cevJYWBWzsI


```

CREATE TABLE "Employees" (
  Name varchar(255) default NULL,
  Number varchar(255) default NULL,
  Country varchar(255) default NULL,
  ZIP varchar(255) default NULL,
  Birthday varchar(255),
  Sex varchar(255) default NULL,
  MaritalStatus varchar(255) default NULL,
  DateOfHire varchar(255),
  DateOfTermination varchar(255),
  ReasonForTermination varchar(255) default NULL,
  EmploymentStatus varchar(255) default NULL,
  Department varchar(255) default NULL,
  PerformanceScore varchar(255) default NULL,
  City varchar(255)
);
```

```

copy Employees
from 's3://XXXX'
credentials
'aws_access_key_id=XXXXXX;aws_secret_access_key=XXXX'
csv;
```
